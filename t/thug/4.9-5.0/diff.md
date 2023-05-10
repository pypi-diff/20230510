# Comparing `tmp/thug-4.9.tar.gz` & `tmp/thug-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-4.9.tar", last modified: Fri Mar 10 14:03:18 2023, max compression
+gzip compressed data, was "thug-5.0.tar", last modified: Wed May 10 07:26:43 2023, max compression
```

## Comparing `thug-4.9.tar` & `thug-5.0.tar`

### file list

```diff
@@ -1,518 +1,518 @@
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.306868 thug-4.9/
--rw-r--r--   0 buffer     (502) staff       (20)    17987 2022-12-28 14:31:40.000000 thug-4.9/LICENSE.txt
--rw-r--r--   0 buffer     (502) staff       (20)      130 2023-01-03 13:39:45.000000 thug-4.9/MANIFEST.in
--rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-03-10 14:03:18.306562 thug-4.9/PKG-INFO
--rw-r--r--   0 buffer     (502) staff       (20)     2676 2023-01-17 09:44:55.000000 thug-4.9/README.rst
--rw-r--r--   0 buffer     (502) staff       (20)     3502 2023-03-10 10:37:22.000000 thug-4.9/pyproject.toml
--rw-r--r--   0 buffer     (502) staff       (20)      341 2023-03-10 10:36:03.000000 thug-4.9/requirements.txt
--rw-r--r--   0 buffer     (502) staff       (20)       38 2023-03-10 14:03:18.306950 thug-4.9/setup.cfg
--rw-r--r--   0 buffer     (502) staff       (20)     1346 2023-01-03 12:33:41.000000 thug-4.9/setup.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:17.862786 thug-4.9/thug/
--rw-r--r--   0 buffer     (502) staff       (20)     8196 2022-11-04 15:21:57.000000 thug-4.9/thug/.DS_Store
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:17.874210 thug-4.9/thug/ActiveX/
--rw-r--r--   0 buffer     (502) staff       (20)     7598 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer     (502) staff       (20)    64018 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.014772 thug-4.9/thug/ActiveX/modules/
--rw-r--r--   0 buffer     (502) staff       (20)      400 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)     1119 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer     (502) staff       (20)     2573 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer     (502) staff       (20)     1482 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer     (502) staff       (20)     1086 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer     (502) staff       (20)      979 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer     (502) staff       (20)      801 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer     (502) staff       (20)      567 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer     (502) staff       (20)      421 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer     (502) staff       (20)      600 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer     (502) staff       (20)      726 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer     (502) staff       (20)      307 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer     (502) staff       (20)      673 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer     (502) staff       (20)      447 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer     (502) staff       (20)      625 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer     (502) staff       (20)      404 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer     (502) staff       (20)     1857 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer     (502) staff       (20)     1500 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer     (502) staff       (20)      825 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)     3049 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)     2221 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer     (502) staff       (20)      496 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer     (502) staff       (20)      656 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer     (502) staff       (20)      420 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer     (502) staff       (20)      561 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer     (502) staff       (20)     4119 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      443 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer     (502) staff       (20)      945 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer     (502) staff       (20)      672 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer     (502) staff       (20)     1964 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer     (502) staff       (20)      405 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer     (502) staff       (20)      601 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer     (502) staff       (20)      535 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer     (502) staff       (20)     4390 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer     (502) staff       (20)     2048 2023-01-13 08:09:32.000000 thug-4.9/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer     (502) staff       (20)     8006 2023-01-06 14:50:41.000000 thug-4.9/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer     (502) staff       (20)      466 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer     (502) staff       (20)      438 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer     (502) staff       (20)      589 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer     (502) staff       (20)     1259 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer     (502) staff       (20)      616 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer     (502) staff       (20)     3311 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)     1175 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer     (502) staff       (20)     1057 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer     (502) staff       (20)     1201 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      498 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer     (502) staff       (20)      494 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)      973 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer     (502) staff       (20)     2335 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      348 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)      831 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer     (502) staff       (20)      449 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer     (502) staff       (20)     1116 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer     (502) staff       (20)     1027 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer     (502) staff       (20)     5185 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer     (502) staff       (20)     1527 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer     (502) staff       (20)      273 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer     (502) staff       (20)      921 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer     (502) staff       (20)     1472 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer     (502) staff       (20)      715 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer     (502) staff       (20)      906 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer     (502) staff       (20)      677 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer     (502) staff       (20)     2436 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer     (502) staff       (20)      516 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer     (502) staff       (20)     1061 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer     (502) staff       (20)     2224 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/SymantecBackupExec.py
--rw-r--r--   0 buffer     (502) staff       (20)     4772 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer     (502) staff       (20)      391 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer     (502) staff       (20)      691 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer     (502) staff       (20)     1763 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer     (502) staff       (20)      719 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer     (502) staff       (20)      796 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer     (502) staff       (20)      132 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1280 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer     (502) staff       (20)     1689 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer     (502) staff       (20)     8980 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer     (502) staff       (20)      213 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer     (502) staff       (20)      645 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer     (502) staff       (20)     1373 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      599 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer     (502) staff       (20)      145 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer     (502) staff       (20)      942 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer     (502) staff       (20)     1026 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer     (502) staff       (20)     1159 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer     (502) staff       (20)     1077 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)     1244 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer     (502) staff       (20)     1932 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer     (502) staff       (20)     2870 2022-12-28 14:31:40.000000 thug-4.9/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.015558 thug-4.9/thug/Analysis/
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.017295 thug-4.9/thug/Analysis/awis/
--rw-r--r--   0 buffer     (502) staff       (20)     3224 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.019883 thug-4.9/thug/Analysis/context/
--rw-r--r--   0 buffer     (502) staff       (20)     1554 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.021957 thug-4.9/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer     (502) staff       (20)     4000 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.023359 thug-4.9/thug/Analysis/screenshot/
--rw-r--r--   0 buffer     (502) staff       (20)     1333 2023-03-07 14:57:11.000000 thug-4.9/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.025115 thug-4.9/thug/Analysis/shellcode/
--rw-r--r--   0 buffer     (502) staff       (20)     8069 2023-01-13 08:09:32.000000 thug-4.9/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.038880 thug-4.9/thug/Classifier/
--rw-r--r--   0 buffer     (502) staff       (20)     4908 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2106 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2159 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2070 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2008 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2243 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2082 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2330 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)     2014 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.102637 thug-4.9/thug/DOM/
--rw-r--r--   0 buffer     (502) staff       (20)     2534 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Alexa.py
--rw-r--r--   0 buffer     (502) staff       (20)     2324 2023-03-07 14:57:11.000000 thug-4.9/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer     (502) staff       (20)     2254 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Chrome.py
--rw-r--r--   0 buffer     (502) staff       (20)     1304 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer     (502) staff       (20)      817 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Components.py
--rw-r--r--   0 buffer     (502) staff       (20)     5901 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Console.py
--rw-r--r--   0 buffer     (502) staff       (20)     1112 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Crypto.py
--rw-r--r--   0 buffer     (502) staff       (20)    54541 2023-03-01 08:10:57.000000 thug-4.9/thug/DOM/DFT.py
--rw-r--r--   0 buffer     (502) staff       (20)     3602 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/External.py
--rw-r--r--   0 buffer     (502) staff       (20)     2776 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer     (502) staff       (20)     9866 2023-03-07 14:57:11.000000 thug-4.9/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer     (502) staff       (20)      932 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer     (502) staff       (20)     3593 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/History.py
--rw-r--r--   0 buffer     (502) staff       (20)     3506 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/JSClass.py
--rw-r--r--   0 buffer     (502) staff       (20)     7824 2023-01-06 16:11:13.000000 thug-4.9/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer     (502) staff       (20)     4502 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer     (502) staff       (20)     5959 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer     (502) staff       (20)      752 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     4661 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/Location.py
--rw-r--r--   0 buffer     (502) staff       (20)    19549 2023-02-27 08:54:28.000000 thug-4.9/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer     (502) staff       (20)      762 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Map.py
--rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/MimeType.py
--rw-r--r--   0 buffer     (502) staff       (20)     5282 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer     (502) staff       (20)    13340 2023-03-07 14:57:11.000000 thug-4.9/thug/DOM/Navigator.py
--rw-r--r--   0 buffer     (502) staff       (20)     4056 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Personality.py
--rw-r--r--   0 buffer     (502) staff       (20)     1233 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Plugin.py
--rw-r--r--   0 buffer     (502) staff       (20)     1471 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Plugins.py
--rw-r--r--   0 buffer     (502) staff       (20)     1069 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer     (502) staff       (20)     6150 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Screen.py
--rw-r--r--   0 buffer     (502) staff       (20)      756 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     1750 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer     (502) staff       (20)     3502 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Storage.py
--rw-r--r--   0 buffer     (502) staff       (20)     3216 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.106836 thug-4.9/thug/DOM/W3C/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.128377 thug-4.9/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer     (502) staff       (20)     2138 2023-01-06 12:37:35.000000 thug-4.9/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer     (502) staff       (20)      265 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1241 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer     (502) staff       (20)     3531 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer     (502) staff       (20)      564 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer     (502) staff       (20)     1910 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer     (502) staff       (20)     5765 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer     (502) staff       (20)     8868 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer     (502) staff       (20)     2412 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer     (502) staff       (20)     1513 2023-01-06 12:31:24.000000 thug-4.9/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer     (502) staff       (20)     9544 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer     (502) staff       (20)      457 2023-01-06 12:38:21.000000 thug-4.9/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer     (502) staff       (20)      501 2023-01-06 12:38:52.000000 thug-4.9/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer     (502) staff       (20)    14464 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer     (502) staff       (20)      569 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer     (502) staff       (20)      474 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer     (502) staff       (20)      485 2023-01-06 12:34:08.000000 thug-4.9/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer     (502) staff       (20)      510 2023-01-06 12:34:27.000000 thug-4.9/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer     (502) staff       (20)      803 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer     (502) staff       (20)     1051 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      337 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer     (502) staff       (20)      274 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer     (502) staff       (20)     1454 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.141584 thug-4.9/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer     (502) staff       (20)      868 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     4120 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer     (502) staff       (20)      525 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer     (502) staff       (20)      272 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer     (502) staff       (20)     9134 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1206 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     2198 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1575 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)      636 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer     (502) staff       (20)      691 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.143620 thug-4.9/thug/DOM/W3C/File/
--rw-r--r--   0 buffer     (502) staff       (20)     2433 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer     (502) staff       (20)     1381 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer     (502) staff       (20)       85 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.195407 thug-4.9/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer     (502) staff       (20)      194 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer     (502) staff       (20)      374 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1922 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      654 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      252 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      331 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1321 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      582 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1281 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)      265 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      263 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer     (502) staff       (20)    15982 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer     (502) staff       (20)      955 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer     (502) staff       (20)      412 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     4141 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      322 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)     1742 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      978 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      289 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      407 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1300 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1302 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1466 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      277 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      373 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      376 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      558 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     4216 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      264 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      667 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      296 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2595 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      343 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      227 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer     (502) staff       (20)      259 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      988 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1636 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      177 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      316 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      262 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      917 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     4711 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2800 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     2091 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1031 2022-12-30 12:26:43.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer     (502) staff       (20)      280 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer     (502) staff       (20)      681 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer     (502) staff       (20)     5132 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      442 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      426 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      436 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer     (502) staff       (20)      806 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.196159 thug-4.9/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.197937 thug-4.9/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer     (502) staff       (20)      425 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.199632 thug-4.9/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer     (502) staff       (20)     4843 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer     (502) staff       (20)     2710 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.201979 thug-4.9/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer     (502) staff       (20)      217 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer     (502) staff       (20)      211 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)       56 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      367 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer     (502) staff       (20)      829 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/WebStore.py
--rw-r--r--   0 buffer     (502) staff       (20)    35015 2023-01-13 08:09:32.000000 thug-4.9/thug/DOM/Window.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)     7624 2022-12-28 14:31:40.000000 thug-4.9/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.202936 thug-4.9/thug/Encoding/
--rw-r--r--   0 buffer     (502) staff       (20)      877 2022-12-28 14:31:40.000000 thug-4.9/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.204637 thug-4.9/thug/Java/
--rw-r--r--   0 buffer     (502) staff       (20)     1114 2022-12-28 14:31:40.000000 thug-4.9/thug/Java/System.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Java/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      763 2022-12-28 14:31:40.000000 thug-4.9/thug/Java/java.py
--rw-r--r--   0 buffer     (502) staff       (20)      771 2022-12-28 14:31:40.000000 thug-4.9/thug/Java/lang.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.208868 thug-4.9/thug/Logging/
--rw-r--r--   0 buffer     (502) staff       (20)     2454 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)     3893 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/Features.py
--rw-r--r--   0 buffer     (502) staff       (20)      920 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer     (502) staff       (20)     5106 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)    14604 2023-01-03 10:16:05.000000 thug-4.9/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.211908 thug-4.9/thug/Logging/modules/
--rw-r--r--   0 buffer     (502) staff       (20)     2565 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer     (502) staff       (20)     1301 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer     (502) staff       (20)    14581 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer     (502) staff       (20)    10438 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer     (502) staff       (20)    16889 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer     (502) staff       (20)       83 2022-12-28 14:31:40.000000 thug-4.9/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.213006 thug-4.9/thug/Magic/
--rw-r--r--   0 buffer     (502) staff       (20)     1593 2022-12-28 14:31:40.000000 thug-4.9/thug/Magic/Magic.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.214324 thug-4.9/thug/OS/
--rw-r--r--   0 buffer     (502) staff       (20)     4912 2022-12-28 14:31:40.000000 thug-4.9/thug/OS/Windows.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/OS/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.216322 thug-4.9/thug/Plugins/
--rw-r--r--   0 buffer     (502) staff       (20)      956 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer     (502) staff       (20)     3401 2023-01-03 10:15:59.000000 thug-4.9/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.216686 thug-4.9/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.217574 thug-4.9/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.218638 thug-4.9/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.224426 thug-4.9/thug/ThugAPI/
--rw-r--r--   0 buffer     (502) staff       (20)    18741 2023-03-07 14:57:11.000000 thug-4.9/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-4.9/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer     (502) staff       (20)    16007 2023-03-07 14:57:11.000000 thug-4.9/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer     (502) staff       (20)     9649 2023-03-07 14:57:11.000000 thug-4.9/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer     (502) staff       (20)     4203 2022-12-28 14:31:40.000000 thug-4.9/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer     (502) staff       (20)     1642 2022-12-28 14:31:40.000000 thug-4.9/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-4.9/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)      317 2022-12-28 14:31:40.000000 thug-4.9/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.226687 thug-4.9/thug/WebTracking/
--rw-r--r--   0 buffer     (502) staff       (20)     3206 2022-12-28 14:31:40.000000 thug-4.9/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer     (502) staff       (20)     1176 2022-12-28 14:31:40.000000 thug-4.9/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer     (502) staff       (20)     1596 2022-12-28 14:31:40.000000 thug-4.9/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer     (502) staff       (20)     2024 2023-03-10 13:51:50.000000 thug-4.9/thug/__init__.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.228680 thug-4.9/thug/conf/
--rw-r--r--   0 buffer     (502) staff       (20)     6148 2022-11-04 15:21:57.000000 thug-4.9/thug/conf/.DS_Store
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.229568 thug-4.9/thug/conf/hooks/
--rw-r--r--   0 buffer     (502) staff       (20)       45 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/hooks/README
--rw-r--r--   0 buffer     (502) staff       (20)      174 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/inspector.json
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.264890 thug-4.9/thug/conf/personalities/
--rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer     (502) staff       (20)      743 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer     (502) staff       (20)      793 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer     (502) staff       (20)      729 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer     (502) staff       (20)      692 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer     (502) staff       (20)      680 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer     (502) staff       (20)      748 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer     (502) staff       (20)      690 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer     (502) staff       (20)      682 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer     (502) staff       (20)      396 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer     (502) staff       (20)     2851 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer     (502) staff       (20)     3826 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer     (502) staff       (20)      915 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer     (502) staff       (20)      579 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer     (502) staff       (20)     3769 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer     (502) staff       (20)     3800 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer     (502) staff       (20)     3820 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer     (502) staff       (20)      678 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer     (502) staff       (20)      674 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer     (502) staff       (20)      564 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer     (502) staff       (20)     2876 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer     (502) staff       (20)     2896 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer     (502) staff       (20)     2871 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer     (502) staff       (20)     2968 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer     (502) staff       (20)      666 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.265629 thug-4.9/thug/conf/plugins/
--rw-r--r--   0 buffer     (502) staff       (20)       47 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/plugins/README
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.275425 thug-4.9/thug/conf/rules/
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.275881 thug-4.9/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.276827 thug-4.9/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.277894 thug-4.9/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.278783 thug-4.9/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.279733 thug-4.9/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.280781 thug-4.9/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      103 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.281677 thug-4.9/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      245 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.282460 thug-4.9/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       97 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.283558 thug-4.9/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.284748 thug-4.9/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.285860 thug-4.9/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.286835 thug-4.9/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.299867 thug-4.9/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)     3005 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer     (502) staff       (20)      418 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer     (502) staff       (20)      641 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer     (502) staff       (20)     1000 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer     (502) staff       (20)      870 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer     (502) staff       (20)      387 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer     (502) staff       (20)      808 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer     (502) staff       (20)      612 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer     (502) staff       (20)      969 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer     (502) staff       (20)      765 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer     (502) staff       (20)      427 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer     (502) staff       (20)      176 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer     (502) staff       (20)     2400 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer     (502) staff       (20)      849 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer     (502) staff       (20)      340 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.300889 thug-4.9/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.301683 thug-4.9/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.302362 thug-4.9/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:18.305957 thug-4.9/thug/conf/scripts/
--rw-r--r--   0 buffer     (502) staff       (20)       69 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/date.js
--rw-r--r--   0 buffer     (502) staff       (20)      197 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer     (502) staff       (20)       87 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer     (502) staff       (20)      753 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer     (502) staff       (20)      205 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/scripts/write.js
--rw-r--r--   0 buffer     (502) staff       (20)      325 2022-12-28 14:31:40.000000 thug-4.9/thug/conf/thug.conf
--rw-r--r--   0 buffer     (502) staff       (20)    17085 2023-03-07 14:57:11.000000 thug-4.9/thug/thug.py
-drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-03-10 14:03:17.869792 thug-4.9/thug.egg-info/
--rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer     (502) staff       (20)    15813 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer     (502) staff       (20)        1 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer     (502) staff       (20)       40 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer     (502) staff       (20)      517 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/requires.txt
--rw-r--r--   0 buffer     (502) staff       (20)        5 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer     (502) staff       (20)        1 2023-03-10 14:03:17.000000 thug-4.9/thug.egg-info/zip-safe
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.075065 thug-5.0/
+-rw-r--r--   0 buffer     (502) staff       (20)    17987 2022-12-28 14:31:40.000000 thug-5.0/LICENSE.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      130 2023-01-03 13:39:45.000000 thug-5.0/MANIFEST.in
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-05-10 07:26:43.074195 thug-5.0/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)     2676 2023-01-17 09:44:55.000000 thug-5.0/README.rst
+-rw-r--r--   0 buffer     (502) staff       (20)     3485 2023-05-05 08:26:35.000000 thug-5.0/pyproject.toml
+-rw-r--r--   0 buffer     (502) staff       (20)      339 2023-05-05 08:26:42.000000 thug-5.0/requirements.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       38 2023-05-10 07:26:43.075251 thug-5.0/setup.cfg
+-rw-r--r--   0 buffer     (502) staff       (20)     1346 2023-01-03 12:33:41.000000 thug-5.0/setup.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.631637 thug-5.0/thug/
+-rw-r--r--   0 buffer     (502) staff       (20)     8196 2022-11-04 15:21:57.000000 thug-5.0/thug/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.645223 thug-5.0/thug/ActiveX/
+-rw-r--r--   0 buffer     (502) staff       (20)     7598 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 buffer     (502) staff       (20)    64018 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/CLSID.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.775296 thug-5.0/thug/ActiveX/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)      400 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1119 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2573 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1482 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1086 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 buffer     (502) staff       (20)      979 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 buffer     (502) staff       (20)      801 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      567 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 buffer     (502) staff       (20)      421 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      600 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      726 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 buffer     (502) staff       (20)      307 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 buffer     (502) staff       (20)      673 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 buffer     (502) staff       (20)      447 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)      625 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 buffer     (502) staff       (20)      404 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1857 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1500 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      825 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3049 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2221 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 buffer     (502) staff       (20)      496 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 buffer     (502) staff       (20)      656 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 buffer     (502) staff       (20)      420 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 buffer     (502) staff       (20)      561 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4119 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      443 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 buffer     (502) staff       (20)      945 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      672 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1964 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)      405 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 buffer     (502) staff       (20)      601 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      535 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4390 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2048 2023-01-13 08:09:32.000000 thug-5.0/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8006 2023-01-06 14:50:41.000000 thug-5.0/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      466 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 buffer     (502) staff       (20)      438 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 buffer     (502) staff       (20)      589 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1259 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 buffer     (502) staff       (20)      616 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3311 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1175 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1057 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1201 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      498 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 buffer     (502) staff       (20)      494 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)      973 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2335 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      348 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)      831 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 buffer     (502) staff       (20)      449 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1116 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1027 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 buffer     (502) staff       (20)      341 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5185 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1527 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 buffer     (502) staff       (20)      361 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 buffer     (502) staff       (20)      394 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 buffer     (502) staff       (20)      273 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 buffer     (502) staff       (20)      921 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1472 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      715 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 buffer     (502) staff       (20)      906 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 buffer     (502) staff       (20)      677 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2436 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 buffer     (502) staff       (20)      516 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1061 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2224 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/SymantecBackupExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4772 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 buffer     (502) staff       (20)      391 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1763 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 buffer     (502) staff       (20)      719 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      699 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 buffer     (502) staff       (20)      796 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 buffer     (502) staff       (20)      132 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1280 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1689 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8980 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 buffer     (502) staff       (20)      213 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 buffer     (502) staff       (20)      645 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1373 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      599 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 buffer     (502) staff       (20)      145 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 buffer     (502) staff       (20)      942 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1026 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1159 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1077 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1244 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1932 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2870 2022-12-28 14:31:40.000000 thug-5.0/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.776249 thug-5.0/thug/Analysis/
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.777902 thug-5.0/thug/Analysis/awis/
+-rw-r--r--   0 buffer     (502) staff       (20)     3224 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.779364 thug-5.0/thug/Analysis/context/
+-rw-r--r--   0 buffer     (502) staff       (20)     1554 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.780805 thug-5.0/thug/Analysis/honeyagent/
+-rw-r--r--   0 buffer     (502) staff       (20)     4000 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.782480 thug-5.0/thug/Analysis/screenshot/
+-rw-r--r--   0 buffer     (502) staff       (20)     1333 2023-03-07 14:57:11.000000 thug-5.0/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.784082 thug-5.0/thug/Analysis/shellcode/
+-rw-r--r--   0 buffer     (502) staff       (20)     8069 2023-01-13 08:09:32.000000 thug-5.0/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.794591 thug-5.0/thug/Classifier/
+-rw-r--r--   0 buffer     (502) staff       (20)     5017 2023-03-28 13:07:55.000000 thug-5.0/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2106 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2159 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2070 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2008 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2243 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2082 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2330 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2014 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Classifier/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.836708 thug-5.0/thug/DOM/
+-rw-r--r--   0 buffer     (502) staff       (20)     2534 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Alexa.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2289 2023-03-28 10:08:11.000000 thug-5.0/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2254 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Chrome.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1304 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/ClipboardData.py
+-rw-r--r--   0 buffer     (502) staff       (20)      817 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Components.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5901 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Console.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1112 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Crypto.py
+-rw-r--r--   0 buffer     (502) staff       (20)    54541 2023-03-01 08:10:57.000000 thug-5.0/thug/DOM/DFT.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3602 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/External.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2776 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9866 2023-03-07 14:57:11.000000 thug-5.0/thug/DOM/HTTPSession.py
+-rw-r--r--   0 buffer     (502) staff       (20)      932 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3593 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/History.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3506 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/JSClass.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7824 2023-01-06 16:11:13.000000 thug-5.0/thug/DOM/JSEngine.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4502 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/JSInspector.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5959 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 buffer     (502) staff       (20)      752 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/LocalStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4661 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/Location.py
+-rw-r--r--   0 buffer     (502) staff       (20)    19549 2023-02-27 08:54:28.000000 thug-5.0/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)      762 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Map.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1197 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/MimeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5282 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/MimeTypes.py
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/MozConnection.py
+-rw-r--r--   0 buffer     (502) staff       (20)    13340 2023-03-07 14:57:11.000000 thug-5.0/thug/DOM/Navigator.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4056 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Personality.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1233 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Plugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1471 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Plugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1069 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 buffer     (502) staff       (20)     6150 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Screen.py
+-rw-r--r--   0 buffer     (502) staff       (20)      756 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/SessionStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1750 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Sidebar.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3502 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Storage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3216 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/UserProfile.py
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/Utils.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.842689 thug-5.0/thug/DOM/W3C/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.880836 thug-5.0/thug/DOM/W3C/Core/
+-rw-r--r--   0 buffer     (502) staff       (20)     2138 2023-01-06 12:37:35.000000 thug-5.0/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1241 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3531 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1910 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5765 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 buffer     (502) staff       (20)     8868 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2412 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1513 2023-01-06 12:31:24.000000 thug-5.0/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9544 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 buffer     (502) staff       (20)      457 2023-01-06 12:38:21.000000 thug-5.0/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 buffer     (502) staff       (20)      501 2023-01-06 12:38:52.000000 thug-5.0/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14464 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 buffer     (502) staff       (20)      569 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      474 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 buffer     (502) staff       (20)      485 2023-01-06 12:34:08.000000 thug-5.0/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 buffer     (502) staff       (20)      510 2023-01-06 12:34:27.000000 thug-5.0/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 buffer     (502) staff       (20)      803 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1051 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      337 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 buffer     (502) staff       (20)      274 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1454 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.893121 thug-5.0/thug/DOM/W3C/Events/
+-rw-r--r--   0 buffer     (502) staff       (20)      868 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4120 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 buffer     (502) staff       (20)      525 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 buffer     (502) staff       (20)      272 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9134 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 buffer     (502) staff       (20)      484 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1206 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2198 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1575 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      636 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 buffer     (502) staff       (20)      691 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.895514 thug-5.0/thug/DOM/W3C/File/
+-rw-r--r--   0 buffer     (502) staff       (20)     2433 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1381 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 buffer     (502) staff       (20)       85 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.959986 thug-5.0/thug/DOM/W3C/HTML/
+-rw-r--r--   0 buffer     (502) staff       (20)      194 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      610 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 buffer     (502) staff       (20)      374 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1922 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      654 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      252 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      331 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1486 2023-04-11 09:54:20.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      582 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1281 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      265 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      263 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)    15982 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 buffer     (502) staff       (20)      955 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 buffer     (502) staff       (20)      412 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4141 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      322 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1742 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      978 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      289 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      407 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      257 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1300 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1302 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1466 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      277 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      291 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      373 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      376 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      558 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4216 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      264 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      667 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      296 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2595 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      343 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      720 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      227 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 buffer     (502) staff       (20)      259 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      378 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      258 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      253 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      988 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1636 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      177 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      316 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      262 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      917 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      445 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4711 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2800 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2091 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1031 2022-12-30 12:26:43.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      247 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)      336 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1105 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 buffer     (502) staff       (20)      280 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 buffer     (502) staff       (20)      681 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5132 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      442 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      426 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      436 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 buffer     (502) staff       (20)      806 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.960541 thug-5.0/thug/DOM/W3C/Style/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.962043 thug-5.0/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 buffer     (502) staff       (20)     1293 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 buffer     (502) staff       (20)      425 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.963473 thug-5.0/thug/DOM/W3C/URL/
+-rw-r--r--   0 buffer     (502) staff       (20)     4843 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2710 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.967081 thug-5.0/thug/DOM/W3C/Views/
+-rw-r--r--   0 buffer     (502) staff       (20)      217 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 buffer     (502) staff       (20)      211 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)       56 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      367 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 buffer     (502) staff       (20)      829 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/WebStore.py
+-rw-r--r--   0 buffer     (502) staff       (20)    35015 2023-01-13 08:09:32.000000 thug-5.0/thug/DOM/Window.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     7624 2022-12-28 14:31:40.000000 thug-5.0/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.968553 thug-5.0/thug/Encoding/
+-rw-r--r--   0 buffer     (502) staff       (20)      877 2022-12-28 14:31:40.000000 thug-5.0/thug/Encoding/Encoding.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Encoding/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.971604 thug-5.0/thug/Java/
+-rw-r--r--   0 buffer     (502) staff       (20)     1114 2022-12-28 14:31:40.000000 thug-5.0/thug/Java/System.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Java/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      763 2022-12-28 14:31:40.000000 thug-5.0/thug/Java/java.py
+-rw-r--r--   0 buffer     (502) staff       (20)      771 2022-12-28 14:31:40.000000 thug-5.0/thug/Java/lang.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.978155 thug-5.0/thug/Logging/
+-rw-r--r--   0 buffer     (502) staff       (20)     2454 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/BaseLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3893 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/Features.py
+-rw-r--r--   0 buffer     (502) staff       (20)      920 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/LoggingModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     5106 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/SampleLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14604 2023-01-03 10:16:05.000000 thug-5.0/thug/Logging/ThugLogging.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.983209 thug-5.0/thug/Logging/modules/
+-rw-r--r--   0 buffer     (502) staff       (20)     2565 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1301 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 buffer     (502) staff       (20)    14581 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/JSON.py
+-rw-r--r--   0 buffer     (502) staff       (20)    10438 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16889 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 buffer     (502) staff       (20)       83 2022-12-28 14:31:40.000000 thug-5.0/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.984953 thug-5.0/thug/Magic/
+-rw-r--r--   0 buffer     (502) staff       (20)     1593 2022-12-28 14:31:40.000000 thug-5.0/thug/Magic/Magic.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Magic/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.986275 thug-5.0/thug/OS/
+-rw-r--r--   0 buffer     (502) staff       (20)     4912 2022-12-28 14:31:40.000000 thug-5.0/thug/OS/Windows.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/OS/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.988730 thug-5.0/thug/Plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)      956 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/IPlugin.py
+-rw-r--r--   0 buffer     (502) staff       (20)     3401 2023-01-03 10:15:59.000000 thug-5.0/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.989453 thug-5.0/thug/Plugins/plugins/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.991051 thug-5.0/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.991945 thug-5.0/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 buffer     (502) staff       (20)      878 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.996874 thug-5.0/thug/ThugAPI/
+-rw-r--r--   0 buffer     (502) staff       (20)    18741 2023-03-07 14:57:11.000000 thug-5.0/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)      787 2022-12-28 14:31:40.000000 thug-5.0/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 buffer     (502) staff       (20)    16007 2023-03-07 14:57:11.000000 thug-5.0/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 buffer     (502) staff       (20)     9649 2023-03-07 14:57:11.000000 thug-5.0/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 buffer     (502) staff       (20)     4203 2022-12-28 14:31:40.000000 thug-5.0/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1642 2022-12-28 14:31:40.000000 thug-5.0/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.0/thug/ThugAPI/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)      317 2022-12-28 14:31:40.000000 thug-5.0/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.999421 thug-5.0/thug/WebTracking/
+-rw-r--r--   0 buffer     (502) staff       (20)     3206 2022-12-28 14:31:40.000000 thug-5.0/thug/WebTracking/Cookies.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1176 2022-12-28 14:31:40.000000 thug-5.0/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 buffer     (502) staff       (20)     1596 2022-12-28 14:31:40.000000 thug-5.0/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/WebTracking/__init__.py
+-rw-r--r--   0 buffer     (502) staff       (20)     2024 2023-05-10 07:10:35.000000 thug-5.0/thug/__init__.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.001098 thug-5.0/thug/conf/
+-rw-r--r--   0 buffer     (502) staff       (20)     6148 2022-11-04 15:21:57.000000 thug-5.0/thug/conf/.DS_Store
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.001922 thug-5.0/thug/conf/hooks/
+-rw-r--r--   0 buffer     (502) staff       (20)       45 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/hooks/README
+-rw-r--r--   0 buffer     (502) staff       (20)      174 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/inspector.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.040554 thug-5.0/thug/conf/personalities/
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      747 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 buffer     (502) staff       (20)      743 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 buffer     (502) staff       (20)      793 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 buffer     (502) staff       (20)      739 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      737 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 buffer     (502) staff       (20)      729 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 buffer     (502) staff       (20)      692 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 buffer     (502) staff       (20)      688 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 buffer     (502) staff       (20)      680 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 buffer     (502) staff       (20)      648 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 buffer     (502) staff       (20)      652 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      524 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      748 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 buffer     (502) staff       (20)      690 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 buffer     (502) staff       (20)      679 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      682 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 buffer     (502) staff       (20)      396 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 buffer     (502) staff       (20)     2851 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 buffer     (502) staff       (20)     3826 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 buffer     (502) staff       (20)      782 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)      915 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 buffer     (502) staff       (20)      686 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 buffer     (502) staff       (20)      579 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3769 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3800 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)     3820 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 buffer     (502) staff       (20)      678 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 buffer     (502) staff       (20)      674 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 buffer     (502) staff       (20)      564 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2876 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2896 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2871 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 buffer     (502) staff       (20)     2968 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 buffer     (502) staff       (20)      666 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.041109 thug-5.0/thug/conf/plugins/
+-rw-r--r--   0 buffer     (502) staff       (20)       47 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/plugins/README
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.046771 thug-5.0/thug/conf/rules/
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.047005 thug-5.0/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.047446 thug-5.0/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.047936 thug-5.0/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.048552 thug-5.0/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.049273 thug-5.0/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      115 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.049757 thug-5.0/thug/conf/rules/imagefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      103 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.050251 thug-5.0/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      245 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.050807 thug-5.0/thug/conf/rules/jsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       97 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.051334 thug-5.0/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      117 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.051917 thug-5.0/thug/conf/rules/samplefilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      105 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.052438 thug-5.0/thug/conf/rules/textclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      113 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.052913 thug-5.0/thug/conf/rules/textfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)      101 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/textfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.064909 thug-5.0/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)     3005 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      418 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      766 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      641 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     1000 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      870 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      387 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      808 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      612 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      969 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      765 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      427 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      176 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      478 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 buffer     (502) staff       (20)     2400 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      849 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 buffer     (502) staff       (20)      340 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.065736 thug-5.0/thug/conf/rules/urlfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.066614 thug-5.0/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 buffer     (502) staff       (20)      111 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.067437 thug-5.0/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 buffer     (502) staff       (20)       99 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 buffer     (502) staff       (20)        0 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:43.072974 thug-5.0/thug/conf/scripts/
+-rw-r--r--   0 buffer     (502) staff       (20)       69 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/date.js
+-rw-r--r--   0 buffer     (502) staff       (20)      197 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/eval.js
+-rw-r--r--   0 buffer     (502) staff       (20)       87 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/message-event.js
+-rw-r--r--   0 buffer     (502) staff       (20)      204 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/storage.js
+-rw-r--r--   0 buffer     (502) staff       (20)      753 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/thug.js
+-rw-r--r--   0 buffer     (502) staff       (20)      205 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/scripts/write.js
+-rw-r--r--   0 buffer     (502) staff       (20)      325 2022-12-28 14:31:40.000000 thug-5.0/thug/conf/thug.conf
+-rw-r--r--   0 buffer     (502) staff       (20)    17085 2023-03-07 14:57:11.000000 thug-5.0/thug/thug.py
+drwxr-xr-x   0 buffer     (502) staff       (20)        0 2023-05-10 07:26:42.640377 thug-5.0/thug.egg-info/
+-rw-r--r--   0 buffer     (502) staff       (20)     3948 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer     (502) staff       (20)    15813 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer     (502) staff       (20)       40 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer     (502) staff       (20)      507 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        5 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer     (502) staff       (20)        1 2023-05-10 07:26:42.000000 thug-5.0/thug.egg-info/zip-safe
```

### Comparing `thug-4.9/LICENSE.txt` & `thug-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-4.9/PKG-INFO` & `thug-5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 4.9
+Version: 5.0
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
```

### Comparing `thug-4.9/README.rst` & `thug-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `thug-4.9/pyproject.toml` & `thug-5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -33,46 +33,45 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
 ]
 dependencies = [
     "appdirs==1.4.4",
-    "beautifulsoup4==4.11.2",
+    "beautifulsoup4==4.12.2",
     "charset-normalizer==3.1.0",
     "cssutils==2.6.0",
     "html5lib==1.1",
     "lxml==4.9.2",
-    "networkx==3.0",
+    "networkx==3.1",
     "pefile==2023.2.7",
     "promise==2.3",
     "pylibemu==0.8",
     "pymongo==4.3.3",
     "pysocks==1.7.1",
     "python-magic==0.4.27",
     "rarfile==4.0",
-    "requests==2.28.2",
+    "requests==2.30.0",
     "requests-futures==1.0.0",
     "setuptools>=65.5.1",
     "ssdeep==3.4",
-    "yara-python==4.2.3",
-    "zope.interface==5.5.2",
+    "yara-python==4.3.1",
+    "zope.interface==6.0",
 ]
 keywords = [
     "honeyclient",
     "low-interaction",
     "client-honeypot",
     "security-tools",
 ]
 
 [project.optional-dependencies]
 test = [
-    "codecov",
     "elasticmock",
-    "elasticsearch==7.17.8",
+    "elasticsearch==7.17.9",
     "imgkit==1.1.0",
     "mock",
     "mongomock",
     "pre-commit",
     "pygraphviz",
     "pytesseract",
     "pytest",
```

