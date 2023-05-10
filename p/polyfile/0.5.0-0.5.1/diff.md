# Comparing `tmp/polyfile-0.5.0.tar.gz` & `tmp/polyfile-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfile-0.5.0.tar", last modified: Tue Nov 22 16:00:27 2022, max compression
+gzip compressed data, was "polyfile-0.5.1.tar", last modified: Wed May 10 14:56:52 2023, max compression
```

## Comparing `polyfile-0.5.0.tar` & `polyfile-0.5.1.tar`

### file list

```diff
@@ -1,587 +1,596 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.884999 polyfile-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-11-22 16:00:01.000000 polyfile-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    17489 2022-11-22 16:00:27.884999 polyfile-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16809 2022-11-22 16:00:01.000000 polyfile-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.816997 polyfile-0.5.0/polyfile/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17673 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (122)    42407 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/debugger.py
--rw-r--r--   0 runner    (1001) docker     (122)    11218 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/expressions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11188 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4100 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/html.py
--rw-r--r--   0 runner    (1001) docker     (122)     2310 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/iterators.py
--rw-r--r--   0 runner    (1001) docker     (122)      702 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/jpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.816997 polyfile-0.5.0/polyfile/kaitai/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5707 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    10314 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.840998 polyfile-0.5.0/polyfile/kaitai/parsers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5088 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/aix_utmp.py
--rw-r--r--   0 runner    (1001) docker     (122)    16311 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/allegro_dat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/andes_firmware.py
--rw-r--r--   0 runner    (1001) docker     (122)     5264 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_asus.py
--rw-r--r--   0 runner    (1001) docker     (122)     8361 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_huawei.py
--rw-r--r--   0 runner    (1001) docker     (122)    12098 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_qcom.py
--rw-r--r--   0 runner    (1001) docker     (122)     6432 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_dto.py
--rw-r--r--   0 runner    (1001) docker     (122)    13778 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_img.py
--rw-r--r--   0 runner    (1001) docker     (122)     3935 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_nanoapp_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     7201 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_opengl_shaders_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)    11435 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_sparse.py
--rw-r--r--   0 runner    (1001) docker     (122)    22822 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/android_super.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/apm_partition_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     7718 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/apple_single_double.py
--rw-r--r--   0 runner    (1001) docker     (122)     9565 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/asn1_der.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/au.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/avantes_roh60.py
--rw-r--r--   0 runner    (1001) docker     (122)    13489 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/avi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5553 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/bcd.py
--rw-r--r--   0 runner    (1001) docker     (122)    10696 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/bitcoin_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)    16180 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/blender_blend.py
--rw-r--r--   0 runner    (1001) docker     (122)    37749 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/bmp.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/broadcom_trx.py
--rw-r--r--   0 runner    (1001) docker     (122)    19067 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/bson.py
--rw-r--r--   0 runner    (1001) docker     (122)    14505 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/btrfs_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/bytes_with_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     8409 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/chrome_pak.py
--rw-r--r--   0 runner    (1001) docker     (122)    17671 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/code_6502.py
--rw-r--r--   0 runner    (1001) docker     (122)    11500 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/compressed_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/cpio_old_le.py
--rw-r--r--   0 runner    (1001) docker     (122)    14804 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/cramfs.py
--rw-r--r--   0 runner    (1001) docker     (122)    15487 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/creative_voice_file.py
--rw-r--r--   0 runner    (1001) docker     (122)    13658 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)    35086 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_0.py
--rw-r--r--   0 runner    (1001) docker     (122)    20261 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_1.py
--rw-r--r--   0 runner    (1001) docker     (122)    18157 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_variable_length_integer.py
--rw-r--r--   0 runner    (1001) docker     (122)    49963 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dex.py
--rw-r--r--   0 runner    (1001) docker     (122)   197752 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dicom.py
--rw-r--r--   0 runner    (1001) docker     (122)     9538 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dime_message.py
--rw-r--r--   0 runner    (1001) docker     (122)    24113 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dns_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)    30308 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/doom_wad.py
--rw-r--r--   0 runner    (1001) docker     (122)     8576 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dos_datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     8216 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dos_mz.py
--rw-r--r--   0 runner    (1001) docker     (122)    25076 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ds_store.py
--rw-r--r--   0 runner    (1001) docker     (122)    13994 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dtb.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/dune_2_pak.py
--rw-r--r--   0 runner    (1001) docker     (122)    23167 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/edid.py
--rw-r--r--   0 runner    (1001) docker     (122)    16125 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/efivar_signature_list.py
--rw-r--r--   0 runner    (1001) docker     (122)   108372 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/elf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ethernet_frame.py
--rw-r--r--   0 runner    (1001) docker     (122)    30390 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/exif.py
--rw-r--r--   0 runner    (1001) docker     (122)    27149 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ext2.py
--rw-r--r--   0 runner    (1001) docker     (122)     7681 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/fallout2_dat.py
--rw-r--r--   0 runner    (1001) docker     (122)     7063 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/fallout_dat.py
--rw-r--r--   0 runner    (1001) docker     (122)    30681 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/fasttracker_xm_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ftl_dat.py
--rw-r--r--   0 runner    (1001) docker     (122)     7321 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/genmidi_op2.py
--rw-r--r--   0 runner    (1001) docker     (122)    24355 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gettext_mo.py
--rw-r--r--   0 runner    (1001) docker     (122)    22124 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gif.py
--rw-r--r--   0 runner    (1001) docker     (122)    11233 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gimp_brush.py
--rw-r--r--   0 runner    (1001) docker     (122)     4823 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/glibc_utmp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5410 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gltf_binary.py
--rw-r--r--   0 runner    (1001) docker     (122)     6636 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/google_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8297 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gpt_partition_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6227 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gran_turismo_vol.py
--rw-r--r--   0 runner    (1001) docker     (122)    15254 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/grub2_font.py
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/gzip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/hashcat_restore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4729 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/hccap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5124 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/hccapx.py
--rw-r--r--   0 runner    (1001) docker     (122)     8289 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/heaps_pak.py
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/heroes_of_might_and_magic_agg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/heroes_of_might_and_magic_bmp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5929 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/icmp_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ico.py
--rw-r--r--   0 runner    (1001) docker     (122)     7331 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/id3v1_1.py
--rw-r--r--   0 runner    (1001) docker     (122)    14483 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/id3v2_3.py
--rw-r--r--   0 runner    (1001) docker     (122)    20412 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/id3v2_4.py
--rw-r--r--   0 runner    (1001) docker     (122)    13021 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ines.py
--rw-r--r--   0 runner    (1001) docker     (122)     6736 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ipv4_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ipv6_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)    27743 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/iso9660.py
--rw-r--r--   0 runner    (1001) docker     (122)    46144 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/java_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    16309 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/jpeg.py
--rw-r--r--   0 runner    (1001) docker     (122)     8224 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/luks.py
--rw-r--r--   0 runner    (1001) docker     (122)    19846 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/lvm2.py
--rw-r--r--   0 runner    (1001) docker     (122)     7497 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/lzh.py
--rw-r--r--   0 runner    (1001) docker     (122)    23884 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mac_os_resource_snd.py
--rw-r--r--   0 runner    (1001) docker     (122)   148271 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mach_o.py
--rw-r--r--   0 runner    (1001) docker     (122)     4277 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mach_o_fat.py
--rw-r--r--   0 runner    (1001) docker     (122)    17454 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/magicavoxel_vox.py
--rw-r--r--   0 runner    (1001) docker     (122)    24698 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mbr_partition_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    48729 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mcap.py
--rw-r--r--   0 runner    (1001) docker     (122)    14321 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_cfb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12376 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_network_monitor_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    39086 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_pe.py
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mifare_classic.py
--rw-r--r--   0 runner    (1001) docker     (122)    21255 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/minecraft_nbt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/monomakh_sapr_chg.py
--rw-r--r--   0 runner    (1001) docker     (122)    11146 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mozilla_mar.py
--rw-r--r--   0 runner    (1001) docker     (122)    14096 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/mp4.py
--rw-r--r--   0 runner    (1001) docker     (122)    18187 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (122)    69659 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/nitf.py
--rw-r--r--   0 runner    (1001) docker     (122)    66870 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/nt_mdt.py
--rw-r--r--   0 runner    (1001) docker     (122)     7466 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/nt_mdt_pal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ogg.py
--rw-r--r--   0 runner    (1001) docker     (122)    46147 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/openpgp_message.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/packet_ppi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/pcap.py
--rw-r--r--   0 runner    (1001) docker     (122)    25501 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/pcf_font.py
--rw-r--r--   0 runner    (1001) docker     (122)     9213 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/pcx.py
--rw-r--r--   0 runner    (1001) docker     (122)     3107 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/pcx_dcx.py
--rw-r--r--   0 runner    (1001) docker     (122)    19299 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/phar_without_stub.py
--rw-r--r--   0 runner    (1001) docker     (122)    24615 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/php_serialized_value.py
--rw-r--r--   0 runner    (1001) docker     (122)    32303 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/png.py
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/protocol_body.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/psx_tim.py
--rw-r--r--   0 runner    (1001) docker     (122)    30279 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/python_pickle.py
--rw-r--r--   0 runner    (1001) docker     (122)    20413 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/python_pyc_27.py
--rw-r--r--   0 runner    (1001) docker     (122)    20983 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/quake_mdl.py
--rw-r--r--   0 runner    (1001) docker     (122)     4580 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/quake_pak.py
--rw-r--r--   0 runner    (1001) docker     (122)    24688 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/quicktime_mov.py
--rw-r--r--   0 runner    (1001) docker     (122)    11690 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/rar.py
--rw-r--r--   0 runner    (1001) docker     (122)    29723 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/regf.py
--rw-r--r--   0 runner    (1001) docker     (122)    33901 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/renderware_binary_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)    32958 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/resource_fork.py
--rw-r--r--   0 runner    (1001) docker     (122)    18135 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/riff.py
--rw-r--r--   0 runner    (1001) docker     (122)    38378 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/rpm.py
--rw-r--r--   0 runner    (1001) docker     (122)    25558 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/rtcp_payload.py
--rw-r--r--   0 runner    (1001) docker     (122)     6130 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/rtp_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/rtpdump.py
--rw-r--r--   0 runner    (1001) docker     (122)    18603 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ruby_marshal.py
--rw-r--r--   0 runner    (1001) docker     (122)    23542 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/s3m.py
--rw-r--r--   0 runner    (1001) docker     (122)    11663 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/saints_row_2_vpp_pc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8321 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/shapefile_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    45337 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/shapefile_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     9759 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/some_ip.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_container.py
--rw-r--r--   0 runner    (1001) docker     (122)     4135 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7843 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd_entries.py
--rw-r--r--   0 runner    (1001) docker     (122)    18418 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    18941 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/specpr.py
--rw-r--r--   0 runner    (1001) docker     (122)    22295 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (122)    10547 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ssh_public_key.py
--rw-r--r--   0 runner    (1001) docker     (122)    16581 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/standard_midi_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     4732 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/stl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8793 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/sudoers_ts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18099 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/swf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17782 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/systemd_journal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/tcp_segment.py
--rw-r--r--   0 runner    (1001) docker     (122)    10745 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/tga.py
--rw-r--r--   0 runner    (1001) docker     (122)    12742 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/tls_client_hello.py
--rw-r--r--   0 runner    (1001) docker     (122)    15034 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/tr_dos_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     9032 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/tsm.py
--rw-r--r--   0 runner    (1001) docker     (122)   104490 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/ttf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/udp_datagram.py
--rw-r--r--   0 runner    (1001) docker     (122)    11124 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/uefi_te.py
--rw-r--r--   0 runner    (1001) docker     (122)     6650 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/uimage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5932 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/utf8_string.py
--rw-r--r--   0 runner    (1001) docker     (122)    22828 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vdi.py
--rw-r--r--   0 runner    (1001) docker     (122)    21194 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vfat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vlq_base128_be.py
--rw-r--r--   0 runner    (1001) docker     (122)     5501 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vlq_base128_le.py
--rw-r--r--   0 runner    (1001) docker     (122)     8628 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vmware_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (122)     5131 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/vp8_ivf.py
--rw-r--r--   0 runner    (1001) docker     (122)    16616 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/warcraft_2_pud.py
--rw-r--r--   0 runner    (1001) docker     (122)    42097 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/wav.py
--rw-r--r--   0 runner    (1001) docker     (122)     7598 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/websocket.py
--rw-r--r--   0 runner    (1001) docker     (122)    14896 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_evt_log.py
--rw-r--r--   0 runner    (1001) docker     (122)    24003 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_lnk_file.py
--rw-r--r--   0 runner    (1001) docker     (122)    27119 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_minidump.py
--rw-r--r--   0 runner    (1001) docker     (122)    10555 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_resource_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     7883 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_shell_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/windows_systemtime.py
--rw-r--r--   0 runner    (1001) docker     (122)    20034 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/wmf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9079 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/xar.py
--rw-r--r--   0 runner    (1001) docker     (122)     9802 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/xwd.py
--rw-r--r--   0 runner    (1001) docker     (122)    34076 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/zip.py
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/zisofs.py
--rw-r--r--   0 runner    (1001) docker     (122)     8138 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitai/parsers/zx_spectrum_tap.py
--rw-r--r--   0 runner    (1001) docker     (122)     4296 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/kaitaimatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     7965 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/languagematcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4020 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)   115065 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.884999 polyfile-0.5.0/polyfile/magic_defs/
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     3731 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/acorn
--rw-r--r--   0 runner    (1001) docker     (122)      425 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/adi
--rw-r--r--   0 runner    (1001) docker     (122)     4490 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/adventure
--rw-r--r--   0 runner    (1001) docker     (122)      988 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/aes
--rw-r--r--   0 runner    (1001) docker     (122)     1377 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/algol68
--rw-r--r--   0 runner    (1001) docker     (122)      402 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/allegro
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/alliant
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/alpha
--rw-r--r--   0 runner    (1001) docker     (122)      385 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/amanda
--rw-r--r--   0 runner    (1001) docker     (122)     8789 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/amigaos
--rw-r--r--   0 runner    (1001) docker     (122)     7567 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/android
--rw-r--r--   0 runner    (1001) docker     (122)    51507 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/animation
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/aout
--rwxr-xr-x   0 runner    (1001) docker     (122)      822 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/apache
--rw-r--r--   0 runner    (1001) docker     (122)      276 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/apl
--rw-r--r--   0 runner    (1001) docker     (122)    24322 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/apple
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/application
--rw-r--r--   0 runner    (1001) docker     (122)      428 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/applix
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/apt
--rw-r--r--   0 runner    (1001) docker     (122)    73451 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/archive
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/aria
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/arm
--rw-r--r--   0 runner    (1001) docker     (122)     6547 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/asf
--rw-r--r--   0 runner    (1001) docker     (122)      700 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/assembler
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/asterix
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/att3b
--rw-r--r--   0 runner    (1001) docker     (122)    40257 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/audio
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/avm
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/basis
--rw-r--r--   0 runner    (1001) docker     (122)      289 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/beetle
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ber
--rw-r--r--   0 runner    (1001) docker     (122)      414 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bflt
--rw-r--r--   0 runner    (1001) docker     (122)      341 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bhl
--rw-r--r--   0 runner    (1001) docker     (122)     7683 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bioinformatics
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/biosig
--rw-r--r--   0 runner    (1001) docker     (122)      282 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/blackberry
--rw-r--r--   0 runner    (1001) docker     (122)      746 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/blcr
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/blender
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/blit
--rw-r--r--   0 runner    (1001) docker     (122)      381 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bm
--rw-r--r--   0 runner    (1001) docker     (122)      349 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bout
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bsdi
--rw-r--r--   0 runner    (1001) docker     (122)      327 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bsi
--rw-r--r--   0 runner    (1001) docker     (122)      429 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/btsnoop
--rw-r--r--   0 runner    (1001) docker     (122)      304 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/burp
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/bytecode
--rw-r--r--   0 runner    (1001) docker     (122)     3543 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/c-lang
--rw-r--r--   0 runner    (1001) docker     (122)     5795 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/c64
--rw-r--r--   0 runner    (1001) docker     (122)    15643 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cad
--rw-r--r--   0 runner    (1001) docker     (122)     3648 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cafebabe
--rw-r--r--   0 runner    (1001) docker     (122)      610 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cbor
--rw-r--r--   0 runner    (1001) docker     (122)      599 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ccf
--rw-r--r--   0 runner    (1001) docker     (122)      386 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cddb
--rw-r--r--   0 runner    (1001) docker     (122)      577 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/chord
--rw-r--r--   0 runner    (1001) docker     (122)      495 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cisco
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/citrus
--rw-r--r--   0 runner    (1001) docker     (122)      769 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/clarion
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/claris
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/clipper
--rw-r--r--   0 runner    (1001) docker     (122)     1138 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/clojure
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/coff
--rw-r--r--   0 runner    (1001) docker     (122)     7180 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/commands
--rw-r--r--   0 runner    (1001) docker     (122)      853 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/communications
--rw-r--r--   0 runner    (1001) docker     (122)    14852 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/compress
--rw-r--r--   0 runner    (1001) docker     (122)    41408 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/console
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/convex
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/coverage
--rw-r--r--   0 runner    (1001) docker     (122)      531 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cracklib
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/crypto
--rw-r--r--   0 runner    (1001) docker     (122)      385 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/csv
--rw-r--r--   0 runner    (1001) docker     (122)      297 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ctags
--rw-r--r--   0 runner    (1001) docker     (122)      824 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ctf
--rw-r--r--   0 runner    (1001) docker     (122)      403 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cubemap
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/cups
--rw-r--r--   0 runner    (1001) docker     (122)      379 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dact
--rw-r--r--   0 runner    (1001) docker     (122)    31552 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/database
--rw-r--r--   0 runner    (1001) docker     (122)     1848 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dataone
--rw-r--r--   0 runner    (1001) docker     (122)      630 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dbpf
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/der
--rw-r--r--   0 runner    (1001) docker     (122)      509 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/diamond
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dif
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/diff
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/digital
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dolby
--rw-r--r--   0 runner    (1001) docker     (122)      854 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dsf
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dump
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/dyadic
--rw-r--r--   0 runner    (1001) docker     (122)      350 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ebml
--rw-r--r--   0 runner    (1001) docker     (122)      377 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/edid
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/editors
--rw-r--r--   0 runner    (1001) docker     (122)      547 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/efi
--rw-r--r--   0 runner    (1001) docker     (122)    12568 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/elf
--rw-r--r--   0 runner    (1001) docker     (122)      725 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/encore
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/epoc
--rw-r--r--   0 runner    (1001) docker     (122)      709 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/erlang
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/espressif
--rw-r--r--   0 runner    (1001) docker     (122)      826 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/esri
--rw-r--r--   0 runner    (1001) docker     (122)     2033 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/etf
--rw-r--r--   0 runner    (1001) docker     (122)      516 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/fcs
--rw-r--r--   0 runner    (1001) docker     (122)   103933 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/filesystems
--rw-r--r--   0 runner    (1001) docker     (122)      488 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/finger
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/firmware
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/flash
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/flif
--rw-r--r--   0 runner    (1001) docker     (122)    16491 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/fonts
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/forth
--rw-r--r--   0 runner    (1001) docker     (122)      349 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/fortran
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/frame
--rw-r--r--   0 runner    (1001) docker     (122)     5476 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/freebsd
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/fsav
--rw-r--r--   0 runner    (1001) docker     (122)      430 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/fusecompress
--rw-r--r--   0 runner    (1001) docker     (122)    20686 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/games
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gcc
--rw-r--r--   0 runner    (1001) docker     (122)      344 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gconv
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gentoo
--rw-r--r--   0 runner    (1001) docker     (122)     6008 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/geo
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/geos
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gimp
--rw-r--r--   0 runner    (1001) docker     (122)      330 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/git
--rw-r--r--   0 runner    (1001) docker     (122)      879 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/glibc
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gnome
--rw-r--r--   0 runner    (1001) docker     (122)     6110 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gnu
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gnumeric
--rw-r--r--   0 runner    (1001) docker     (122)     9979 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gpt
--rw-r--r--   0 runner    (1001) docker     (122)      925 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gpu
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/grace
--rw-r--r--   0 runner    (1001) docker     (122)      580 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/graphviz
--rw-r--r--   0 runner    (1001) docker     (122)     1577 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/gringotts
--rw-r--r--   0 runner    (1001) docker     (122)      471 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/guile
--rw-r--r--   0 runner    (1001) docker     (122)      385 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/hardware
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/hitachi-sh
--rw-r--r--   0 runner    (1001) docker     (122)    14070 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/hp
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/human68k
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ibm370
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ibm6000
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/icc
--rw-r--r--   0 runner    (1001) docker     (122)     3032 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/iff
--rw-r--r--   0 runner    (1001) docker     (122)   145544 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/images
--rw-r--r--   0 runner    (1001) docker     (122)      333 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/inform
--rw-r--r--   0 runner    (1001) docker     (122)    13829 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/intel
--rw-r--r--   0 runner    (1001) docker     (122)      333 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/interleaf
--rw-r--r--   0 runner    (1001) docker     (122)      345 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/island
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ispell
--rw-r--r--   0 runner    (1001) docker     (122)      514 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/isz
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/java
--rw-r--r--   0 runner    (1001) docker     (122)     5265 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/javascript
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/jpeg
--rw-r--r--   0 runner    (1001) docker     (122)      390 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/json
--rw-r--r--   0 runner    (1001) docker     (122)      291 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/karma
--rw-r--r--   0 runner    (1001) docker     (122)      390 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/kde
--rw-r--r--   0 runner    (1001) docker     (122)      692 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/keepass
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/kerberos
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/kicad
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/kml
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lammps
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lecter
--rw-r--r--   0 runner    (1001) docker     (122)      528 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lex
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lif
--rw-r--r--   0 runner    (1001) docker     (122)    19300 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/linux
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lisp
--rw-r--r--   0 runner    (1001) docker     (122)      723 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/llvm
--rw-r--r--   0 runner    (1001) docker     (122)      543 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/locoscript
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/lua
--rw-r--r--   0 runner    (1001) docker     (122)     4958 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/luks
--rw-r--r--   0 runner    (1001) docker     (122)      370 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/m4
--rw-r--r--   0 runner    (1001) docker     (122)    10853 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mach
--rw-r--r--   0 runner    (1001) docker     (122)    16932 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/macintosh
--rw-r--r--   0 runner    (1001) docker     (122)      206 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/macos
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/magic
--rw-r--r--   0 runner    (1001) docker     (122)  6649560 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/magic.mgc
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mail.news
--rw-r--r--   0 runner    (1001) docker     (122)      893 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/make
--rw-r--r--   0 runner    (1001) docker     (122)    13740 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/map
--rw-r--r--   0 runner    (1001) docker     (122)     3873 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/maple
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/marc21
--rw-r--r--   0 runner    (1001) docker     (122)      300 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mathcad
--rw-r--r--   0 runner    (1001) docker     (122)     6667 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mathematica
--rw-r--r--   0 runner    (1001) docker     (122)      422 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/matroska
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mcrypt
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/measure
--rw-r--r--   0 runner    (1001) docker     (122)      424 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mercurial
--rw-r--r--   0 runner    (1001) docker     (122)      337 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/metastore
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/meteorological
--rw-r--r--   0 runner    (1001) docker     (122)      741 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/microfocus
--rw-r--r--   0 runner    (1001) docker     (122)      280 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mime
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mips
--rw-r--r--   0 runner    (1001) docker     (122)      258 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mirage
--rw-r--r--   0 runner    (1001) docker     (122)     3227 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/misctools
--rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mkid
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mlssa
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mmdf
--rw-r--r--   0 runner    (1001) docker     (122)     3445 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/modem
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/modulefile
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/motorola
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mozilla
--rw-r--r--   0 runner    (1001) docker     (122)    76709 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/msdos
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/msooxml
--rw-r--r--   0 runner    (1001) docker     (122)    10148 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/msvc
--rw-r--r--   0 runner    (1001) docker     (122)     9532 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/msx
--rw-r--r--   0 runner    (1001) docker     (122)      781 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/mup
--rw-r--r--   0 runner    (1001) docker     (122)      546 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/music
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/nasa
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/natinst
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ncr
--rw-r--r--   0 runner    (1001) docker     (122)      373 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/neko
--rw-r--r--   0 runner    (1001) docker     (122)     7541 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/netbsd
--rw-r--r--   0 runner    (1001) docker     (122)      902 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/netscape
--rw-r--r--   0 runner    (1001) docker     (122)      412 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/netware
--rw-r--r--   0 runner    (1001) docker     (122)      555 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/news
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/nifty
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/nim-lang
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/nitpicker
--rw-r--r--   0 runner    (1001) docker     (122)      401 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/numpy
--rw-r--r--   0 runner    (1001) docker     (122)      471 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/oasis
--rw-r--r--   0 runner    (1001) docker     (122)      542 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ocaml
--rw-r--r--   0 runner    (1001) docker     (122)      323 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/octave
--rw-r--r--   0 runner    (1001) docker     (122)    27816 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ole2compounddocs
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/olf
--rw-r--r--   0 runner    (1001) docker     (122)      616 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/openfst
--rw-r--r--   0 runner    (1001) docker     (122)      704 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/opentimestamps
--rw-r--r--   0 runner    (1001) docker     (122)      536 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/oric
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/os2
--rw-r--r--   0 runner    (1001) docker     (122)     1923 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/os400
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/os9
--rw-r--r--   0 runner    (1001) docker     (122)      254 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/osf1
--rw-r--r--   0 runner    (1001) docker     (122)     5317 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/palm
--rw-r--r--   0 runner    (1001) docker     (122)      384 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/parix
--rw-r--r--   0 runner    (1001) docker     (122)      764 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/parrot
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pascal
--rw-r--r--   0 runner    (1001) docker     (122)      444 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pbf
--rw-r--r--   0 runner    (1001) docker     (122)      258 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pbm
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pc88
--rw-r--r--   0 runner    (1001) docker     (122)     2790 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pc98
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pci_ids
--rw-r--r--   0 runner    (1001) docker     (122)      355 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pcjr
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pdp
--rw-r--r--   0 runner    (1001) docker     (122)     3601 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/perl
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pgf
--rw-r--r--   0 runner    (1001) docker     (122)    13995 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pgp
--rw-r--r--   0 runner    (1001) docker     (122)    13416 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pgp-binary-keys
--rw-r--r--   0 runner    (1001) docker     (122)      297 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pkgadd
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/plan9
--rw-r--r--   0 runner    (1001) docker     (122)      550 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/plus5
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pmem
--rw-r--r--   0 runner    (1001) docker     (122)      195 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/polyfile_zip
--rw-r--r--   0 runner    (1001) docker     (122)      744 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/polyml
--rw-r--r--   0 runner    (1001) docker     (122)     5969 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/printer
--rw-r--r--   0 runner    (1001) docker     (122)      389 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/project
--rw-r--r--   0 runner    (1001) docker     (122)      483 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/psdbms
--rw-r--r--   0 runner    (1001) docker     (122)      559 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/psl
--rw-r--r--   0 runner    (1001) docker     (122)      370 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pulsar
--rw-r--r--   0 runner    (1001) docker     (122)      588 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/puzzle
--rw-r--r--   0 runner    (1001) docker     (122)      669 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pwsafe
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/pyramid
--rw-r--r--   0 runner    (1001) docker     (122)    11537 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/python
--rw-r--r--   0 runner    (1001) docker     (122)      745 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/qt
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/revision
--rw-r--r--   0 runner    (1001) docker     (122)    33173 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/riff
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rinex
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ringdove
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rpi
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rpm
--rw-r--r--   0 runner    (1001) docker     (122)      349 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rpmsg
--rw-r--r--   0 runner    (1001) docker     (122)      385 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rst
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/rtf
--rw-r--r--   0 runner    (1001) docker     (122)     1905 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ruby
--rw-r--r--   0 runner    (1001) docker     (122)      245 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sc
--rw-r--r--   0 runner    (1001) docker     (122)      899 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sccs
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/scientific
--rw-r--r--   0 runner    (1001) docker     (122)      366 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/securitycerts
--rw-r--r--   0 runner    (1001) docker     (122)      806 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/selinux
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sendmail
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sequent
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sereal
--rw-r--r--   0 runner    (1001) docker     (122)     4171 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sgi
--rw-r--r--   0 runner    (1001) docker     (122)     4644 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sgml
--rw-r--r--   0 runner    (1001) docker     (122)      816 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sharc
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sinclair
--rw-r--r--   0 runner    (1001) docker     (122)      471 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sisu
--rw-r--r--   0 runner    (1001) docker     (122)      258 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sketch
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/smalltalk
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/smile
--rw-r--r--   0 runner    (1001) docker     (122)    17529 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sniffer
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/softquad
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sosi
--rw-r--r--   0 runner    (1001) docker     (122)      600 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/spec
--rw-r--r--   0 runner    (1001) docker     (122)     3240 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/spectrum
--rw-r--r--   0 runner    (1001) docker     (122)     9624 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sql
--rw-r--r--   0 runner    (1001) docker     (122)     1437 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ssh
--rw-r--r--   0 runner    (1001) docker     (122)      929 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ssl
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/statistics
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/subtitle
--rw-r--r--   0 runner    (1001) docker     (122)     4799 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sun
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sylk
--rw-r--r--   0 runner    (1001) docker     (122)      915 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/symbos
--rw-r--r--   0 runner    (1001) docker     (122)    16247 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/sysex
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/tcl
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/teapot
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/terminfo
--rw-r--r--   0 runner    (1001) docker     (122)     4664 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/tex
--rw-r--r--   0 runner    (1001) docker     (122)      262 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/tgif
--rw-r--r--   0 runner    (1001) docker     (122)     7733 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/ti-8x
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/timezone
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/tplink
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/troff
--rw-r--r--   0 runner    (1001) docker     (122)      306 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/tuxedo
--rw-r--r--   0 runner    (1001) docker     (122)      286 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/typeset
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/uf2
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/unicode
--rw-r--r--   0 runner    (1001) docker     (122)      402 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/unisig
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/unknown
--rw-r--r--   0 runner    (1001) docker     (122)      568 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/usd
--rw-r--r--   0 runner    (1001) docker     (122)      469 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/uterus
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/uuencode
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vacuum-cleaner
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/varied.out
--rw-r--r--   0 runner    (1001) docker     (122)      580 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/varied.script
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vax
--rw-r--r--   0 runner    (1001) docker     (122)      759 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vicar
--rw-r--r--   0 runner    (1001) docker     (122)    11929 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/virtual
--rw-r--r--   0 runner    (1001) docker     (122)      524 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/virtutech
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/visx
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vms
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vmware
--rw-r--r--   0 runner    (1001) docker     (122)     6112 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vorbis
--rw-r--r--   0 runner    (1001) docker     (122)      489 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/vxl
--rw-r--r--   0 runner    (1001) docker     (122)      596 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/warc
--rw-r--r--   0 runner    (1001) docker     (122)      629 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/weak
--rw-r--r--   0 runner    (1001) docker     (122)      522 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/web
--rw-r--r--   0 runner    (1001) docker     (122)      671 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/webassembly
--rw-r--r--   0 runner    (1001) docker     (122)    54880 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/windows
--rw-r--r--   0 runner    (1001) docker     (122)      295 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/wireless
--rw-r--r--   0 runner    (1001) docker     (122)    20403 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/wordprocessors
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/wsdl
--rw-r--r--   0 runner    (1001) docker     (122)      743 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/x68000
--rw-r--r--   0 runner    (1001) docker     (122)      548 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/xdelta
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/xenix
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/xilinx
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/xo65
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/xwindows
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/yara
--rw-r--r--   0 runner    (1001) docker     (122)     2423 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/zfs
--rw-r--r--   0 runner    (1001) docker     (122)      451 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/zilog
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/zip
--rw-r--r--   0 runner    (1001) docker     (122)      613 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/magic_defs/zyxel
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/nes.py
--rw-r--r--   0 runner    (1001) docker     (122)      587 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/nitf.py
--rw-r--r--   0 runner    (1001) docker     (122)    38219 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    14414 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/polyfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/profiling.py
--rw-r--r--   0 runner    (1001) docker     (122)    24055 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/repl.py
--rw-r--r--   0 runner    (1001) docker     (122)     9837 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     8275 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/structmatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     9484 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.884999 polyfile-0.5.0/polyfile/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     6000 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/templates/download.js
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/templates/hexdump.css
--rw-r--r--   0 runner    (1001) docker     (122)    22917 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/templates/hexdump.js
--rw-r--r--   0 runner    (1001) docker     (122)    88145 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/templates/jquery-3.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/wildcards.py
--rw-r--r--   0 runner    (1001) docker     (122)     6847 2022-11-22 16:00:01.000000 polyfile-0.5.0/polyfile/zipmatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.816997 polyfile-0.5.0/polyfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17489 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17412 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-22 16:00:27.000000 polyfile-0.5.0/polyfile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 16:00:27.884999 polyfile-0.5.0/polymerge/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2022-11-22 16:00:01.000000 polyfile-0.5.0/polymerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13261 2022-11-22 16:00:01.000000 polyfile-0.5.0/polymerge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4293 2022-11-22 16:00:01.000000 polyfile-0.5.0/polymerge/cfg.py
--rw-r--r--   0 runner    (1001) docker     (122)     8357 2022-11-22 16:00:01.000000 polyfile-0.5.0/polymerge/polymerge.py
--rw-r--r--   0 runner    (1001) docker     (122)     6866 2022-11-22 16:00:01.000000 polyfile-0.5.0/polymerge/polytracker.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 16:00:27.884999 polyfile-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2022-11-22 16:00:01.000000 polyfile-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.843814 polyfile-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-10 14:56:37.000000 polyfile-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-05-10 14:56:52.843814 polyfile-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-05-10 14:56:37.000000 polyfile-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.767814 polyfile-0.5.1/polyfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17685 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42407 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.767814 polyfile-0.5.1/polyfile/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/defacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/http_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/http/structured_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/jpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.767814 polyfile-0.5.1/polyfile/kaitai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5707 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.791814 polyfile-0.5.1/polyfile/kaitai/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/aix_utmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/allegro_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/andes_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_asus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_huawei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_qcom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_nanoapp_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_opengl_shaders_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/android_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/apm_partition_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/apple_single_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/asn1_der.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/au.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/avantes_roh60.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/avi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/bitcoin_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/blender_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37749 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/bmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/broadcom_trx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/bson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/btrfs_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/bytes_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/chrome_pak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/code_6502.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/compressed_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/cpio_old_le.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/cramfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/creative_voice_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35086 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_variable_length_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49963 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197752 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dime_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24113 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dns_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30308 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/doom_wad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dos_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dos_mz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ds_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/dune_2_pak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/edid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/efivar_signature_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108372 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ethernet_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30390 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27149 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ext2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/fallout2_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/fallout_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30681 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/fasttracker_xm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ftl_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/genmidi_op2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24355 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gettext_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gimp_brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/glibc_utmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gltf_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/google_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gpt_partition_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gran_turismo_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/grub2_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/hashcat_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/hccap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/hccapx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/heaps_pak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/heroes_of_might_and_magic_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/heroes_of_might_and_magic_bmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/icmp_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/id3v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/id3v2_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/id3v2_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ipv4_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ipv6_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27743 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/iso9660.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46144 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/java_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/luks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/lvm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/lzh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23884 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mac_os_resource_snd.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148271 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mach_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mach_o_fat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/magicavoxel_vox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mbr_partition_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48729 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_cfb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_network_monitor_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39086 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32672 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mifare_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/minecraft_nbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/monomakh_sapr_chg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mozilla_mar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/mp4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69659 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/nitf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66870 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/nt_mdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/nt_mdt_pal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ogg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46147 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/openpgp_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/packet_ppi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/pcf_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/pcx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/pcx_dcx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/phar_without_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24615 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/php_serialized_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/png.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/protocol_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/psx_tim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30279 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/python_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/python_pyc_27.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/quake_mdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/quake_pak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24688 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/quicktime_mov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/rar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29723 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33901 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/renderware_binary_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/resource_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/riff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/rpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25558 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/rtcp_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/rtp_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/rtpdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ruby_marshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/s3m.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/saints_row_2_vpp_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/shapefile_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45337 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/shapefile_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/some_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18941 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/specpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22295 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ssh_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/standard_midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/sudoers_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/swf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/systemd_journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/tcp_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/tga.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/tls_client_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/tr_dos_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/tsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104490 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/udp_datagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/uefi_te.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/uimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/utf8_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21194 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vfat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vlq_base128_be.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vlq_base128_le.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vmware_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/vp8_ivf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/warcraft_2_pud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42097 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_evt_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_lnk_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27119 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_minidump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_resource_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_shell_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/windows_systemtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/wmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/xar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/xwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34076 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/zisofs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitai/parsers/zx_spectrum_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/kaitaimatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/languagematcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115065 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.843814 polyfile-0.5.1/polyfile/magic_defs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/acorn
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/adi
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/adventure
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/aes
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/algol68
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/allegro
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/alliant
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/alpha
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/amanda
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/amigaos
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/android
+-rw-r--r--   0 runner    (1001) docker     (123)    51507 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/animation
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/aout
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/apache
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/apl
+-rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/apple
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/application
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/applix
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/apt
+-rw-r--r--   0 runner    (1001) docker     (123)    73451 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/archive
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/aria
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/arm
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/asf
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/assembler
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/asterix
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/att3b
+-rw-r--r--   0 runner    (1001) docker     (123)    40257 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/audio
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/avm
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/basis
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/beetle
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ber
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bflt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bhl
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bioinformatics
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/biosig
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/blackberry
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/blcr
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/blender
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/blit
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bm
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bout
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bsdi
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bsi
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/btsnoop
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/burp
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/bytecode
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/c-lang
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/c64
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cad
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cafebabe
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cbor
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ccf
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cddb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/chord
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cisco
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/citrus
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/clarion
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/claris
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/clipper
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/clojure
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/coff
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/commands
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/communications
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/compress
+-rw-r--r--   0 runner    (1001) docker     (123)    41408 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/console
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/convex
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/coverage
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cracklib
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/crypto
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/csv
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ctags
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ctf
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cubemap
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/cups
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dact
+-rw-r--r--   0 runner    (1001) docker     (123)    31552 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/database
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dataone
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dbpf
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/der
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/diamond
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/diff
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/digital
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dolby
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dsf
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dump
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/dyadic
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ebml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/edid
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/editors
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/efi
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/elf
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/encore
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/epoc
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/erlang
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/espressif
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/esri
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/etf
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/fcs
+-rw-r--r--   0 runner    (1001) docker     (123)   103933 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/filesystems
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/finger
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/firmware
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/flash
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/flif
+-rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/fonts
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/forth
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/fortran
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/frame
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/freebsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/fsav
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/fusecompress
+-rw-r--r--   0 runner    (1001) docker     (123)    20686 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/games
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gcc
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gconv
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gentoo
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/geo
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/geos
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gimp
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/git
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/glibc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gnome
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gnu
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gnumeric
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gpt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/grace
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/graphviz
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/gringotts
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/guile
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/hardware
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/hitachi-sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/hp
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/human68k
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ibm370
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ibm6000
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/icc
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/iff
+-rw-r--r--   0 runner    (1001) docker     (123)   145544 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/images
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/inform
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/intel
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/interleaf
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/island
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ispell
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/isz
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/java
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/javascript
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/json
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/karma
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/kde
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/keepass
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/kerberos
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/kicad
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/kml
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lecter
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lex
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lif
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/linux
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lisp
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/llvm
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/locoscript
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/luks
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/m4
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mach
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/macintosh
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/macos
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/magic
+-rw-r--r--   0 runner    (1001) docker     (123)  6649560 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/magic.mgc
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mail.news
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/make
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/map
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/maple
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/marc21
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mathcad
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mathematica
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/matroska
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mcrypt
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/measure
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mercurial
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/metastore
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/meteorological
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/microfocus
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mime
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mips
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mirage
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/misctools
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mkid
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mlssa
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mmdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/modem
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/modulefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/motorola
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mozilla
+-rw-r--r--   0 runner    (1001) docker     (123)    76709 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/msdos
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/msooxml
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/msvc
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/msx
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/mup
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/music
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/nasa
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/natinst
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ncr
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/neko
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/netbsd
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/netscape
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/netware
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/news
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/nifty
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/nim-lang
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/nitpicker
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/numpy
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/oasis
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ocaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/octave
+-rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ole2compounddocs
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/olf
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/openfst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/opentimestamps
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/oric
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/os2
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/os400
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/os9
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/osf1
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/palm
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/parix
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/parrot
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pascal
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pbf
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pbm
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pc88
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pc98
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pci_ids
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pcjr
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pdp
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/perl
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pgf
+-rw-r--r--   0 runner    (1001) docker     (123)    13995 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pgp
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pgp-binary-keys
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pkgadd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/plan9
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/plus5
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pmem
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/polyfile_zip
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/polyml
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/printer
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/project
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/psdbms
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/psl
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pulsar
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/puzzle
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pwsafe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/pyramid
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/python
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/qt
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/revision
+-rw-r--r--   0 runner    (1001) docker     (123)    33173 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/riff
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rinex
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ringdove
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rpi
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rpm
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rpmsg
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/rtf
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sc
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sccs
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/scientific
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/securitycerts
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/selinux
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sendmail
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sequent
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sereal
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sgi
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sgml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sharc
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sinclair
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sisu
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sketch
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/smalltalk
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/smile
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sniffer
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/softquad
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sosi
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/spec
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/spectrum
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ssh
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ssl
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/statistics
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/subtitle
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sun
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sylk
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/symbos
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/sysex
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/teapot
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/terminfo
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/tex
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/tgif
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/ti-8x
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/timezone
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/tplink
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/troff
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/tuxedo
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/typeset
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/uf2
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/unicode
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/unisig
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/unknown
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/usd
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/uterus
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/uuencode
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vacuum-cleaner
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/varied.out
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/varied.script
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vax
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vicar
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/virtual
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/virtutech
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/visx
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vms
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vmware
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vorbis
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/vxl
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/warc
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/weak
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/web
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/webassembly
+-rw-r--r--   0 runner    (1001) docker     (123)    54880 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/windows
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/wireless
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/wordprocessors
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/x68000
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/xdelta
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/xenix
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/xilinx
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/xo65
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/xwindows
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/yara
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/zfs
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/zilog
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/zip
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/magic_defs/zyxel
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/nes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/nitf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46929 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/polyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24132 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/structmatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.843814 polyfile-0.5.1/polyfile/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/templates/download.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/templates/hexdump.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/templates/hexdump.js
+-rw-r--r--   0 runner    (1001) docker     (123)    88145 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/templates/jquery-3.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/wildcards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-10 14:56:37.000000 polyfile-0.5.1/polyfile/zipmatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.767814 polyfile-0.5.1/polyfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 14:56:52.000000 polyfile-0.5.1/polyfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:52.843814 polyfile-0.5.1/polymerge/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 14:56:37.000000 polyfile-0.5.1/polymerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-05-10 14:56:37.000000 polyfile-0.5.1/polymerge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-10 14:56:37.000000 polyfile-0.5.1/polymerge/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-10 14:56:37.000000 polyfile-0.5.1/polymerge/polymerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-10 14:56:37.000000 polyfile-0.5.1/polymerge/polytracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:56:52.843814 polyfile-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-10 14:56:37.000000 polyfile-0.5.1/setup.py
```

### Comparing `polyfile-0.5.0/LICENSE` & `polyfile-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/PKG-INFO` & `polyfile-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfile
-Version: 0.5.0
+Version: 0.5.1
 Summary: A utility to recursively map the structure of a file.
 Home-page: https://github.com/trailofbits/polyfile
 Author: Trail of Bits
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -209,15 +209,15 @@
 matcher = MagicMatcher.parse(*list_of_paths_to_definitions)
 with open("file_to_test", "rb") as f:
     for match in matcher.match(f.read()):
         ...
 ```
 
 ### Debugging the libmagic DSL
-`libmagic` has an esoteric, poorly documented doman-specific language (DSL) for specifying its matching signatures.
+`libmagic` has an esoteric, poorly documented domain-specific language (DSL) for specifying its matching signatures.
 You can read the minimal and—as we have discovered in our cleanroom implementation—_incomplete_ documentation by running
 `man 5 magic`. PolyFile implements an interactive debugger for stepping through the DSL specifications, modeled after
 GDB. You can enter this debugger by passing the `--debugger` or `-db` argument to PolyFile. It is useful for both
 implementing new `libmagic` DSLs, as well as figuring out why an existing DSL fails to match against a given file.
 ```console
 $ polyfile -db input_file
 PolyFile 0.3.5
