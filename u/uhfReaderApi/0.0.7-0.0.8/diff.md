# Comparing `tmp/uhfReaderApi-0.0.7.tar.gz` & `tmp/uhfReaderApi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\uhfReaderApi-0.0.7.tar", last modified: Wed May 10 08:12:35 2023, max compression
+gzip compressed data, was "dist\uhfReaderApi-0.0.8.tar", last modified: Wed May 10 09:01:41 2023, max compression
```

## Comparing `uhfReaderApi-0.0.7.tar` & `uhfReaderApi-0.0.8.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/
--rw-rw-rw-   0        0        0      300 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-05-10 08:12:10.000000 uhfReaderApi-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhf/
--rw-rw-rw-   0        0        0     3144 2022-08-18 10:16:17.000000 uhfReaderApi-0.0.7/uhf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhf/reader/
--rw-rw-rw-   0        0        0    17157 2022-08-05 03:05:36.000000 uhfReaderApi-0.0.7/uhf/reader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhf/reader/communication/
--rw-rw-rw-   0        0        0      422 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.7/uhf/reader/communication/__init__.py
--rw-rw-rw-   0        0        0    10958 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.7/uhf/reader/communication/gclient.py
--rw-rw-rw-   0        0        0     2186 2020-08-17 07:43:04.000000 uhfReaderApi-0.0.7/uhf/reader/communication/gserver.py
--rw-rw-rw-   0        0        0     2270 2022-08-18 09:28:23.000000 uhfReaderApi-0.0.7/uhf/reader/communication/hid.py
--rw-rw-rw-   0        0        0     4016 2021-04-22 07:59:15.000000 uhfReaderApi-0.0.7/uhf/reader/communication/interface.py
--rw-rw-rw-   0        0        0     2609 2020-12-16 02:27:13.000000 uhfReaderApi-0.0.7/uhf/reader/communication/serial_client.py
--rw-rw-rw-   0        0        0     2735 2020-12-30 08:51:55.000000 uhfReaderApi-0.0.7/uhf/reader/communication/tcp_client.py
--rw-rw-rw-   0        0        0     1547 2020-08-17 07:47:02.000000 uhfReaderApi-0.0.7/uhf/reader/communication/tcp_server.py
--rw-rw-rw-   0        0        0     3892 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.7/uhf/reader/communication/usb_hid.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/
--rw-rw-rw-   0        0        0    10103 2022-08-18 09:19:07.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/__init__.py
--rw-rw-rw-   0        0        0     1609 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/action_param_fail.py
--rw-rw-rw-   0        0        0     1612 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/action_param_success.py
--rw-rw-rw-   0        0        0      703 2022-08-18 09:19:07.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_all_gpiState.py
--rw-rw-rw-   0        0        0      618 2020-12-02 06:22:16.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_clearCacheData.py
--rw-rw-rw-   0        0        0      585 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_del_whiteList.py
--rw-rw-rw-   0        0        0      795 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_baseVersion.py
--rw-rw-rw-   0        0        0      681 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_breakpointResume.py
--rw-rw-rw-   0        0        0      634 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_cacheTagData.py
--rw-rw-rw-   0        0        0     2066 2020-08-18 11:37:45.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_easAlarm.py
--rw-rw-rw-   0        0        0     1876 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_ethernetIp.py
--rw-rw-rw-   0        0        0      773 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_gpiState.py
--rw-rw-rw-   0        0        0     1650 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_gpiTrigger.py
--rw-rw-rw-   0        0        0     1357 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_httpParam.py
--rw-rw-rw-   0        0        0     2324 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerInfo.py
--rw-rw-rw-   0        0        0     1030 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerMac.py
--rw-rw-rw-   0        0        0      855 2020-08-18 09:53:50.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerTime.py
--rw-rw-rw-   0        0        0      755 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_rs485.py
--rw-rw-rw-   0        0        0      692 2020-08-18 09:36:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_serialParam.py
--rw-rw-rw-   0        0        0     1311 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_tcpMode.py
--rw-rw-rw-   0        0        0     1024 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_udpParam.py
--rw-rw-rw-   0        0        0     1028 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteList.py
--rw-rw-rw-   0        0        0      793 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteListAction.py
--rw-rw-rw-   0        0        0      781 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteListSwitch.py
--rw-rw-rw-   0        0        0      899 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wiegand.py
--rw-rw-rw-   0        0        0      789 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiConnectStatus.py
--rw-rw-rw-   0        0        0     1044 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiHotspotSearch.py
--rw-rw-rw-   0        0        0     1932 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiIp.py
--rw-rw-rw-   0        0        0      680 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiSwitch.py
--rw-rw-rw-   0        0        0      893 2020-12-02 06:09:18.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_gpiOver.py
--rw-rw-rw-   0        0        0      892 2020-12-02 06:10:20.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_gpiStart.py
--rw-rw-rw-   0        0        0      718 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_heartbeat.py
--rw-rw-rw-   0        0        0     1182 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_import_whiteList.py
--rw-rw-rw-   0        0        0      368 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_reset.py
--rw-rw-rw-   0        0        0      701 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_restoreDefault.py
--rw-rw-rw-   0        0        0      863 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_beep.py
--rw-rw-rw-   0        0        0      786 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_beepOnOff.py
--rw-rw-rw-   0        0        0      784 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_breakpointResume.py
--rw-rw-rw-   0        0        0     2045 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_easAlarm.py
--rw-rw-rw-   0        0        0     2145 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_ethernetIp.py
--rw-rw-rw-   0        0        0     1819 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_gpiTrigger.py
--rw-rw-rw-   0        0        0     5685 2022-08-18 08:40:29.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_gpo.py
--rw-rw-rw-   0        0        0     1390 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_httpParam.py
--rw-rw-rw-   0        0        0      872 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_readerTime.py
--rw-rw-rw-   0        0        0      947 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_rs485.py
--rw-rw-rw-   0        0        0      833 2020-10-26 03:24:47.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_serialParam.py
--rw-rw-rw-   0        0        0     1525 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_tpcMode.py
--rw-rw-rw-   0        0        0     1398 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_udpParam.py
--rw-rw-rw-   0        0        0      896 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_whiteListAction.py
--rw-rw-rw-   0        0        0      881 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_whiteListSwitch.py
--rw-rw-rw-   0        0        0     1197 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wiegand.py
--rw-rw-rw-   0        0        0     1545 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiHotspot.py
--rw-rw-rw-   0        0        0     2313 2020-08-24 07:51:37.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiIp.py
--rw-rw-rw-   0        0        0      787 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiSwitch.py
--rw-rw-rw-   0        0        0      772 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_tagDataReply.py
--rw-rw-rw-   0        0        0      540 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/app_wifiHotspotSearch.py
--rw-rw-rw-   0        0        0     1458 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyEpc.py
--rw-rw-rw-   0        0        0     1775 2022-01-14 02:32:38.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyGJb.py
--rw-rw-rw-   0        0        0     1773 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyGb.py
--rw-rw-rw-   0        0        0      807 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_antennaHub.py
--rw-rw-rw-   0        0        0      768 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_autoDormancy.py
--rw-rw-rw-   0        0        0      958 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_baseband.py
--rw-rw-rw-   0        0        0     1277 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_capabilities.py
--rw-rw-rw-   0        0        0      694 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_freRange.py
--rw-rw-rw-   0        0        0      866 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_frequency.py
--rw-rw-rw-   0        0        0     1362 2020-09-18 07:26:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_gb_baseband.py
--rw-rw-rw-   0        0        0      801 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_power.py
--rw-rw-rw-   0        0        0     1000 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_residenceTime.py
--rw-rw-rw-   0        0        0      771 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_tagLog.py
--rw-rw-rw-   0        0        0     1524 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventory6b.py
--rw-rw-rw-   0        0        0     3723 2020-08-17 10:14:57.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryEpc.py
--rw-rw-rw-   0        0        0     2154 2022-01-14 02:21:40.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryGJb.py
--rw-rw-rw-   0        0        0     2151 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryGb.py
--rw-rw-rw-   0        0        0      964 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventory_Hybrid.py
--rw-rw-rw-   0        0        0     1284 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_lock6b.py
--rw-rw-rw-   0        0        0     1296 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_lock6bGet.py
--rw-rw-rw-   0        0        0     1759 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockEpc.py
--rw-rw-rw-   0        0        0     2020 2022-01-14 02:32:38.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockGJb.py
--rw-rw-rw-   0        0        0     2018 2022-01-14 02:11:54.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockGb.py
--rw-rw-rw-   0        0        0     1715 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_safe_attestation.py
--rw-rw-rw-   0        0        0     1015 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_antennaHub.py
--rw-rw-rw-   0        0        0     1024 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_autoDormancy.py
--rw-rw-rw-   0        0        0     1593 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_baseband.py
--rw-rw-rw-   0        0        0      883 2020-08-17 09:53:57.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_freRange.py
--rw-rw-rw-   0        0        0     1417 2020-08-17 09:53:58.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_frequency.py
--rw-rw-rw-   0        0        0     2119 2020-09-18 07:20:38.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_gb_baseband.py
--rw-rw-rw-   0        0        0     1248 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_power.py
--rw-rw-rw-   0        0        0     1197 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_residenceTime.py
--rw-rw-rw-   0        0        0     1112 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_tagLog.py
--rw-rw-rw-   0        0        0      499 2020-12-02 06:22:16.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_stop.py
--rw-rw-rw-   0        0        0     1618 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_super_rw.py
--rw-rw-rw-   0        0        0     1577 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_write6b.py
--rw-rw-rw-   0        0        0     2437 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeEpc.py
--rw-rw-rw-   0        0        0     2719 2022-01-14 02:28:29.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeGJb.py
--rw-rw-rw-   0        0        0     2885 2022-01-14 02:29:37.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeGb.py
--rw-rw-rw-   0        0        0     2424 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeMonzaQt.py
--rw-rw-rw-   0        0        0     6030 2022-08-18 09:02:45.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/enumg.py
--rw-rw-rw-   0        0        0     1428 2020-08-18 01:36:44.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_6b_info.py
--rw-rw-rw-   0        0        0      683 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_6b_over.py
--rw-rw-rw-   0        0        0     3977 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_epc_info.py
--rw-rw-rw-   0        0        0      687 2020-08-17 09:57:46.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_epc_over.py
--rw-rw-rw-   0        0        0     1831 2020-08-18 01:36:44.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_gb_info.py
--rw-rw-rw-   0        0        0      683 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_gb_over.py
--rw-rw-rw-   0        0        0     5415 2022-01-14 02:07:14.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/message.py
--rw-rw-rw-   0        0        0      693 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_6b_readUserData.py
--rw-rw-rw-   0        0        0      700 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_fastId.py
--rw-rw-rw-   0        0        0     1034 2020-08-03 03:44:41.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_filter.py
--rw-rw-rw-   0        0        0      693 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readEpc.py
--rw-rw-rw-   0        0        0      698 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readReserved.py
--rw-rw-rw-   0        0        0      685 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readTid.py
--rw-rw-rw-   0        0        0      698 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readUserData.py
--rw-rw-rw-   0        0        0      847 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_gb_readUserData.py
--rw-rw-rw-   0        0        0      772 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/param_safe_attestation.py
--rw-rw-rw-   0        0        0      112 2020-06-04 11:33:17.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/parameter.py
--rw-rw-rw-   0        0        0     1034 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_carrierWave.py
--rw-rw-rw-   0        0        0      569 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_dc_autobias.py
--rw-rw-rw-   0        0        0      881 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_dcbias.py
--rw-rw-rw-   0        0        0      665 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_dcbias_get.py
--rw-rw-rw-   0        0        0      628 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_encryptionParam_get.py
--rw-rw-rw-   0        0        0      835 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_encryptionParam_set.py
--rw-rw-rw-   0        0        0     1255 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_env_rssiAutoDetection.py
--rw-rw-rw-   0        0        0     1349 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_env_rssiDetection.py
--rw-rw-rw-   0        0        0      708 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_get_rssiCalibration.py
--rw-rw-rw-   0        0        0     1102 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_power_calibration.py
--rw-rw-rw-   0        0        0     1065 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_power_calibrationGet.py
--rw-rw-rw-   0        0        0     1366 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_r2000_readWrite.py
--rw-rw-rw-   0        0        0     1237 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_r2000_receivingGain.py
--rw-rw-rw-   0        0        0      948 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_serialno_set.py
--rw-rw-rw-   0        0        0      823 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_set_rssiCalibration.py
--rw-rw-rw-   0        0        0      763 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_vswr_check.py
--rw-rw-rw-   0        0        0     1220 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_workMode_get.py
--rw-rw-rw-   0        0        0     1551 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/test_workMode_set.py
--rw-rw-rw-   0        0        0     1192 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/upgrade_app.py
--rw-rw-rw-   0        0        0     1202 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.7/uhf/reader/protocol/upgrade_baseband.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhf/reader/utils/
--rw-rw-rw-   0        0        0      768 2020-10-09 10:11:25.000000 uhfReaderApi-0.0.7/uhf/reader/utils/HexUtils.py
--rw-rw-rw-   0        0        0     4466 2020-03-10 07:22:38.000000 uhfReaderApi-0.0.7/uhf/reader/utils/ThreadPool.py
--rw-rw-rw-   0        0        0      692 2023-05-10 08:10:19.000000 uhfReaderApi-0.0.7/uhf/reader/utils/__init__.py
--rw-rw-rw-   0        0        0     3989 2022-01-14 02:07:14.000000 uhfReaderApi-0.0.7/uhf/reader/utils/byteBuffer.py
--rw-rw-rw-   0        0        0     1489 2020-05-13 06:02:47.000000 uhfReaderApi-0.0.7/uhf/reader/utils/byteStruct.py
--rw-rw-rw-   0        0        0     1318 2020-10-09 09:57:03.000000 uhfReaderApi-0.0.7/uhf/reader/utils/dateUtils.py
--rw-rw-rw-   0        0        0      219 2020-11-20 07:18:46.000000 uhfReaderApi-0.0.7/uhf/reader/utils/decodeUtils.py
--rw-rw-rw-   0        0        0      759 2023-05-10 08:05:06.000000 uhfReaderApi-0.0.7/uhf/reader/utils/hid_utils.py
--rw-rw-rw-   0        0        0     1675 2020-09-28 09:44:55.000000 uhfReaderApi-0.0.7/uhf/reader/utils/pcUtils.py
--rw-rw-rw-   0        0        0     2392 2020-10-09 10:13:53.000000 uhfReaderApi-0.0.7/uhf/reader/utils/ring_buffer.py
--rw-rw-rw-   0        0        0      309 2020-10-09 10:15:44.000000 uhfReaderApi-0.0.7/uhf/reader/utils/serial_utils.py
--rw-rw-rw-   0        0        0     2531 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.7/uhf/reader/utils/usb_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/
--rw-rw-rw-   0        0        0      300 2023-05-10 08:12:34.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6436 2023-05-10 08:12:35.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:12:34.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-10 08:12:34.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 08:12:34.000000 uhfReaderApi-0.0.7/uhfReaderApi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:41.000000 uhfReaderApi-0.0.8/
+-rw-rw-rw-   0        0        0      300 2023-05-10 09:01:41.000000 uhfReaderApi-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:01:41.000000 uhfReaderApi-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-05-10 09:01:37.000000 uhfReaderApi-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhf/
+-rw-rw-rw-   0        0        0     3144 2022-08-18 10:16:17.000000 uhfReaderApi-0.0.8/uhf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhf/reader/
+-rw-rw-rw-   0        0        0    17157 2022-08-05 03:05:36.000000 uhfReaderApi-0.0.8/uhf/reader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhf/reader/communication/
+-rw-rw-rw-   0        0        0      422 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.8/uhf/reader/communication/__init__.py
+-rw-rw-rw-   0        0        0    10958 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.8/uhf/reader/communication/gclient.py
+-rw-rw-rw-   0        0        0     2186 2020-08-17 07:43:04.000000 uhfReaderApi-0.0.8/uhf/reader/communication/gserver.py
+-rw-rw-rw-   0        0        0     2270 2022-08-18 09:28:23.000000 uhfReaderApi-0.0.8/uhf/reader/communication/hid.py
+-rw-rw-rw-   0        0        0     4016 2021-04-22 07:59:15.000000 uhfReaderApi-0.0.8/uhf/reader/communication/interface.py
+-rw-rw-rw-   0        0        0     2609 2020-12-16 02:27:13.000000 uhfReaderApi-0.0.8/uhf/reader/communication/serial_client.py
+-rw-rw-rw-   0        0        0     2735 2020-12-30 08:51:55.000000 uhfReaderApi-0.0.8/uhf/reader/communication/tcp_client.py
+-rw-rw-rw-   0        0        0     1547 2020-08-17 07:47:02.000000 uhfReaderApi-0.0.8/uhf/reader/communication/tcp_server.py
+-rw-rw-rw-   0        0        0     3892 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.8/uhf/reader/communication/usb_hid.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:41.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/
+-rw-rw-rw-   0        0        0    10103 2022-08-18 09:19:07.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1609 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/action_param_fail.py
+-rw-rw-rw-   0        0        0     1612 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/action_param_success.py
+-rw-rw-rw-   0        0        0      703 2022-08-18 09:19:07.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_all_gpiState.py
+-rw-rw-rw-   0        0        0      618 2020-12-02 06:22:16.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_clearCacheData.py
+-rw-rw-rw-   0        0        0      585 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_del_whiteList.py
+-rw-rw-rw-   0        0        0      795 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_baseVersion.py
+-rw-rw-rw-   0        0        0      681 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_breakpointResume.py
+-rw-rw-rw-   0        0        0      634 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_cacheTagData.py
+-rw-rw-rw-   0        0        0     2066 2020-08-18 11:37:45.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_easAlarm.py
+-rw-rw-rw-   0        0        0     1876 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_ethernetIp.py
+-rw-rw-rw-   0        0        0      773 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_gpiState.py
+-rw-rw-rw-   0        0        0     1650 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_gpiTrigger.py
+-rw-rw-rw-   0        0        0     1357 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_httpParam.py
+-rw-rw-rw-   0        0        0     2324 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerInfo.py
+-rw-rw-rw-   0        0        0     1030 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerMac.py
+-rw-rw-rw-   0        0        0      855 2020-08-18 09:53:50.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerTime.py
+-rw-rw-rw-   0        0        0      755 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_rs485.py
+-rw-rw-rw-   0        0        0      692 2020-08-18 09:36:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_serialParam.py
+-rw-rw-rw-   0        0        0     1311 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_tcpMode.py
+-rw-rw-rw-   0        0        0     1024 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_udpParam.py
+-rw-rw-rw-   0        0        0     1028 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteList.py
+-rw-rw-rw-   0        0        0      793 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteListAction.py
+-rw-rw-rw-   0        0        0      781 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteListSwitch.py
+-rw-rw-rw-   0        0        0      899 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wiegand.py
+-rw-rw-rw-   0        0        0      789 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiConnectStatus.py
+-rw-rw-rw-   0        0        0     1044 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiHotspotSearch.py
+-rw-rw-rw-   0        0        0     1932 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiIp.py
+-rw-rw-rw-   0        0        0      680 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiSwitch.py
+-rw-rw-rw-   0        0        0      893 2020-12-02 06:09:18.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_gpiOver.py
+-rw-rw-rw-   0        0        0      892 2020-12-02 06:10:20.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_gpiStart.py
+-rw-rw-rw-   0        0        0      718 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_heartbeat.py
+-rw-rw-rw-   0        0        0     1182 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_import_whiteList.py
+-rw-rw-rw-   0        0        0      368 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_reset.py
+-rw-rw-rw-   0        0        0      701 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_restoreDefault.py
+-rw-rw-rw-   0        0        0      863 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_beep.py
+-rw-rw-rw-   0        0        0      786 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_beepOnOff.py
+-rw-rw-rw-   0        0        0      784 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_breakpointResume.py
+-rw-rw-rw-   0        0        0     2045 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_easAlarm.py
+-rw-rw-rw-   0        0        0     2145 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_ethernetIp.py
+-rw-rw-rw-   0        0        0     1819 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_gpiTrigger.py
+-rw-rw-rw-   0        0        0     5685 2022-08-18 08:40:29.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_gpo.py
+-rw-rw-rw-   0        0        0     1390 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_httpParam.py
+-rw-rw-rw-   0        0        0      872 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_readerTime.py
+-rw-rw-rw-   0        0        0      947 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_rs485.py
+-rw-rw-rw-   0        0        0      833 2020-10-26 03:24:47.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_serialParam.py
+-rw-rw-rw-   0        0        0     1525 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_tpcMode.py
+-rw-rw-rw-   0        0        0     1398 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_udpParam.py
+-rw-rw-rw-   0        0        0      896 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_whiteListAction.py
+-rw-rw-rw-   0        0        0      881 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_whiteListSwitch.py
+-rw-rw-rw-   0        0        0     1197 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wiegand.py
+-rw-rw-rw-   0        0        0     1545 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiHotspot.py
+-rw-rw-rw-   0        0        0     2313 2020-08-24 07:51:37.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiIp.py
+-rw-rw-rw-   0        0        0      787 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiSwitch.py
+-rw-rw-rw-   0        0        0      772 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_tagDataReply.py
+-rw-rw-rw-   0        0        0      540 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/app_wifiHotspotSearch.py
+-rw-rw-rw-   0        0        0     1458 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyEpc.py
+-rw-rw-rw-   0        0        0     1775 2022-01-14 02:32:38.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyGJb.py
+-rw-rw-rw-   0        0        0     1773 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyGb.py
+-rw-rw-rw-   0        0        0      807 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_antennaHub.py
+-rw-rw-rw-   0        0        0      768 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_autoDormancy.py
+-rw-rw-rw-   0        0        0      958 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_baseband.py
+-rw-rw-rw-   0        0        0     1277 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_capabilities.py
+-rw-rw-rw-   0        0        0      694 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_freRange.py
+-rw-rw-rw-   0        0        0      866 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_frequency.py
+-rw-rw-rw-   0        0        0     1362 2020-09-18 07:26:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_gb_baseband.py
+-rw-rw-rw-   0        0        0      801 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_power.py
+-rw-rw-rw-   0        0        0     1000 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_residenceTime.py
+-rw-rw-rw-   0        0        0      771 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_tagLog.py
+-rw-rw-rw-   0        0        0     1524 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventory6b.py
+-rw-rw-rw-   0        0        0     3723 2020-08-17 10:14:57.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryEpc.py
+-rw-rw-rw-   0        0        0     2154 2022-01-14 02:21:40.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryGJb.py
+-rw-rw-rw-   0        0        0     2151 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryGb.py
+-rw-rw-rw-   0        0        0      964 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventory_Hybrid.py
+-rw-rw-rw-   0        0        0     1284 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_lock6b.py
+-rw-rw-rw-   0        0        0     1296 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_lock6bGet.py
+-rw-rw-rw-   0        0        0     1759 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockEpc.py
+-rw-rw-rw-   0        0        0     2020 2022-01-14 02:32:38.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockGJb.py
+-rw-rw-rw-   0        0        0     2018 2022-01-14 02:11:54.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockGb.py
+-rw-rw-rw-   0        0        0     1715 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_safe_attestation.py
+-rw-rw-rw-   0        0        0     1015 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_antennaHub.py
+-rw-rw-rw-   0        0        0     1024 2020-08-17 09:53:32.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_autoDormancy.py
+-rw-rw-rw-   0        0        0     1593 2020-08-17 09:53:33.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_baseband.py
+-rw-rw-rw-   0        0        0      883 2020-08-17 09:53:57.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_freRange.py
+-rw-rw-rw-   0        0        0     1417 2020-08-17 09:53:58.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_frequency.py
+-rw-rw-rw-   0        0        0     2119 2020-09-18 07:20:38.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_gb_baseband.py
+-rw-rw-rw-   0        0        0     1248 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_power.py
+-rw-rw-rw-   0        0        0     1197 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_residenceTime.py
+-rw-rw-rw-   0        0        0     1112 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_tagLog.py
+-rw-rw-rw-   0        0        0      499 2020-12-02 06:22:16.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_stop.py
+-rw-rw-rw-   0        0        0     1618 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_super_rw.py
+-rw-rw-rw-   0        0        0     1577 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_write6b.py
+-rw-rw-rw-   0        0        0     2437 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeEpc.py
+-rw-rw-rw-   0        0        0     2719 2022-01-14 02:28:29.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeGJb.py
+-rw-rw-rw-   0        0        0     2885 2022-01-14 02:29:37.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeGb.py
+-rw-rw-rw-   0        0        0     2424 2020-08-17 09:56:31.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeMonzaQt.py
+-rw-rw-rw-   0        0        0     6030 2022-08-18 09:02:45.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/enumg.py
+-rw-rw-rw-   0        0        0     1428 2020-08-18 01:36:44.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_6b_info.py
+-rw-rw-rw-   0        0        0      683 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_6b_over.py
+-rw-rw-rw-   0        0        0     3977 2023-05-10 08:09:54.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_epc_info.py
+-rw-rw-rw-   0        0        0      687 2020-08-17 09:57:46.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_epc_over.py
+-rw-rw-rw-   0        0        0     1831 2020-08-18 01:36:44.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_gb_info.py
+-rw-rw-rw-   0        0        0      683 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_gb_over.py
+-rw-rw-rw-   0        0        0     5415 2022-01-14 02:07:14.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/message.py
+-rw-rw-rw-   0        0        0      693 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_6b_readUserData.py
+-rw-rw-rw-   0        0        0      700 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_fastId.py
+-rw-rw-rw-   0        0        0     1034 2020-08-03 03:44:41.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_filter.py
+-rw-rw-rw-   0        0        0      693 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readEpc.py
+-rw-rw-rw-   0        0        0      698 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readReserved.py
+-rw-rw-rw-   0        0        0      685 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readTid.py
+-rw-rw-rw-   0        0        0      698 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readUserData.py
+-rw-rw-rw-   0        0        0      847 2020-08-03 02:56:24.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_gb_readUserData.py
+-rw-rw-rw-   0        0        0      772 2020-08-03 02:56:25.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/param_safe_attestation.py
+-rw-rw-rw-   0        0        0      112 2020-06-04 11:33:17.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/parameter.py
+-rw-rw-rw-   0        0        0     1034 2020-08-17 09:57:45.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_carrierWave.py
+-rw-rw-rw-   0        0        0      569 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_dc_autobias.py
+-rw-rw-rw-   0        0        0      881 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_dcbias.py
+-rw-rw-rw-   0        0        0      665 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_dcbias_get.py
+-rw-rw-rw-   0        0        0      628 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_encryptionParam_get.py
+-rw-rw-rw-   0        0        0      835 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_encryptionParam_set.py
+-rw-rw-rw-   0        0        0     1255 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_env_rssiAutoDetection.py
+-rw-rw-rw-   0        0        0     1349 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_env_rssiDetection.py
+-rw-rw-rw-   0        0        0      708 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_get_rssiCalibration.py
+-rw-rw-rw-   0        0        0     1102 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_power_calibration.py
+-rw-rw-rw-   0        0        0     1065 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_power_calibrationGet.py
+-rw-rw-rw-   0        0        0     1366 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_r2000_readWrite.py
+-rw-rw-rw-   0        0        0     1237 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_r2000_receivingGain.py
+-rw-rw-rw-   0        0        0      948 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_serialno_set.py
+-rw-rw-rw-   0        0        0      823 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_set_rssiCalibration.py
+-rw-rw-rw-   0        0        0      763 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_vswr_check.py
+-rw-rw-rw-   0        0        0     1220 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_workMode_get.py
+-rw-rw-rw-   0        0        0     1551 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/test_workMode_set.py
+-rw-rw-rw-   0        0        0     1192 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/upgrade_app.py
+-rw-rw-rw-   0        0        0     1202 2020-08-17 10:02:55.000000 uhfReaderApi-0.0.8/uhf/reader/protocol/upgrade_baseband.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:41.000000 uhfReaderApi-0.0.8/uhf/reader/utils/
+-rw-rw-rw-   0        0        0      768 2020-10-09 10:11:25.000000 uhfReaderApi-0.0.8/uhf/reader/utils/HexUtils.py
+-rw-rw-rw-   0        0        0     4466 2020-03-10 07:22:38.000000 uhfReaderApi-0.0.8/uhf/reader/utils/ThreadPool.py
+-rw-rw-rw-   0        0        0      692 2023-05-10 08:10:19.000000 uhfReaderApi-0.0.8/uhf/reader/utils/__init__.py
+-rw-rw-rw-   0        0        0     3989 2022-01-14 02:07:14.000000 uhfReaderApi-0.0.8/uhf/reader/utils/byteBuffer.py
+-rw-rw-rw-   0        0        0     1489 2020-05-13 06:02:47.000000 uhfReaderApi-0.0.8/uhf/reader/utils/byteStruct.py
+-rw-rw-rw-   0        0        0     1318 2020-10-09 09:57:03.000000 uhfReaderApi-0.0.8/uhf/reader/utils/dateUtils.py
+-rw-rw-rw-   0        0        0      219 2020-11-20 07:18:46.000000 uhfReaderApi-0.0.8/uhf/reader/utils/decodeUtils.py
+-rw-rw-rw-   0        0        0      759 2023-05-10 08:05:06.000000 uhfReaderApi-0.0.8/uhf/reader/utils/hid_utils.py
+-rw-rw-rw-   0        0        0     1675 2020-09-28 09:44:55.000000 uhfReaderApi-0.0.8/uhf/reader/utils/pcUtils.py
+-rw-rw-rw-   0        0        0     2392 2020-10-09 10:13:53.000000 uhfReaderApi-0.0.8/uhf/reader/utils/ring_buffer.py
+-rw-rw-rw-   0        0        0      309 2020-10-09 10:15:44.000000 uhfReaderApi-0.0.8/uhf/reader/utils/serial_utils.py
+-rw-rw-rw-   0        0        0     2535 2023-05-10 09:01:37.000000 uhfReaderApi-0.0.8/uhf/reader/utils/usb_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6436 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 09:01:40.000000 uhfReaderApi-0.0.8/uhfReaderApi.egg-info/top_level.txt
```

### Comparing `uhfReaderApi-0.0.7/setup.py` & `uhfReaderApi-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="uhfReaderApi",
-    version="0.0.7",
+    version="0.0.8",
     author="rfid",
     description="ReaderApi",
     platforms=['linux/Windows'],
     # uhf.
     packages=setuptools.find_namespace_packages(
         exclude=["*.qt", "qt.*", "qt", "*.qt.*", "*.test", "test.*", "test",
                  "*.test.*"]),