### Comparing `thug-4.9/setup.py` & `thug-5.0/setup.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/.DS_Store` & `thug-5.0/thug/.DS_Store`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/ActiveX.py` & `thug-5.0/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/CLSID.py` & `thug-5.0/thug/ActiveX/CLSID.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AcroPDF.py` & `thug-5.0/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AdodbRecordset.py` & `thug-5.0/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AdodbStream.py` & `thug-5.0/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AnswerWorks.py` & `thug-5.0/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AolAmpX.py` & `thug-5.0/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/AolICQ.py` & `thug-5.0/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/BaiduBar.py` & `thug-5.0/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/BitDefender.py` & `thug-5.0/thug/ActiveX/modules/BitDefender.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/CGAgent.py` & `thug-5.0/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/Comodo.py` & `thug-5.0/thug/ActiveX/modules/Comodo.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-5.0/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/DPClient.py` & `thug-5.0/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/DirectShow.py` & `thug-5.0/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/Domino.py` & `thug-5.0/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/EnjoySAP.py` & `thug-5.0/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-5.0/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/File.py` & `thug-5.0/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/Folder.py` & `thug-5.0/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-5.0/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/GomWeb.py` & `thug-5.0/thug/ActiveX/modules/GomWeb.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/HPInfo.py` & `thug-5.0/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/IMWebControl.py` & `thug-5.0/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/InternetCleverSuite.py` & `thug-5.0/thug/ActiveX/modules/InternetCleverSuite.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-5.0/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-5.0/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MSRICHTXT.py` & `thug-5.0/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MSVFP.py` & `thug-5.0/thug/ActiveX/modules/MSVFP.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MSXML2DOMDocument.py` & `thug-5.0/thug/ActiveX/modules/MSXML2DOMDocument.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-5.0/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-5.0/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-5.0/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-5.0/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/NamoInstaller.py` & `thug-5.0/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/NeoTracePro.py` & `thug-5.0/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-5.0/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/OfficeOCX.py` & `thug-5.0/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-5.0/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/PPlayer.py` & `thug-5.0/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/RDSDataSpace.py` & `thug-5.0/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/RealPlayer.py` & `thug-5.0/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/RegistryPro.py` & `thug-5.0/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-5.0/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-5.0/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-5.0/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/ShellApplication.py` & `thug-5.0/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SinaDLoader.py` & `thug-5.0/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SnapshotViewer.py` & `thug-5.0/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-5.0/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/Spreadsheet.py` & `thug-5.0/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/StormConfig.py` & `thug-5.0/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/StormMps.py` & `thug-5.0/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/StreamAudioChainCast.py` & `thug-5.0/thug/ActiveX/modules/StreamAudioChainCast.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SymantecAppStream.py` & `thug-5.0/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-5.0/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/TextStream.py` & `thug-5.0/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/Toshiba.py` & `thug-5.0/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/UniversalUpload.py` & `thug-5.0/thug/ActiveX/modules/UniversalUpload.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/VLC.py` & `thug-5.0/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-5.0/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/VsaIDEDTE.py` & `thug-5.0/thug/ActiveX/modules/VsaIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/VsmIDEDTE.py` & `thug-5.0/thug/ActiveX/modules/VsmIDEDTE.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-5.0/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WScriptExec.py` & `thug-5.0/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WScriptNetwork.py` & `thug-5.0/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WScriptShell.py` & `thug-5.0/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-5.0/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-5.0/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/WinZip.py` & `thug-5.0/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-5.0/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/XUpload.py` & `thug-5.0/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/YahooJukebox.py` & `thug-5.0/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/YahooMessengerCyft.py` & `thug-5.0/thug/ActiveX/modules/YahooMessengerCyft.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-5.0/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-5.0/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-5.0/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ActiveX/modules/__init__.py` & `thug-5.0/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Analysis/awis/AWIS.py` & `thug-5.0/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Analysis/context/ContextAnalyzer.py` & `thug-5.0/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-5.0/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Analysis/screenshot/Screenshot.py` & `thug-5.0/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Analysis/shellcode/Shellcode.py` & `thug-5.0/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/BaseClassifier.py` & `thug-5.0/thug/Classifier/BaseClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 
     def handle_match_etags(self, match):
         etags = match.meta.get('etags', None)
         if etags is None:
             return
 
         _etags = [t.strip() for t in etags.split(',')]