```

### Comparing `polyfile-0.5.0/README.md` & `polyfile-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 matcher = MagicMatcher.parse(*list_of_paths_to_definitions)
 with open("file_to_test", "rb") as f:
     for match in matcher.match(f.read()):
         ...
 ```
 
 ### Debugging the libmagic DSL
-`libmagic` has an esoteric, poorly documented doman-specific language (DSL) for specifying its matching signatures.
+`libmagic` has an esoteric, poorly documented domain-specific language (DSL) for specifying its matching signatures.
 You can read the minimal and—as we have discovered in our cleanroom implementation—_incomplete_ documentation by running
 `man 5 magic`. PolyFile implements an interactive debugger for stepping through the DSL specifications, modeled after
 GDB. You can enter this debugger by passing the `--debugger` or `-db` argument to PolyFile. It is useful for both
 implementing new `libmagic` DSLs, as well as figuring out why an existing DSL fails to match against a given file.
 ```console
 $ polyfile -db input_file
 PolyFile 0.3.5
```

### Comparing `polyfile-0.5.0/polyfile/__main__.py` & `polyfile-0.5.1/polyfile/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 def main(argv=None):
     parser = argparse.ArgumentParser(description='A utility to recursively map the structure of a file.',
                                      formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('FILE', nargs='?', default='-',
                         help='the file to analyze; pass \'-\' or omit to read from STDIN')
 
     parser.add_argument('--format', '-r', type=FormatOutput, action="append", choices=[
-        FormatOutput(f) for f in ("file", "mime", "html", "json", "sbud")
+        FormatOutput(f) for f in FormatOutput.valid_formats + ("json",)
     ], help=dedent("""PolyFile's output format
 
 Output formats are:
 file ...... the detected formats associated with the file,
             like the output of the `file` command
 mime ...... the detected MIME types associated with the file,
             like the output of the `file --mime-type` command
@@ -372,15 +372,15 @@
                         log.clear_status()
                     elif not output_format.output_to_stdout:
                         log.info(f"Saved MIME output to {output_format.output_path}")
                 elif output_format.output_format == "json" or output_format.output_format == "sbud":
                     assert needs_sbud
                     json.dump(sbud, output)
                     if not output_format.output_to_stdout:
-                        log.info(f"Saved {output_format.upper()} output to {output_format.output_path}")
+                        log.info(f"Saved {output_format.output_format.upper()} output to {output_format.output_path}")
                 elif output_format.output_format == "html":
                     assert needs_sbud
                     output.write(html.generate(file_path, sbud))
                     if not output_format.output_to_stdout:
                         log.info(f"Saved HTML output to {output_format.output_path}")
                 else:
                     # This should never happen because the output formats are constrained by argparse
```

### Comparing `polyfile-0.5.0/polyfile/arithmetic.py` & `polyfile-0.5.1/polyfile/arithmetic.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/debugger.py` & `polyfile-0.5.1/polyfile/debugger.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/expressions.py` & `polyfile-0.5.1/polyfile/expressions.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/fileutils.py` & `polyfile-0.5.1/polyfile/fileutils.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/html.py` & `polyfile-0.5.1/polyfile/html.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/iterators.py` & `polyfile-0.5.1/polyfile/iterators.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/jpeg.py` & `polyfile-0.5.1/polyfile/jpeg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/compiler.py` & `polyfile-0.5.1/polyfile/kaitai/compiler.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parser.py` & `polyfile-0.5.1/polyfile/kaitai/parser.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/aix_utmp.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/aix_utmp.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/allegro_dat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/allegro_dat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/andes_firmware.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/andes_firmware.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_asus.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_asus.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_huawei.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_huawei.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_bootldr_qcom.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_bootldr_qcom.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_dto.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_dto.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_img.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_img.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_nanoapp_header.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_nanoapp_header.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_opengl_shaders_cache.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_opengl_shaders_cache.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_sparse.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_sparse.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/android_super.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/android_super.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/apm_partition_table.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/apm_partition_table.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/apple_single_double.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/apple_single_double.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/asn1_der.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/asn1_der.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/au.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/au.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/avantes_roh60.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/avantes_roh60.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/avi.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/avi.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/bcd.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/bcd.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/bitcoin_transaction.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/bitcoin_transaction.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/blender_blend.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/blender_blend.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/bmp.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/bmp.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/broadcom_trx.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/broadcom_trx.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/bson.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/bson.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/btrfs_stream.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/btrfs_stream.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/bytes_with_io.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/bytes_with_io.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/chrome_pak.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/chrome_pak.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/code_6502.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/code_6502.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/compressed_resource.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/compressed_resource.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/cpio_old_le.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/cpio_old_le.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/cramfs.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/cramfs.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/creative_voice_file.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/creative_voice_file.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dbf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dbf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_0.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_0.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_1.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_1.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_2.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_2.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dcmp_variable_length_integer.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dcmp_variable_length_integer.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dex.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dex.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dicom.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dicom.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dime_message.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dime_message.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dns_packet.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dns_packet.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/doom_wad.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/doom_wad.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dos_datetime.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dos_datetime.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dos_mz.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dos_mz.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ds_store.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ds_store.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dtb.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dtb.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/dune_2_pak.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/dune_2_pak.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/edid.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/edid.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/efivar_signature_list.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/efivar_signature_list.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/elf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/elf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ethernet_frame.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ethernet_frame.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/exif.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/exif.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ext2.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ext2.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/fallout2_dat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/fallout2_dat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/fallout_dat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/fallout_dat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/fasttracker_xm_module.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/fasttracker_xm_module.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ftl_dat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ftl_dat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/genmidi_op2.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/genmidi_op2.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gettext_mo.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gettext_mo.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gif.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gif.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gimp_brush.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gimp_brush.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/glibc_utmp.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/glibc_utmp.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gltf_binary.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gltf_binary.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/google_protobuf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/google_protobuf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gpt_partition_table.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gpt_partition_table.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gran_turismo_vol.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gran_turismo_vol.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/grub2_font.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/grub2_font.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/gzip.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/gzip.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/hashcat_restore.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/hashcat_restore.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/hccap.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/hccap.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/hccapx.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/hccapx.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/heaps_pak.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/heaps_pak.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/heroes_of_might_and_magic_agg.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/heroes_of_might_and_magic_agg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/heroes_of_might_and_magic_bmp.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/heroes_of_might_and_magic_bmp.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/icmp_packet.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/icmp_packet.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ico.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ico.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/id3v1_1.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/id3v1_1.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/id3v2_3.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/id3v2_3.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/id3v2_4.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/id3v2_4.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ines.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ines.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ipv4_packet.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ipv4_packet.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ipv6_packet.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ipv6_packet.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/iso9660.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/iso9660.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/java_class.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/java_class.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/jpeg.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/jpeg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/luks.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/luks.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/lvm2.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/lvm2.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/lzh.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/lzh.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mac_os_resource_snd.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mac_os_resource_snd.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mach_o.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mach_o.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mach_o_fat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mach_o_fat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/magicavoxel_vox.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/magicavoxel_vox.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/manifest.json` & `polyfile-0.5.1/polyfile/kaitai/parsers/manifest.json`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mbr_partition_table.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mbr_partition_table.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mcap.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mcap.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_cfb.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_cfb.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_network_monitor_v2.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_network_monitor_v2.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/microsoft_pe.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/microsoft_pe.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mifare_classic.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mifare_classic.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/minecraft_nbt.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/minecraft_nbt.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/monomakh_sapr_chg.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/monomakh_sapr_chg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mozilla_mar.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mozilla_mar.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/mp4.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/mp4.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/msgpack.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/msgpack.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/nitf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/nitf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/nt_mdt.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/nt_mdt.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/nt_mdt_pal.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/nt_mdt_pal.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ogg.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ogg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/openpgp_message.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/openpgp_message.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/packet_ppi.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/packet_ppi.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/pcap.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/pcap.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/pcf_font.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/pcf_font.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/pcx.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/pcx.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/pcx_dcx.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/pcx_dcx.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/phar_without_stub.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/phar_without_stub.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/php_serialized_value.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/php_serialized_value.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/png.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/png.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/protocol_body.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/protocol_body.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/psx_tim.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/psx_tim.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/python_pickle.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/python_pickle.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/python_pyc_27.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/python_pyc_27.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/quake_mdl.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/quake_mdl.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/quake_pak.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/quake_pak.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/quicktime_mov.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/quicktime_mov.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/rar.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/rar.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/regf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/regf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/renderware_binary_stream.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/renderware_binary_stream.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/resource_fork.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/resource_fork.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/riff.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/riff.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/rpm.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/rpm.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/rtcp_payload.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/rtcp_payload.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/rtp_packet.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/rtp_packet.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/rtpdump.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/rtpdump.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ruby_marshal.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ruby_marshal.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/s3m.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/s3m.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/saints_row_2_vpp_pc.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/saints_row_2_vpp_pc.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/shapefile_index.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/shapefile_index.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/shapefile_main.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/shapefile_main.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/some_ip.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/some_ip.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_container.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_container.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd_entries.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd_entries.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/some_ip_sd_options.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/some_ip_sd_options.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/specpr.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/specpr.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/sqlite3.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/sqlite3.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ssh_public_key.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ssh_public_key.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/standard_midi_file.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/standard_midi_file.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/stl.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/stl.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/sudoers_ts.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/sudoers_ts.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/swf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/swf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/systemd_journal.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/systemd_journal.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/tcp_segment.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/tcp_segment.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/tga.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/tga.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/tls_client_hello.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/tls_client_hello.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/tr_dos_image.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/tr_dos_image.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/tsm.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/tsm.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/ttf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/ttf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/udp_datagram.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/udp_datagram.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/uefi_te.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/uefi_te.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/uimage.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/uimage.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/utf8_string.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/utf8_string.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vdi.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vdi.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vfat.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vfat.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vlq_base128_be.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vlq_base128_be.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vlq_base128_le.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vlq_base128_le.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vmware_vmdk.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vmware_vmdk.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/vp8_ivf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/vp8_ivf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/warcraft_2_pud.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/warcraft_2_pud.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/wav.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/wav.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/websocket.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/websocket.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_evt_log.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_evt_log.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_lnk_file.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_lnk_file.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_minidump.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_minidump.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_resource_file.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_resource_file.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_shell_items.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_shell_items.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/windows_systemtime.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/windows_systemtime.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/wmf.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/wmf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/xar.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/xar.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/xwd.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/xwd.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/zip.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/zip.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/zisofs.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/zisofs.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitai/parsers/zx_spectrum_tap.py` & `polyfile-0.5.1/polyfile/kaitai/parsers/zx_spectrum_tap.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/kaitaimatcher.py` & `polyfile-0.5.1/polyfile/kaitaimatcher.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/languagematcher.py` & `polyfile-0.5.1/polyfile/languagematcher.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/logger.py` & `polyfile-0.5.1/polyfile/logger.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic.py` & `polyfile-0.5.1/polyfile/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -2392,15 +2392,15 @@
         return MatchedTest(self, offset=absolute_offset, length=len(data) - absolute_offset, parent=parent_match,
                            value=data)
 
 
 TEST_PATTERN: Pattern[str] = re.compile(
     r"^(?P<level>[>]*)(?P<offset>[^\s!][^\s]*)\s+(?P<data_type>[^\s]+)\s+(?P<remainder>.+)$"
 )
-MIME_PATTERN: Pattern[str] = re.compile(r"^!:mime\s+([^\s]+)\s*(#.*)?$")
+MIME_PATTERN: Pattern[str] = re.compile(r"^!:mime\s+([^#]+?)\s*(#.*)?$")
 EXTENSION_PATTERN: Pattern[str] = re.compile(r"^!:ext\s+([^\s]+)\s*(#.*)?$")
 
 
 def _split_with_escapes(text: str) -> Tuple[str, str]:
     first_length = 0
     escaped = False
     delimiter_length = 1
```

### Comparing `polyfile-0.5.0/polyfile/magic_defs/COPYING` & `polyfile-0.5.1/polyfile/magic_defs/COPYING`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/acorn` & `polyfile-0.5.1/polyfile/magic_defs/acorn`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/adventure` & `polyfile-0.5.1/polyfile/magic_defs/adventure`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/aes` & `polyfile-0.5.1/polyfile/magic_defs/aes`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/algol68` & `polyfile-0.5.1/polyfile/magic_defs/algol68`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/alliant` & `polyfile-0.5.1/polyfile/magic_defs/alliant`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/alpha` & `polyfile-0.5.1/polyfile/magic_defs/alpha`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/amigaos` & `polyfile-0.5.1/polyfile/magic_defs/amigaos`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/android` & `polyfile-0.5.1/polyfile/magic_defs/android`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/animation` & `polyfile-0.5.1/polyfile/magic_defs/animation`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/aout` & `polyfile-0.5.1/polyfile/magic_defs/aout`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/apache` & `polyfile-0.5.1/polyfile/magic_defs/apache`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/apple` & `polyfile-0.5.1/polyfile/magic_defs/apple`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/apt` & `polyfile-0.5.1/polyfile/magic_defs/apt`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/archive` & `polyfile-0.5.1/polyfile/magic_defs/archive`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/aria` & `polyfile-0.5.1/polyfile/magic_defs/aria`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/arm` & `polyfile-0.5.1/polyfile/magic_defs/arm`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/asf` & `polyfile-0.5.1/polyfile/magic_defs/asf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/assembler` & `polyfile-0.5.1/polyfile/magic_defs/assembler`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/asterix` & `polyfile-0.5.1/polyfile/magic_defs/asterix`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/att3b` & `polyfile-0.5.1/polyfile/magic_defs/att3b`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/audio` & `polyfile-0.5.1/polyfile/magic_defs/audio`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/avm` & `polyfile-0.5.1/polyfile/magic_defs/avm`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/basis` & `polyfile-0.5.1/polyfile/magic_defs/basis`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ber` & `polyfile-0.5.1/polyfile/magic_defs/ber`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/bioinformatics` & `polyfile-0.5.1/polyfile/magic_defs/bioinformatics`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/biosig` & `polyfile-0.5.1/polyfile/magic_defs/biosig`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/blcr` & `polyfile-0.5.1/polyfile/magic_defs/blcr`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/blender` & `polyfile-0.5.1/polyfile/magic_defs/blender`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/blit` & `polyfile-0.5.1/polyfile/magic_defs/blit`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/bsdi` & `polyfile-0.5.1/polyfile/magic_defs/bsdi`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/bytecode` & `polyfile-0.5.1/polyfile/magic_defs/bytecode`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/c-lang` & `polyfile-0.5.1/polyfile/magic_defs/c-lang`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/c64` & `polyfile-0.5.1/polyfile/magic_defs/c64`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/cad` & `polyfile-0.5.1/polyfile/magic_defs/cad`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/cafebabe` & `polyfile-0.5.1/polyfile/magic_defs/cafebabe`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/cbor` & `polyfile-0.5.1/polyfile/magic_defs/cbor`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ccf` & `polyfile-0.5.1/polyfile/magic_defs/ccf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/chord` & `polyfile-0.5.1/polyfile/magic_defs/chord`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/clarion` & `polyfile-0.5.1/polyfile/magic_defs/clarion`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/claris` & `polyfile-0.5.1/polyfile/magic_defs/claris`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/clipper` & `polyfile-0.5.1/polyfile/magic_defs/clipper`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/clojure` & `polyfile-0.5.1/polyfile/magic_defs/clojure`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/coff` & `polyfile-0.5.1/polyfile/magic_defs/coff`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/commands` & `polyfile-0.5.1/polyfile/magic_defs/commands`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/communications` & `polyfile-0.5.1/polyfile/magic_defs/communications`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/compress` & `polyfile-0.5.1/polyfile/magic_defs/compress`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/console` & `polyfile-0.5.1/polyfile/magic_defs/console`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/convex` & `polyfile-0.5.1/polyfile/magic_defs/convex`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/coverage` & `polyfile-0.5.1/polyfile/magic_defs/coverage`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/cracklib` & `polyfile-0.5.1/polyfile/magic_defs/cracklib`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ctf` & `polyfile-0.5.1/polyfile/magic_defs/ctf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/cups` & `polyfile-0.5.1/polyfile/magic_defs/cups`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/database` & `polyfile-0.5.1/polyfile/magic_defs/database`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dataone` & `polyfile-0.5.1/polyfile/magic_defs/dataone`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dbpf` & `polyfile-0.5.1/polyfile/magic_defs/dbpf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/der` & `polyfile-0.5.1/polyfile/magic_defs/der`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dif` & `polyfile-0.5.1/polyfile/magic_defs/dif`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/diff` & `polyfile-0.5.1/polyfile/magic_defs/diff`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/digital` & `polyfile-0.5.1/polyfile/magic_defs/digital`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dolby` & `polyfile-0.5.1/polyfile/magic_defs/dolby`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dsf` & `polyfile-0.5.1/polyfile/magic_defs/dsf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dump` & `polyfile-0.5.1/polyfile/magic_defs/dump`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/dyadic` & `polyfile-0.5.1/polyfile/magic_defs/dyadic`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/editors` & `polyfile-0.5.1/polyfile/magic_defs/editors`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/efi` & `polyfile-0.5.1/polyfile/magic_defs/efi`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/elf` & `polyfile-0.5.1/polyfile/magic_defs/elf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/encore` & `polyfile-0.5.1/polyfile/magic_defs/encore`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/epoc` & `polyfile-0.5.1/polyfile/magic_defs/epoc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/erlang` & `polyfile-0.5.1/polyfile/magic_defs/erlang`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/espressif` & `polyfile-0.5.1/polyfile/magic_defs/espressif`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/esri` & `polyfile-0.5.1/polyfile/magic_defs/esri`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/etf` & `polyfile-0.5.1/polyfile/magic_defs/etf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/fcs` & `polyfile-0.5.1/polyfile/magic_defs/fcs`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/filesystems` & `polyfile-0.5.1/polyfile/magic_defs/filesystems`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/firmware` & `polyfile-0.5.1/polyfile/magic_defs/firmware`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/flash` & `polyfile-0.5.1/polyfile/magic_defs/flash`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/flif` & `polyfile-0.5.1/polyfile/magic_defs/flif`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/fonts` & `polyfile-0.5.1/polyfile/magic_defs/fonts`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/forth` & `polyfile-0.5.1/polyfile/magic_defs/forth`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/frame` & `polyfile-0.5.1/polyfile/magic_defs/frame`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/freebsd` & `polyfile-0.5.1/polyfile/magic_defs/freebsd`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/fsav` & `polyfile-0.5.1/polyfile/magic_defs/fsav`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/games` & `polyfile-0.5.1/polyfile/magic_defs/games`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gentoo` & `polyfile-0.5.1/polyfile/magic_defs/gentoo`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/geo` & `polyfile-0.5.1/polyfile/magic_defs/geo`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/geos` & `polyfile-0.5.1/polyfile/magic_defs/geos`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gimp` & `polyfile-0.5.1/polyfile/magic_defs/gimp`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/glibc` & `polyfile-0.5.1/polyfile/magic_defs/glibc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gnome` & `polyfile-0.5.1/polyfile/magic_defs/gnome`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gnu` & `polyfile-0.5.1/polyfile/magic_defs/gnu`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gpt` & `polyfile-0.5.1/polyfile/magic_defs/gpt`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gpu` & `polyfile-0.5.1/polyfile/magic_defs/gpu`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/grace` & `polyfile-0.5.1/polyfile/magic_defs/grace`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/graphviz` & `polyfile-0.5.1/polyfile/magic_defs/graphviz`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/gringotts` & `polyfile-0.5.1/polyfile/magic_defs/gringotts`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/hitachi-sh` & `polyfile-0.5.1/polyfile/magic_defs/hitachi-sh`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/hp` & `polyfile-0.5.1/polyfile/magic_defs/hp`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/human68k` & `polyfile-0.5.1/polyfile/magic_defs/human68k`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ibm370` & `polyfile-0.5.1/polyfile/magic_defs/ibm370`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ibm6000` & `polyfile-0.5.1/polyfile/magic_defs/ibm6000`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/icc` & `polyfile-0.5.1/polyfile/magic_defs/icc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/iff` & `polyfile-0.5.1/polyfile/magic_defs/iff`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/images` & `polyfile-0.5.1/polyfile/magic_defs/images`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/intel` & `polyfile-0.5.1/polyfile/magic_defs/intel`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ispell` & `polyfile-0.5.1/polyfile/magic_defs/ispell`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/isz` & `polyfile-0.5.1/polyfile/magic_defs/isz`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/java` & `polyfile-0.5.1/polyfile/magic_defs/java`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/javascript` & `polyfile-0.5.1/polyfile/magic_defs/javascript`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/jpeg` & `polyfile-0.5.1/polyfile/magic_defs/jpeg`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/keepass` & `polyfile-0.5.1/polyfile/magic_defs/keepass`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/kerberos` & `polyfile-0.5.1/polyfile/magic_defs/kerberos`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/kicad` & `polyfile-0.5.1/polyfile/magic_defs/kicad`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/kml` & `polyfile-0.5.1/polyfile/magic_defs/kml`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/lammps` & `polyfile-0.5.1/polyfile/magic_defs/lammps`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/lex` & `polyfile-0.5.1/polyfile/magic_defs/lex`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/lif` & `polyfile-0.5.1/polyfile/magic_defs/lif`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/linux` & `polyfile-0.5.1/polyfile/magic_defs/linux`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/lisp` & `polyfile-0.5.1/polyfile/magic_defs/lisp`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/llvm` & `polyfile-0.5.1/polyfile/magic_defs/llvm`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/locoscript` & `polyfile-0.5.1/polyfile/magic_defs/locoscript`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/lua` & `polyfile-0.5.1/polyfile/magic_defs/lua`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/luks` & `polyfile-0.5.1/polyfile/magic_defs/luks`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mach` & `polyfile-0.5.1/polyfile/magic_defs/mach`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/macintosh` & `polyfile-0.5.1/polyfile/magic_defs/macintosh`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/magic.mgc` & `polyfile-0.5.1/polyfile/magic_defs/magic.mgc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mail.news` & `polyfile-0.5.1/polyfile/magic_defs/mail.news`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/make` & `polyfile-0.5.1/polyfile/magic_defs/make`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/map` & `polyfile-0.5.1/polyfile/magic_defs/map`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/maple` & `polyfile-0.5.1/polyfile/magic_defs/maple`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/marc21` & `polyfile-0.5.1/polyfile/magic_defs/marc21`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mathematica` & `polyfile-0.5.1/polyfile/magic_defs/mathematica`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mcrypt` & `polyfile-0.5.1/polyfile/magic_defs/mcrypt`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/measure` & `polyfile-0.5.1/polyfile/magic_defs/measure`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/meteorological` & `polyfile-0.5.1/polyfile/magic_defs/meteorological`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/microfocus` & `polyfile-0.5.1/polyfile/magic_defs/microfocus`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mips` & `polyfile-0.5.1/polyfile/magic_defs/mips`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/misctools` & `polyfile-0.5.1/polyfile/magic_defs/misctools`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/modem` & `polyfile-0.5.1/polyfile/magic_defs/modem`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/motorola` & `polyfile-0.5.1/polyfile/magic_defs/motorola`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mozilla` & `polyfile-0.5.1/polyfile/magic_defs/mozilla`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/msdos` & `polyfile-0.5.1/polyfile/magic_defs/msdos`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/msooxml` & `polyfile-0.5.1/polyfile/magic_defs/msooxml`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/msvc` & `polyfile-0.5.1/polyfile/magic_defs/msvc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/msx` & `polyfile-0.5.1/polyfile/magic_defs/msx`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/mup` & `polyfile-0.5.1/polyfile/magic_defs/mup`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/music` & `polyfile-0.5.1/polyfile/magic_defs/music`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/natinst` & `polyfile-0.5.1/polyfile/magic_defs/natinst`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ncr` & `polyfile-0.5.1/polyfile/magic_defs/ncr`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/netbsd` & `polyfile-0.5.1/polyfile/magic_defs/netbsd`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/netscape` & `polyfile-0.5.1/polyfile/magic_defs/netscape`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/news` & `polyfile-0.5.1/polyfile/magic_defs/news`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/nifty` & `polyfile-0.5.1/polyfile/magic_defs/nifty`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/nim-lang` & `polyfile-0.5.1/polyfile/magic_defs/nim-lang`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ocaml` & `polyfile-0.5.1/polyfile/magic_defs/ocaml`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ole2compounddocs` & `polyfile-0.5.1/polyfile/magic_defs/ole2compounddocs`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/olf` & `polyfile-0.5.1/polyfile/magic_defs/olf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/openfst` & `polyfile-0.5.1/polyfile/magic_defs/openfst`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/opentimestamps` & `polyfile-0.5.1/polyfile/magic_defs/opentimestamps`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/oric` & `polyfile-0.5.1/polyfile/magic_defs/oric`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/os2` & `polyfile-0.5.1/polyfile/magic_defs/os2`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/os400` & `polyfile-0.5.1/polyfile/magic_defs/os400`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/os9` & `polyfile-0.5.1/polyfile/magic_defs/os9`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/palm` & `polyfile-0.5.1/polyfile/magic_defs/palm`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/parrot` & `polyfile-0.5.1/polyfile/magic_defs/parrot`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pascal` & `polyfile-0.5.1/polyfile/magic_defs/pascal`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pc88` & `polyfile-0.5.1/polyfile/magic_defs/pc88`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pc98` & `polyfile-0.5.1/polyfile/magic_defs/pc98`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pci_ids` & `polyfile-0.5.1/polyfile/magic_defs/pci_ids`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pdf` & `polyfile-0.5.1/polyfile/magic_defs/pdf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pdp` & `polyfile-0.5.1/polyfile/magic_defs/pdp`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/perl` & `polyfile-0.5.1/polyfile/magic_defs/perl`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pgf` & `polyfile-0.5.1/polyfile/magic_defs/pgf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pgp` & `polyfile-0.5.1/polyfile/magic_defs/pgp`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pgp-binary-keys` & `polyfile-0.5.1/polyfile/magic_defs/pgp-binary-keys`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/plan9` & `polyfile-0.5.1/polyfile/magic_defs/plan9`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/plus5` & `polyfile-0.5.1/polyfile/magic_defs/plus5`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pmem` & `polyfile-0.5.1/polyfile/magic_defs/pmem`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/polyml` & `polyfile-0.5.1/polyfile/magic_defs/polyml`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/printer` & `polyfile-0.5.1/polyfile/magic_defs/printer`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/psl` & `polyfile-0.5.1/polyfile/magic_defs/psl`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/puzzle` & `polyfile-0.5.1/polyfile/magic_defs/puzzle`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/pwsafe` & `polyfile-0.5.1/polyfile/magic_defs/pwsafe`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/python` & `polyfile-0.5.1/polyfile/magic_defs/python`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/qt` & `polyfile-0.5.1/polyfile/magic_defs/qt`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/revision` & `polyfile-0.5.1/polyfile/magic_defs/revision`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/riff` & `polyfile-0.5.1/polyfile/magic_defs/riff`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/rinex` & `polyfile-0.5.1/polyfile/magic_defs/rinex`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ringdove` & `polyfile-0.5.1/polyfile/magic_defs/ringdove`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/rpi` & `polyfile-0.5.1/polyfile/magic_defs/rpi`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/rpm` & `polyfile-0.5.1/polyfile/magic_defs/rpm`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/rtf` & `polyfile-0.5.1/polyfile/magic_defs/rtf`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ruby` & `polyfile-0.5.1/polyfile/magic_defs/ruby`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sccs` & `polyfile-0.5.1/polyfile/magic_defs/sccs`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/scientific` & `polyfile-0.5.1/polyfile/magic_defs/scientific`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/selinux` & `polyfile-0.5.1/polyfile/magic_defs/selinux`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sendmail` & `polyfile-0.5.1/polyfile/magic_defs/sendmail`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sequent` & `polyfile-0.5.1/polyfile/magic_defs/sequent`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sereal` & `polyfile-0.5.1/polyfile/magic_defs/sereal`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sgi` & `polyfile-0.5.1/polyfile/magic_defs/sgi`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sgml` & `polyfile-0.5.1/polyfile/magic_defs/sgml`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sharc` & `polyfile-0.5.1/polyfile/magic_defs/sharc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sinclair` & `polyfile-0.5.1/polyfile/magic_defs/sinclair`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/smalltalk` & `polyfile-0.5.1/polyfile/magic_defs/smalltalk`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/smile` & `polyfile-0.5.1/polyfile/magic_defs/smile`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sniffer` & `polyfile-0.5.1/polyfile/magic_defs/sniffer`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/softquad` & `polyfile-0.5.1/polyfile/magic_defs/softquad`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sosi` & `polyfile-0.5.1/polyfile/magic_defs/sosi`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/spec` & `polyfile-0.5.1/polyfile/magic_defs/spec`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/spectrum` & `polyfile-0.5.1/polyfile/magic_defs/spectrum`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sql` & `polyfile-0.5.1/polyfile/magic_defs/sql`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ssh` & `polyfile-0.5.1/polyfile/magic_defs/ssh`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ssl` & `polyfile-0.5.1/polyfile/magic_defs/ssl`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/statistics` & `polyfile-0.5.1/polyfile/magic_defs/statistics`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/subtitle` & `polyfile-0.5.1/polyfile/magic_defs/subtitle`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sun` & `polyfile-0.5.1/polyfile/magic_defs/sun`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sylk` & `polyfile-0.5.1/polyfile/magic_defs/sylk`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/symbos` & `polyfile-0.5.1/polyfile/magic_defs/symbos`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/sysex` & `polyfile-0.5.1/polyfile/magic_defs/sysex`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/tcl` & `polyfile-0.5.1/polyfile/magic_defs/tcl`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/terminfo` & `polyfile-0.5.1/polyfile/magic_defs/terminfo`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/tex` & `polyfile-0.5.1/polyfile/magic_defs/tex`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/ti-8x` & `polyfile-0.5.1/polyfile/magic_defs/ti-8x`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/timezone` & `polyfile-0.5.1/polyfile/magic_defs/timezone`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/tplink` & `polyfile-0.5.1/polyfile/magic_defs/tplink`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/troff` & `polyfile-0.5.1/polyfile/magic_defs/troff`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/uf2` & `polyfile-0.5.1/polyfile/magic_defs/uf2`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/unicode` & `polyfile-0.5.1/polyfile/magic_defs/unicode`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/unknown` & `polyfile-0.5.1/polyfile/magic_defs/unknown`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/usd` & `polyfile-0.5.1/polyfile/magic_defs/usd`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/uuencode` & `polyfile-0.5.1/polyfile/magic_defs/uuencode`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/vacuum-cleaner` & `polyfile-0.5.1/polyfile/magic_defs/vacuum-cleaner`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/varied.out` & `polyfile-0.5.1/polyfile/magic_defs/varied.out`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/varied.script` & `polyfile-0.5.1/polyfile/magic_defs/varied.script`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/vax` & `polyfile-0.5.1/polyfile/magic_defs/vax`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/vicar` & `polyfile-0.5.1/polyfile/magic_defs/vicar`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/virtual` & `polyfile-0.5.1/polyfile/magic_defs/virtual`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/virtutech` & `polyfile-0.5.1/polyfile/magic_defs/virtutech`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/visx` & `polyfile-0.5.1/polyfile/magic_defs/visx`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/vms` & `polyfile-0.5.1/polyfile/magic_defs/vms`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/vorbis` & `polyfile-0.5.1/polyfile/magic_defs/vorbis`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/warc` & `polyfile-0.5.1/polyfile/magic_defs/warc`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/weak` & `polyfile-0.5.1/polyfile/magic_defs/weak`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/web` & `polyfile-0.5.1/polyfile/magic_defs/web`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/webassembly` & `polyfile-0.5.1/polyfile/magic_defs/webassembly`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/windows` & `polyfile-0.5.1/polyfile/magic_defs/windows`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/wordprocessors` & `polyfile-0.5.1/polyfile/magic_defs/wordprocessors`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/wsdl` & `polyfile-0.5.1/polyfile/magic_defs/wsdl`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/x68000` & `polyfile-0.5.1/polyfile/magic_defs/x68000`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/xdelta` & `polyfile-0.5.1/polyfile/magic_defs/xdelta`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/xenix` & `polyfile-0.5.1/polyfile/magic_defs/xenix`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/xilinx` & `polyfile-0.5.1/polyfile/magic_defs/xilinx`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/xo65` & `polyfile-0.5.1/polyfile/magic_defs/xo65`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/xwindows` & `polyfile-0.5.1/polyfile/magic_defs/xwindows`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/zfs` & `polyfile-0.5.1/polyfile/magic_defs/zfs`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/zip` & `polyfile-0.5.1/polyfile/magic_defs/zip`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/magic_defs/zyxel` & `polyfile-0.5.1/polyfile/magic_defs/zyxel`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/nes.py` & `polyfile-0.5.1/polyfile/nes.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/nitf.py` & `polyfile-0.5.1/polyfile/nitf.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/pdf.py` & `polyfile-0.5.1/polyfile/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Callable, Dict, Iterator, Optional, Union
+from typing import Callable, Dict, Iterator, List, Optional, Type, TypeVar, Union
 import zlib
 
 from pdfminer.ascii85 import ascii85decode, asciihexdecode
 from pdfminer.ccitt import ccittfaxdecode
 from pdfminer.lzw import lzwdecode
 from pdfminer.pdfparser import PDFSyntaxError
 from pdfminer.pdftypes import PDFNotImplementedError
@@ -47,55 +47,173 @@
             raise PDFNoValidXRef('Unexpected EOF - file corrupted')
         (_, dic) = x[0]
     self.trailer.update(dict_value(dic))
     log.debug('trailer=%r', self.trailer)
     return
 
 
+def load_xref(self: PDFXRef, parser: "PDFParser"):
+    while True:
+        try:
+            (pos, line) = parser.nextline()
+            line = line.strip()
+            if not line:
+                continue
+        except PSEOF:
+            raise PDFNoValidXRef("Unexpected EOF - file corrupted?")
+        if line.startswith(b"trailer"):
+            parser.seek(pos)
+            break
+        f = line.split(b" ")
+        if len(f) != 2:
+            error_msg = "Trailer not found: {!r}: line={!r}".format(parser, line)
+            raise PDFNoValidXRef(error_msg)
+        try:
+            (start, nobjs) = map(int, f)
+        except ValueError:
+            error_msg = "Invalid line: {!r}: line={!r}".format(parser, line)
+            raise PDFNoValidXRef(error_msg)
+        for objid in range(start, start + nobjs):
+            try:
+                (_, line) = parser.nextline()
+                line = line.strip()
+            except PSEOF:
+                raise PDFNoValidXRef("Unexpected EOF - file corrupted?")
+            f = line.split(b" ")
+            if len(f) != 3:
+                error_msg = "Invalid XRef format: {!r}, line={!r}".format(
+                    parser, line
+                )
+                raise PDFNoValidXRef(error_msg)
+            (pos_b, genno_b, use_b) = f
+            if use_b != b"n":
+                continue
+            self.offsets[objid] = (None, pos_b.__int__(), genno_b.__int__())
+    log.debug("xref objects: %r", self.offsets)
+    self.load_trailer(parser)
+
+
 PDFXRef.load_trailer = load_trailer
+PDFXRef.load = load_xref
 
 
 class PSToken:
     pdf_offset: int
     pdf_bytes: int
 
     def __new__(cls, *args, **kwargs):
         ret = super().__new__(cls, *args)
         ret.pdf_offset = kwargs["pdf_offset"]
         ret.pdf_bytes = kwargs["pdf_bytes"]
         return ret
 
     def __int__(self):
-        return PSInt(self, pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        if isinstance(self, PSInt):
+            return self
+        return PSInt(int(self, base=10), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
 
     def __float__(self):
-        return PSFloat(self, pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        if isinstance(self, float):
+            return self
+        elif isinstance(self, int):
+            return PSFloat(int(self, base=10), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        elif isinstance(self, bytes):
+            return PSFloat(self.decode(), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        elif isinstance(self, PSStr):
+            return PSFloat(str(self), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        else:
+            raise NotImplementedError()
 
     def __bytes__(self):
         if isinstance(self, PSBytes):
             return self
         else:
             return PSBytes(self, pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
 
     def __hex__(self):
         return PSStr(super().__hex__(), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
 
     def __str__(self):
-        return PSStr(super().__str__(), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+        raise NotImplementedError()
+        # return PSStr(super().__str__(), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
 
     def __repr__(self):
         return f"{self.__class__.__name__}({super().__repr__()}, pdf_offset={self.pdf_offset!r}, "\
                f"pdf_bytes={self.pdf_bytes!r})"
 
 
 class PSInt(PSToken, int):
-    pass
+    def __index__(self):
+        return self
+
+    def __str__(self):
+        return str(int(self))
+
+
+C = TypeVar("C")
 
 
 class PSSequence(PSToken):
+    def split(self: Type[C], sep: Optional[C] = None, maxsplit: int = -1) -> List[C]:
+        remainder = self
+        current: Optional[C] = None
+        result: List[C] = []
+        if sep is None:
+            remainder = remainder.strip()
+        while remainder and (maxsplit < 0 or len(result) <= maxsplit):
+            c = remainder[0:1]
+            remainder = remainder[1:]
+            if sep is None:
+                if not c.strip():
+                    if current is not None:
+                        result.append(current)
+                        current = None
+                else:
+                    if current is None:
+                        current = c
+                    else:
+                        current += c
+            else:
+                if current is None:
+                    current = c
+                else:
+                    current += c
+                if current[-len(sep):] == sep:
+                    result.append(current[:-len(sep)])
+                    current = None
+        if current is not None:
+            if not result or maxsplit < 0 or len(result) <= maxsplit:
+                result.append(current)
+            else:
+                result[-1] += current
+        return result
+
+    def __add__(self: Type[C], other) -> C:
+        if isinstance(other, self.__class__) and other.pdf_offset == self.pdf_offset + self.pdf_bytes:
+            return self.__class__(super().__add__(other), pdf_offset=self.pdf_offset)
+        return self.__class__(super().__add__(other), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
+
+    def __radd__(self: Type[C], other) -> C:
+        return self.__class__(other, pdf_offset=self.pdf_offset - len(other)) + self
+
+    def lstrip(self: Type[C], chars: bytes = b" \t\n\r") -> C:
+        ret = self
+        while ret and ret[0] in chars:
+            ret = ret[1:]
+        return ret
+
+    def rstrip(self: Type[C], chars: bytes = b" \t\n\r") -> C:
+        ret = self
+        while ret and ret[-1] in chars:
+            ret = ret[:-1]
+        return ret
+
+    def strip(self: Type[C], chars: bytes = b" \t\n\r") -> C:
+        return self.lstrip(chars).rstrip(chars)
+
     def __getitem__(self, item):
         if isinstance(item, int):
             value = super().__getitem__(item)
             return make_ps_object(value, pdf_offset=self.pdf_offset+item, pdf_bytes=self.pdf_bytes-item)
         elif isinstance(item, slice):
             if item.start is None:
                 start = 0
@@ -135,18 +253,36 @@
 class PSBytes(PSSequence, bytes):
     def __new__(cls, *args, **kwargs):
         kwargs = dict(kwargs)
         if "pdf_bytes" not in kwargs:
             kwargs["pdf_bytes"] = len(args[0])
         return super().__new__(cls, *args, **kwargs)
 
-    def decode(self, encoding: str = ..., errors: str = ...) -> PSStr:
+    def __getitem__(self, item):
+        if isinstance(item, slice):
+            if item.start is None:
+                start = 0
+            else:
+                start = item.start
+            return PSBytes(super().__getitem__(item), pdf_offset=self.pdf_offset + start)
+        else:
+            ret = super().__getitem__(item)
+            if isinstance(ret, PSInt):
+                return ret
+            else:
+                return PSInt(ret, pdf_offset=self.pdf_offset + item)
+
+    def decode(self, encoding: str = "utf-8", errors: str = "strict") -> PSStr:
         return PSStr(super().decode(encoding, errors), pdf_offset=self.pdf_offset, pdf_bytes=self.pdf_bytes)
 
 
+    def __str__(self):
+        return bytes.__str__(self)
+
+
 class PDFDeciphered(PSBytes):
     original_bytes: bytes
 
     def __new__(cls, *args, **kwargs):
         kwargs = dict(kwargs)
         if "pdf_bytes" not in kwargs:
             kwargs["pdf_bytes"] = len(args[0])
@@ -157,15 +293,16 @@
             raise ValueError(f"{cls.__name__}.__init__ requires the `original_bytes` argument")
         ret = super().__new__(cls, *args, **kwargs)
         setattr(ret, "original_bytes", original_bytes)
         return ret
 
 
 class PSFloat(PSToken, float):
-    pass
+    def __str__(self):
+        return float.__str__(self)
 
 
 class PSBool:
     def __init__(self, value: bool, pdf_offset: int, pdf_bytes: int):
         self.value: bool = value
         self.pdf_offset: int = pdf_offset
         self.pdf_bytes: int = pdf_bytes
@@ -276,14 +413,18 @@
 
     def __new__(cls, *args, pdf_offset: int, pdf_bytes: int, **kwargs):
         ret = super().__new__(cls, *args, **kwargs)
         ret.pdf_offset = pdf_offset
         ret.pdf_bytes = pdf_bytes
         return ret
 
+    def __str__(self):
+        return dict.__str__(self)
+
+
 
 class PDFList(PSSequence, list):
     @staticmethod
     def load(iterable) -> "PDFList":
         start_offset: Optional[int] = None
         end_offset: Optional[int] = None
         items = []
@@ -294,14 +435,18 @@
                 if end_offset is None or end_offset < item.pdf_offset + item.pdf_bytes:
                     end_offset = item.pdf_offset + item.pdf_bytes
             items.append(item)
         if start_offset is None or end_offset is None:
             raise ValueError(f"Cannot determine PDF bounds for list {items!r}")
         return PDFList(items, pdf_offset=start_offset, pdf_bytes=end_offset - start_offset)
 
+    def __str__(self):
+        return list.__str__(self)
+
+
 
 def make_ps_object(value, pdf_offset: int, pdf_bytes: int) -> Union[PDFBaseParserToken, PSStr, PDFDict]:
     if isinstance(value, PSLiteral):
         return PDFLiteral(value.name, pdf_offset=pdf_offset, pdf_bytes=pdf_bytes)
     # Unfortunately, we can't convert PSKeywords to PDFKeywords here because pdfminer requires them to be singletons
     # elif isinstance(value, PSKeyword):
     #     return PDFKeyword(value.name, pdf_offset=pdf_offset, pdf_bytes=pdf_bytes)
@@ -804,14 +949,15 @@
 
             try:
                 PDFXRef.get_trailer = get_trailer
                 # try it again with our patched trailer loading:
                 super().__init__(*args, **kwargs)
             finally:
                 PDFXRef.get_trailer = old_get_trailer
+
     # @property
     # def xrefs(self):
     #     if not self._xrefs:
     #         pass
     #     return self._xrefs
     #
     # @xrefs.setter
@@ -923,23 +1069,23 @@
     finally:
         file_stream.seek(start_pos - skipped_bytes)
 
 
 def pdf_obj_parser(file_stream, obj, objid: int, parent: Match, pdf_header_offset: int = 0) -> Iterator[Submatch]:
     data: Optional[bytes] = None
     if isinstance(obj, PDFObjectStream):
-        log.status(f"Parsing PDF obj {obj.objid} {obj.genno}")
+        log.status(f"Parsing PDF obj {obj.objid!s} {obj.genno!s}")
         try:
             data = obj.get_data()
         except PDFNotImplementedError as e:
-            log.error(f"Unsupported PDF stream filter in object {obj.objid} {obj.genno}: {e!s}")
+            log.error(f"Unsupported PDF stream filter in object {obj.objid!s} {obj.genno!s}: {e!s}")
         relative_offset = obj.attrs.pdf_offset
         obj_length = obj.data_value.pdf_offset - obj.attrs.pdf_offset + obj.data_value.pdf_bytes - 1
     else:
-        log.status(f"Parsing PDF obj {objid}")
+        log.status(f"Parsing PDF obj {objid!s}")
         relative_offset = obj.pdf_offset
         obj_length = obj.pdf_bytes - 1
     with file_stream.save_pos():
         file_stream.seek(parent.offset + relative_offset - pdf_header_offset)
         reverse_skip_whitespace(file_stream)
         if reverse_expect(file_stream, b"obj") and reverse_skip_whitespace(file_stream):
             version = reverse_expect(file_stream, lambda _, b: ord('0') <= b[0] <= ord('9'))
@@ -953,15 +1099,15 @@
         skip_whitespace(file_stream)
         if file_stream.read(6) == b"endobj":
             skip_whitespace(file_stream)
             obj_length = file_stream.tell() - (parent.offset + relative_offset - pdf_header_offset)
     if isinstance(obj, PDFObjectStream):
         match = Submatch(
             name="PDFObject",
-            display_name=f"PDFObject{obj.objid}.{obj.genno}",
+            display_name=f"PDFObject{obj.objid!s}.{obj.genno!s}",
             match_obj=(obj.objid, obj.genno),
             relative_offset=relative_offset,
             length=obj_length,
             parent=parent
         )
         yield match
         yield from parse_object(obj.attrs, matcher=parent.matcher, parent=match, pdf_header_offset=pdf_header_offset)
@@ -1019,7 +1165,100 @@
                     continue
                 yielded.add((obj.objid, obj.genno))
             else:
                 if objid in yielded or not hasattr(obj, "pdf_offset") or not hasattr(obj, "pdf_bytes"):
                     continue
                 yielded.add(objid)
             yield from pdf_obj_parser(file_stream, obj, objid, parent, pdf_header_offset=pdf_header_offset)
+
+        trailer = xref.get_trailer()
+        if trailer is not None:
+            trailer_start = min(k.pdf_offset for k in trailer.keys())
+            trailer_end = max(v.pdf_offset + v.pdf_bytes for v in trailer.values())
+            t = Submatch(
+                "Trailer",
+                b"",
+                relative_offset=trailer_start,
+                length=trailer_end - trailer_start,
+                parent=parent
+            )
+            yield t
+            for k, v in trailer.items():
+                kvp = Submatch(
+                    "KeyValuePair",
+                    b"",
+                    relative_offset=k.pdf_offset - trailer_start,
+                    length=v.pdf_offset + v.pdf_bytes - k.pdf_offset,
+                    parent=t
+                )
+                yield kvp
+                yield Submatch(
+                    "Key",
+                    k,
+                    relative_offset=k.pdf_offset - k.pdf_offset,
+                    length=k.pdf_bytes,
+                    parent=kvp
+                )
+                value_match = Submatch(
+                    "Value",
+                    b"",
+                    relative_offset=v.pdf_offset - k.pdf_offset,
+                    length=v.pdf_bytes,
+                    parent=kvp
+                )
+                yield value_match
+                yield from parse_object(v, matcher=parent.matcher, parent=value_match,
+                                        pdf_header_offset=pdf_header_offset)
+
+        if not isinstance(xref, PDFXRef):
+            continue
+
+        xref_start = min(min(c.pdf_offset for c in row if c is not None) for row in xref.offsets.values())
+        xref_end = max(max(c.pdf_offset + c.pdf_bytes for c in row if c is not None) for row in xref.offsets.values())
+        x = Submatch(
+            "XRefTable",
+            b"",
+            relative_offset=xref_start,
+            length=xref_end - xref_start,
+            parent=parent
+        )
+        yield x
+        for row in xref.offsets.values():
+            row_start = min(c.pdf_offset for c in row if c is not None)
+            row_end = max(c.pdf_offset + c.pdf_bytes for c in row if c is not None)
+            row_match = Submatch(
+                "XRefRow",
+                b"",
+                relative_offset=row_start - xref_start,
+                length=row_end - row_start,
+                parent=x
+            )
+            yield row_match
+            obj_id, pos, gen_no = row
+            if obj_id is not None:
+                ret = Submatch(
+                    "ObjectID",
+                    b"",
+                    relative_offset=obj_id.pdf_offset - row_start,
+                    length=obj_id.pdf_bytes,
+                    parent=row_match
+                )
+                yield ret
+                yield from parse_object(obj_id, matcher=parent.matcher, parent=ret, pdf_header_offset=pdf_header_offset)
+            ret = Submatch(
+                "Position",
+                b"",
+                relative_offset=pos.pdf_offset - row_start,
+                length=pos.pdf_bytes,
+                parent=row_match
+            )
+            yield ret
+            yield from parse_object(ret, matcher=parent.matcher, parent=ret, pdf_header_offset=pdf_header_offset)
+            ret = Submatch(
+                "Generation",
+                b"",
+                relative_offset=gen_no.pdf_offset - row_start,
+                length=gen_no.pdf_bytes,
+                parent=row_match
+            )
+            yield ret
+            yield from parse_object(ret, matcher=parent.matcher, parent=ret, pdf_header_offset=pdf_header_offset)
```

### Comparing `polyfile-0.5.0/polyfile/polyfile.py` & `polyfile-0.5.1/polyfile/polyfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 import base64
 import hashlib
 from json import dumps
 from mimetypes import guess_extension
 from pathlib import Path
-import pkg_resources
+import sys
 from time import localtime
+import traceback
 from typing import Any, Callable, Dict, IO, Iterable, Iterator, List, Optional, Set, Tuple, Union
 
 from .fileutils import FileStream
 from . import logger
 from .magic import MagicMatcher, Match as MagicMatch, MatchContext, TestResult
 
-__version__: str = pkg_resources.require("polyfile")[0].version
+if sys.version_info >= (3, 10):
+    from importlib.metadata import version
+    __version__: str = version("polyfile")
+    del version
+else:
+    import pkg_resources
+    __version__ = pkg_resources.require("polyfile")[0].version
+    del pkg_resources
 mod_year = localtime(Path(__file__).stat().st_mtime).tm_year
 __copyright__: str = f"Copyright ©{mod_year} Trail of Bits"
 __license__: str = "Apache License Version 2.0 https://www.apache.org/licenses/"
 
 ParserFunction = Callable[[FileStream, "Match"], Iterator["Submatch"]]
 
 
@@ -251,14 +259,16 @@
                             yield first_submatch
                             yield from submatch_iter
                 except InvalidMatch:
                     pass
                 except Exception as e:
                     log.warning(f"Parser {parser!s} for MIME type {mimetype} raised an exception while "
                                 f"parsing {match_obj!s} in {file_stream!s}: {e!s}")
+                    if log.isEnabledFor(logger.logging.DEBUG):
+                        traceback.print_exc()
 
     def identify(
             self, file_stream: Union[str, Path, IO, FileStream]
     ) -> Iterator[MagicMatch]:
         with FileStream(file_stream) as f:
             context = MatchContext.load(f, only_match_mime=False)
             yield from self.magic_matcher.match(context)
```

### Comparing `polyfile-0.5.0/polyfile/profiling.py` & `polyfile-0.5.1/polyfile/profiling.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/repl.py` & `polyfile-0.5.1/polyfile/repl.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,26 +433,27 @@
                 elif answer == "n":
                     return False
                 elif answer == "y":
                     return True
 
     def load_history(self):
         try:
-            readline.read_history_file(HISTORY_PATH)
+            readline.read_history_file(str(HISTORY_PATH))
             self._prev_history_length = readline.get_current_history_length()
-        except FileNotFoundError:
+        except (FileNotFoundError, OSError):
             open(HISTORY_PATH, 'wb').close()
             self._prev_history_length = 0
         # default history len is -1 (infinite), which may grow unruly
         readline.set_history_length(2048)
 
     def store_history(self):
         new_length = readline.get_current_history_length()
         try:
-            readline.append_history_file(max(new_length - self._prev_history_length, 0), HISTORY_PATH)
+            if hasattr(readline, "append_history_file"):
+                readline.append_history_file(max(new_length - self._prev_history_length, 0), HISTORY_PATH)
             self._prev_history_length = readline.get_current_history_length()
         except IOError as e:
             log.warning(f"Unable to save history to {HISTORY_PATH!s}: {e!s}")
 
     def input(self, prompt: str = "") -> str:
         if not self._bound_tab_completion:
             self._bound_tab_completion = True
```

### Comparing `polyfile-0.5.0/polyfile/search.py` & `polyfile-0.5.1/polyfile/search.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/serialization.py` & `polyfile-0.5.1/polyfile/serialization.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/structmatcher.py` & `polyfile-0.5.1/polyfile/structmatcher.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/structs.py` & `polyfile-0.5.1/polyfile/structs.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/templates/download.js` & `polyfile-0.5.1/polyfile/templates/download.js`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/templates/hexdump.css` & `polyfile-0.5.1/polyfile/templates/hexdump.css`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/templates/hexdump.js` & `polyfile-0.5.1/polyfile/templates/hexdump.js`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/templates/jquery-3.4.1.min.js` & `polyfile-0.5.1/polyfile/templates/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/templates/template.html` & `polyfile-0.5.1/polyfile/templates/template.html`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/wildcards.py` & `polyfile-0.5.1/polyfile/wildcards.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile/zipmatcher.py` & `polyfile-0.5.1/polyfile/zipmatcher.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polyfile.egg-info/PKG-INFO` & `polyfile-0.5.1/polyfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfile
-Version: 0.5.0
+Version: 0.5.1
 Summary: A utility to recursively map the structure of a file.
 Home-page: https://github.com/trailofbits/polyfile
 Author: Trail of Bits
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -209,15 +209,15 @@
 matcher = MagicMatcher.parse(*list_of_paths_to_definitions)
 with open("file_to_test", "rb") as f:
     for match in matcher.match(f.read()):
         ...
 ```
 
 ### Debugging the libmagic DSL
-`libmagic` has an esoteric, poorly documented doman-specific language (DSL) for specifying its matching signatures.
+`libmagic` has an esoteric, poorly documented domain-specific language (DSL) for specifying its matching signatures.
 You can read the minimal and—as we have discovered in our cleanroom implementation—_incomplete_ documentation by running
 `man 5 magic`. PolyFile implements an interactive debugger for stepping through the DSL specifications, modeled after
 GDB. You can enter this debugger by passing the `--debugger` or `-db` argument to PolyFile. It is useful for both
 implementing new `libmagic` DSLs, as well as figuring out why an existing DSL fails to match against a given file.
 ```console
 $ polyfile -db input_file
 PolyFile 0.3.5
```

### Comparing `polyfile-0.5.0/polyfile.egg-info/SOURCES.txt` & `polyfile-0.5.1/polyfile.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 polyfile/__init__.py
 polyfile/__main__.py
 polyfile/arithmetic.py
+polyfile/ast.py
 polyfile/debugger.py
 polyfile/expressions.py
 polyfile/fileutils.py
 polyfile/html.py
 polyfile/iterators.py
 polyfile/jpeg.py
 polyfile/kaitaimatcher.py
@@ -28,14 +29,21 @@
 polyfile/zipmatcher.py
 polyfile.egg-info/PKG-INFO
 polyfile.egg-info/SOURCES.txt
 polyfile.egg-info/dependency_links.txt
 polyfile.egg-info/entry_points.txt
 polyfile.egg-info/requires.txt
 polyfile.egg-info/top_level.txt
+polyfile/http/__init__.py
+polyfile/http/defacto.py
+polyfile/http/deprecated.py
+polyfile/http/experimental.py
+polyfile/http/http_11.py
+polyfile/http/matcher.py
+polyfile/http/structured_headers.py
 polyfile/kaitai/__init__.py
 polyfile/kaitai/compiler.py
 polyfile/kaitai/parser.py
 polyfile/kaitai/parsers/__init__.py
 polyfile/kaitai/parsers/aix_utmp.py
 polyfile/kaitai/parsers/allegro_dat.py
 polyfile/kaitai/parsers/andes_firmware.py
```

### Comparing `polyfile-0.5.0/polymerge/__main__.py` & `polyfile-0.5.1/polymerge/__main__.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polymerge/cfg.py` & `polyfile-0.5.1/polymerge/cfg.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polymerge/polymerge.py` & `polyfile-0.5.1/polymerge/polymerge.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/polymerge/polytracker.py` & `polyfile-0.5.1/polymerge/polytracker.py`

 * *Files identical despite different names*

### Comparing `polyfile-0.5.0/setup.py` & `polyfile-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 setup(
     name='polyfile',
     description='A utility to recursively map the structure of a file.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/trailofbits/polyfile',
     author='Trail of Bits',
-    version="0.5.0",
+    version="0.5.1",
     packages=find_packages(exclude=("tests",)),
     python_requires='>=3.7',
     install_requires=[
+        "abnf~=2.2.0",
         "chardet~=5.0.0",
         "cint>=1.0.0",
         "graphviz>=0.20.1",
         "intervaltree>=2.4.0",
         "jinja2>=2.1.0",
-        "kaitaistruct>=0.7",
+        "kaitaistruct~=0.10",
         "networkx>=2.6.3",
         "pdfminer.six==20220524",
         "Pillow>=5.0.0",
         "pyreadline3;platform_system=='Windows'",
         "pyyaml>=3.13",
-        "setuptools"
+        "setuptools>=65.5.1"
     ],
     extras_require={
         'demangle': ['cxxfilt'],
         "dev": ["mypy", "pytest", "flake8"]
     },
     entry_points={
         'console_scripts': [
```