```

### Comparing `uhfReaderApi-0.0.7/uhf/__init__.py` & `uhfReaderApi-0.0.8/uhf/__init__.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/__init__.py` & `uhfReaderApi-0.0.8/uhf/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/gclient.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/gclient.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/gserver.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/gserver.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/hid.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/hid.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/interface.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/interface.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/serial_client.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/serial_client.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/tcp_client.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/tcp_client.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/tcp_server.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/tcp_server.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/communication/usb_hid.py` & `uhfReaderApi-0.0.8/uhf/reader/communication/usb_hid.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/__init__.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/action_param_fail.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/action_param_fail.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/action_param_success.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/action_param_success.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_all_gpiState.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_all_gpiState.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_clearCacheData.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_clearCacheData.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_del_whiteList.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_del_whiteList.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_baseVersion.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_baseVersion.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_breakpointResume.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_breakpointResume.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_cacheTagData.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_cacheTagData.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_easAlarm.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_easAlarm.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_ethernetIp.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_ethernetIp.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_gpiState.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_gpiState.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_gpiTrigger.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_gpiTrigger.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_httpParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_httpParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerInfo.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerInfo.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerMac.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerMac.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_readerTime.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_readerTime.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_rs485.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_rs485.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_serialParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_serialParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_tcpMode.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_tcpMode.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_udpParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_udpParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteList.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteList.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteListAction.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteListAction.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_whiteListSwitch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_whiteListSwitch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wiegand.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wiegand.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiConnectStatus.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiConnectStatus.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiHotspotSearch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiHotspotSearch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiIp.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiIp.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_get_wifiSwitch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_get_wifiSwitch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_gpiOver.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_gpiOver.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_gpiStart.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_gpiStart.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_heartbeat.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_heartbeat.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_import_whiteList.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_import_whiteList.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_restoreDefault.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_restoreDefault.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_beep.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_beep.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_beepOnOff.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_beepOnOff.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_breakpointResume.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_breakpointResume.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_easAlarm.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_easAlarm.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_ethernetIp.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_ethernetIp.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_gpiTrigger.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_gpiTrigger.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_gpo.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_gpo.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_httpParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_httpParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_readerTime.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_readerTime.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_rs485.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_rs485.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_serialParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_serialParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_tpcMode.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_tpcMode.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_udpParam.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_udpParam.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_whiteListAction.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_whiteListAction.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_whiteListSwitch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_whiteListSwitch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wiegand.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wiegand.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiHotspot.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiHotspot.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiIp.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiIp.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_set_wifiSwitch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_set_wifiSwitch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_tagDataReply.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_tagDataReply.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/app_wifiHotspotSearch.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/app_wifiHotspotSearch.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyEpc.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyEpc.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyGJb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyGJb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_destroyGb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_destroyGb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_antennaHub.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_antennaHub.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_autoDormancy.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_autoDormancy.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_baseband.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_baseband.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_capabilities.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_capabilities.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_freRange.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_freRange.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_frequency.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_frequency.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_gb_baseband.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_gb_baseband.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_power.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_power.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_residenceTime.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_residenceTime.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_get_tagLog.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_get_tagLog.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventory6b.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventory6b.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryEpc.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryEpc.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryGJb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryGJb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventoryGb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventoryGb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_inventory_Hybrid.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_inventory_Hybrid.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_lock6b.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_lock6b.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_lock6bGet.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_lock6bGet.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockEpc.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockEpc.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockGJb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockGJb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_lockGb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_lockGb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_safe_attestation.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_safe_attestation.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_antennaHub.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_antennaHub.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_autoDormancy.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_autoDormancy.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_baseband.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_baseband.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_freRange.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_freRange.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_frequency.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_frequency.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_gb_baseband.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_gb_baseband.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_power.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_power.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_residenceTime.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_residenceTime.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_set_tagLog.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_set_tagLog.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_super_rw.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_super_rw.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_write6b.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_write6b.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeEpc.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeEpc.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeGJb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeGJb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeGb.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeGb.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/base_writeMonzaQt.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/base_writeMonzaQt.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/enumg.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/enumg.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_6b_info.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_6b_info.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_6b_over.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_6b_over.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_epc_info.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_epc_info.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_epc_over.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_epc_over.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_gb_info.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_gb_info.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/log_base_gb_over.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/log_base_gb_over.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/message.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/message.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_6b_readUserData.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_6b_readUserData.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_fastId.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_fastId.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_filter.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_filter.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readEpc.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readEpc.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readReserved.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readReserved.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readTid.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readTid.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_epc_readUserData.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_epc_readUserData.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_gb_readUserData.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_gb_readUserData.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/param_safe_attestation.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/param_safe_attestation.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_carrierWave.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_carrierWave.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_dc_autobias.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_dc_autobias.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_dcbias.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_dcbias.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_dcbias_get.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_dcbias_get.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_encryptionParam_get.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_encryptionParam_get.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_encryptionParam_set.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_encryptionParam_set.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_env_rssiAutoDetection.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_env_rssiAutoDetection.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_env_rssiDetection.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_env_rssiDetection.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_get_rssiCalibration.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_get_rssiCalibration.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_power_calibration.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_power_calibration.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_power_calibrationGet.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_power_calibrationGet.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_r2000_readWrite.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_r2000_readWrite.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_r2000_receivingGain.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_r2000_receivingGain.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_serialno_set.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_serialno_set.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_set_rssiCalibration.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_set_rssiCalibration.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_vswr_check.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_vswr_check.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_workMode_get.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_workMode_get.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/test_workMode_set.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/test_workMode_set.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/upgrade_app.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/upgrade_app.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/protocol/upgrade_baseband.py` & `uhfReaderApi-0.0.8/uhf/reader/protocol/upgrade_baseband.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/HexUtils.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/HexUtils.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/ThreadPool.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/__init__.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/byteBuffer.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/byteBuffer.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/byteStruct.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/byteStruct.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/dateUtils.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/dateUtils.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/hid_utils.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/hid_utils.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/pcUtils.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/pcUtils.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/ring_buffer.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `uhfReaderApi-0.0.7/uhf/reader/utils/usb_utils.py` & `uhfReaderApi-0.0.8/uhf/reader/utils/usb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import usb.core
-import usb.util
+# import usb.core
+# import usb.util
 
 
 # import time
 
 
 # import platform
 #
```

### Comparing `uhfReaderApi-0.0.7/uhfReaderApi.egg-info/SOURCES.txt` & `uhfReaderApi-0.0.8/uhfReaderApi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