+
         for s in match.strings:
-            if s[1] not in _etags:
+            if s.identifier not in _etags:
                 continue
 
-            tag = s[2].decode() if isinstance(s[2], bytes) else s[2]
-            if tag not in match.tags:
-                match.tags.append(tag)
+            for instance in s.instances:
+                data = instance.matched_data
+                tag  = data.decode() if isinstance(data, bytes) else data
+
+                if tag not in match.tags:
+                    match.tags.append(tag)
```

### Comparing `thug-4.9/thug/Classifier/CookieClassifier.py` & `thug-5.0/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/HTMLClassifier.py` & `thug-5.0/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/ImageClassifier.py` & `thug-5.0/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/JSClassifier.py` & `thug-5.0/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/SampleClassifier.py` & `thug-5.0/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/TextClassifier.py` & `thug-5.0/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/URLClassifier.py` & `thug-5.0/thug/Classifier/URLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Classifier/VBSClassifier.py` & `thug-5.0/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Alexa.py` & `thug-5.0/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/AsyncPrefetcher.py` & `thug-5.0/thug/DOM/AsyncPrefetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA  02111-1307  USA
 
 import logging
 
-from urllib.parse import urlparse
-
 from requests_futures.sessions import FuturesSession
 
 log = logging.getLogger("Thug")
 
 
 class AsyncPrefetcher:
     def __init__(self, window = None):
```

### Comparing `thug-4.9/thug/DOM/CCInterpreter.py` & `thug-5.0/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Chrome.py` & `thug-5.0/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/ClipboardData.py` & `thug-5.0/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Components.py` & `thug-5.0/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Console.py` & `thug-5.0/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Crypto.py` & `thug-5.0/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/DFT.py` & `thug-5.0/thug/DOM/DFT.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/External.py` & `thug-5.0/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/HTMLInspector.py` & `thug-5.0/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/HTTPSession.py` & `thug-5.0/thug/DOM/HTTPSession.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/HTTPSessionException.py` & `thug-5.0/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/History.py` & `thug-5.0/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/JSClass.py` & `thug-5.0/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/JSEngine.py` & `thug-5.0/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/JSInspector.py` & `thug-5.0/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/JScriptEncode.py` & `thug-5.0/thug/DOM/JScriptEncode.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/LocalStorage.py` & `thug-5.0/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Location.py` & `thug-5.0/thug/DOM/Location.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/MIMEHandler.py` & `thug-5.0/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Map.py` & `thug-5.0/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/MimeType.py` & `thug-5.0/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/MimeTypes.py` & `thug-5.0/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/MozConnection.py` & `thug-5.0/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Navigator.py` & `thug-5.0/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Personality.py` & `thug-5.0/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Plugin.py` & `thug-5.0/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Plugins.py` & `thug-5.0/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/SchemeHandler.py` & `thug-5.0/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Screen.py` & `thug-5.0/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/SessionStorage.py` & `thug-5.0/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Sidebar.py` & `thug-5.0/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Storage.py` & `thug-5.0/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/UserProfile.py` & `thug-5.0/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Utils.py` & `thug-5.0/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Attr.py` & `thug-5.0/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/CharacterData.py` & `thug-5.0/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/ClassList.py` & `thug-5.0/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Comment.py` & `thug-5.0/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/DOMException.py` & `thug-5.0/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-5.0/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Document.py` & `thug-5.0/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-5.0/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/DocumentType.py` & `thug-5.0/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Element.py` & `thug-5.0/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-5.0/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Node.py` & `thug-5.0/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/NodeList.py` & `thug-5.0/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/Text.py` & `thug-5.0/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Core/__init__.py` & `thug-5.0/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/DOMTokenList.py` & `thug-5.0/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-5.0/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/Event.py` & `thug-5.0/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/EventException.py` & `thug-5.0/thug/DOM/W3C/Events/EventException.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/EventTarget.py` & `thug-5.0/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/MessageEvent.py` & `thug-5.0/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/MouseEvent.py` & `thug-5.0/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/MutationEvent.py` & `thug-5.0/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/StorageEvent.py` & `thug-5.0/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/UIEvent.py` & `thug-5.0/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Events/__init__.py` & `thug-5.0/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/File/Blob.py` & `thug-5.0/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/File/File.py` & `thug-5.0/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/Dataset.py` & `thug-5.0/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     def __str__(self):
         return "[object HTMLBodyElement]"
 
     def getInnerHTML(self):
         html = io.StringIO()
 
         for tag in self.tag.contents:
-            html.write(str(tag))
+            try:
+                html.write(str(tag))
+            except Exception as e: # pylint:disable=broad-except
+                log.warning("[HTMLBodyElement] innerHTML warning: %s", str(e))
 
         return html.getvalue()
 
     def setInnerHTML(self, html):
         log.HTMLClassifier.classify(log.ThugLogging.url if log.ThugOpts.local else log.last_url, html)
 
         self.tag.clear()
```

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-5.0/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-5.0/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-5.0/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/__init__.py` & `thug-5.0/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/HTML/text_property.py` & `thug-5.0/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-5.0/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/URL/URL.py` & `thug-5.0/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-5.0/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/WebStore.py` & `thug-5.0/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/Window.py` & `thug-5.0/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/DOM/w3c_bindings.py` & `thug-5.0/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Encoding/Encoding.py` & `thug-5.0/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Java/System.py` & `thug-5.0/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Java/java.py` & `thug-5.0/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Java/lang.py` & `thug-5.0/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/BaseLogging.py` & `thug-5.0/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/Features.py` & `thug-5.0/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/LoggingModules.py` & `thug-5.0/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/SampleLogging.py` & `thug-5.0/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/ThugLogging.py` & `thug-5.0/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/modules/ElasticSearch.py` & `thug-5.0/thug/Logging/modules/ElasticSearch.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/modules/ExploitGraph.py` & `thug-5.0/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/modules/JSON.py` & `thug-5.0/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/modules/Mapper.py` & `thug-5.0/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Logging/modules/MongoDB.py` & `thug-5.0/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Magic/Magic.py` & `thug-5.0/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/OS/Windows.py` & `thug-5.0/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Plugins/IPlugin.py` & `thug-5.0/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Plugins/ThugPlugins.py` & `thug-5.0/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-5.0/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-5.0/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/IThugAPI.py` & `thug-5.0/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/OpaqueFilter.py` & `thug-5.0/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/ThugAPI.py` & `thug-5.0/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/ThugOpts.py` & `thug-5.0/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/ThugVulnModules.py` & `thug-5.0/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/ThugAPI/Watchdog.py` & `thug-5.0/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/WebTracking/Cookies.py` & `thug-5.0/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/WebTracking/WebStorage.py` & `thug-5.0/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/WebTracking/WebTracking.py` & `thug-5.0/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/__init__.py` & `thug-5.0/thug/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import appdirs
 
-__version__            = "4.9"
+__version__            = "5.0"
 __jsengine__           = ""
 __jsengine_version__   = ""
 
 __global_configuration_path__ = "/etc/thug"
 if os.path.exists(__global_configuration_path__):
     __configuration_path__ = __global_configuration_path__
 else:
```

### Comparing `thug-4.9/thug/conf/.DS_Store` & `thug-5.0/thug/conf/.DS_Store`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/galaxy2chrome18.json` & `thug-5.0/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/galaxy2chrome25.json` & `thug-5.0/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/galaxy2chrome29.json` & `thug-5.0/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome33.json` & `thug-5.0/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome35.json` & `thug-5.0/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome37.json` & `thug-5.0/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome38.json` & `thug-5.0/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome39.json` & `thug-5.0/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome45.json` & `thug-5.0/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome46.json` & `thug-5.0/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadchrome47.json` & `thug-5.0/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadsafari7.json` & `thug-5.0/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadsafari8.json` & `thug-5.0/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/ipadsafari9.json` & `thug-5.0/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxchrome26.json` & `thug-5.0/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxchrome30.json` & `thug-5.0/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxchrome44.json` & `thug-5.0/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxchrome54.json` & `thug-5.0/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxchrome98.json` & `thug-5.0/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxfirefox19.json` & `thug-5.0/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/linuxfirefox40.json` & `thug-5.0/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/nexuschrome18.json` & `thug-5.0/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/osx10chrome19.json` & `thug-5.0/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/osx10chrome80.json` & `thug-5.0/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/osx10chrome97.json` & `thug-5.0/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/osx10safari5.json` & `thug-5.0/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/osx11safari14.json` & `thug-5.0/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win10edge20.json.review` & `thug-5.0/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win10ie110.json` & `thug-5.0/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win2kie60.json` & `thug-5.0/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win2kie80.json` & `thug-5.0/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7chrome20.json` & `thug-5.0/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7chrome40.json` & `thug-5.0/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7chrome45.json` & `thug-5.0/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7chrome49.json` & `thug-5.0/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7firefox3.json` & `thug-5.0/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7ie100.json` & `thug-5.0/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7ie80.json` & `thug-5.0/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7ie90.json` & `thug-5.0/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/win7safari5.json` & `thug-5.0/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpchrome20.json` & `thug-5.0/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpfirefox12.json` & `thug-5.0/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpie60.json` & `thug-5.0/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpie61.json` & `thug-5.0/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpie70.json` & `thug-5.0/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpie80.json` & `thug-5.0/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/personalities/winxpsafari5.json` & `thug-5.0/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-5.0/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-5.0/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-5.0/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-5.0/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-5.0/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-5.0/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-5.0/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/popads.yar` & `thug-5.0/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/redkit.yar` & `thug-5.0/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/styx.yar` & `thug-5.0/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-5.0/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/conf/scripts/thug.js` & `thug-5.0/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug/thug.py` & `thug-5.0/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-4.9/thug.egg-info/PKG-INFO` & `thug-5.0/thug.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 4.9
+Version: 5.0
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
```

### Comparing `thug-4.9/thug.egg-info/SOURCES.txt` & `thug-5.0/thug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

