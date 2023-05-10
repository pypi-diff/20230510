# Comparing `tmp/mahjong-utils-0.4.3.tar.gz` & `tmp/mahjong-utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahjong-utils-0.4.3.tar", last modified: Sun Feb 26 14:06:58 2023, max compression
+gzip compressed data, was "mahjong-utils-0.5.0.tar", last modified: Wed May 10 10:03:46 2023, max compression
```

## Comparing `mahjong-utils-0.4.3.tar` & `mahjong-utils-0.5.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/
--rw-rw-rw-   0        0        0       61 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9237 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     8982 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/
--rw-rw-rw-   0        0        0       27 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/.git
--rw-rw-rw-   0        0        0     2272 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/LICENSE
--rw-rw-rw-   0        0        0     7412 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/README.md
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/build-scripts/
--rw-rw-rw-   0        0        0      219 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/build-scripts/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.287161 mahjong-utils-0.4.3/kt/build-scripts/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.287161 mahjong-utils-0.4.3/kt/build-scripts/src/main/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/build-scripts/src/main/kotlin/
--rw-rw-rw-   0        0        0     3528 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
--rw-rw-rw-   0        0        0     1849 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.287161 mahjong-utils-0.4.3/kt/gradle/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/gradle/wrapper/
--rw-rw-rw-   0        0        0    59821 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/gradle/wrapper/gradle-wrapper.jar
--rw-rw-rw-   0        0        0      207 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/gradle/wrapper/gradle-wrapper.properties
--rw-rw-rw-   0        0        0       70 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/gradle.properties
--rw-rw-rw-   0        0        0     8304 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/gradlew
--rwxrwxrwx   0        0        0     2763 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/gradlew.bat
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/kotlin-js-store/
--rw-rw-rw-   0        0        0    90004 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/kotlin-js-store/yarn.lock
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.318410 mahjong-utils-0.4.3/kt/mahjong-utils-entry/
--rw-rw-rw-   0        0        0     2247 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.287161 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0      765 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
--rw-rw-rw-   0        0        0     3589 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
--rw-rw-rw-   0        0        0     2402 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
--rw-rw-rw-   0        0        0     1098 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsMain/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1468 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsTest/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     6239 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeMain/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1243 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeTest/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     5972 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
--rw-rw-rw-   0        0        0      102 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/settings.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/common/
--rw-rw-rw-   0        0        0     5459 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
--rw-rw-rw-   0        0        0     7596 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     3866 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     6397 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
--rw-rw-rw-   0        0        0     8108 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
--rw-rw-rw-   0        0        0      442 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/
--rw-rw-rw-   0        0        0     3780 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
--rw-rw-rw-   0        0        0     4359 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
--rw-rw-rw-   0        0        0     6033 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
--rw-rw-rw-   0        0        0     7854 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
--rw-rw-rw-   0        0        0      308 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.334035 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/hand/
--rw-rw-rw-   0        0        0      412 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
--rw-rw-rw-   0        0        0     3482 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
--rw-rw-rw-   0        0        0      303 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     3934 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
--rw-rw-rw-   0        0        0     6192 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
--rw-rw-rw-   0        0        0     4392 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
--rw-rw-rw-   0        0        0     3955 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
--rw-rw-rw-   0        0        0     7158 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
--rw-rw-rw-   0        0        0     5459 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
--rw-rw-rw-   0        0        0     2557 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     7774 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
--rw-rw-rw-   0        0        0     1683 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
--rw-rw-rw-   0        0        0    10647 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/jvmTest/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.302786 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     2194 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     5611 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     2140 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
--rw-rw-rw-   0        0        0    30671 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     9674 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
--rw-rw-rw-   0        0        0     6902 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
--rw-rw-rw-   0        0        0      573 2023-02-26 14:06:00.000000 mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.349659 mahjong-utils-0.4.3/mahjong_utils/
--rw-rw-rw-   0        0        0      116 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.365286 mahjong-utils-0.4.3/mahjong_utils/hora/
--rw-rw-rw-   0        0        0       44 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/hora/__init__.py
--rw-rw-rw-   0        0        0     2714 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/hora/hora.py
--rw-rw-rw-   0        0        0     6263 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/hora/models.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.365286 mahjong-utils-0.4.3/mahjong_utils/lib/
--rw-rw-rw-   0        0        0     2209 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/lib/__init__.py
--rw-rw-rw-   0        0        0    21112 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/lib/libmahjongutils_api.i
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.365286 mahjong-utils-0.4.3/mahjong_utils/models/
--rw-rw-rw-   0        0        0      176 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/furo.py
--rw-rw-rw-   0        0        0     1360 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/hand.py
--rw-rw-rw-   0        0        0     6769 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/hand_pattern.py
--rw-rw-rw-   0        0        0     3136 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/mentsu.py
--rw-rw-rw-   0        0        0     4718 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/tatsu.py
--rw-rw-rw-   0        0        0     6600 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/tile.py
--rw-rw-rw-   0        0        0      618 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/tile_type.py
--rw-rw-rw-   0        0        0      367 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/models/wind.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/
--rw-rw-rw-   0        0        0       55 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/__init__.py
--rw-rw-rw-   0        0        0      605 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/models.py
--rw-rw-rw-   0        0        0      924 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/point_by_han_hu.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/mahjong_utils/shanten/
--rw-rw-rw-   0        0        0       47 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/shanten/__init__.py
--rw-rw-rw-   0        0        0    10358 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/shanten/models.py
--rw-rw-rw-   0        0        0     4024 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/shanten/shanten.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/mahjong_utils/yaku/
--rw-rw-rw-   0        0        0      172 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/__init__.py
--rw-rw-rw-   0        0        0      543 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/all_yaku.py
--rw-rw-rw-   0        0        0     1353 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/common.py
--rw-rw-rw-   0        0        0      649 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/extra.py
--rw-rw-rw-   0        0        0      168 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/yaku.py
--rw-rw-rw-   0        0        0     1156 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/mahjong_utils/yaku/yakuman.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.365286 mahjong-utils-0.4.3/mahjong_utils.egg-info/
--rw-rw-rw-   0        0        0     9237 2023-02-26 14:06:58.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3932 2023-02-26 14:06:58.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 14:06:58.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-26 14:06:57.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-02-26 14:06:58.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-26 14:06:58.000000 mahjong-utils-0.4.3/mahjong_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     5019 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:06:58.380910 mahjong-utils-0.4.3/tests/
--rw-rw-rw-   0        0        0     1221 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/tests/test_han_hu.py
--rw-rw-rw-   0        0        0     5422 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/tests/test_hora.py
--rw-rw-rw-   0        0        0      297 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/tests/test_lib.py
--rw-rw-rw-   0        0        0     8777 2023-02-26 14:05:58.000000 mahjong-utils-0.4.3/tests/test_shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.259481 mahjong-utils-0.5.0/
+-rw-rw-rw-   0        0        0       61 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9237 2023-05-10 10:03:46.258950 mahjong-utils-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8982 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/
+-rw-rw-rw-   0        0        0       27 2023-05-10 10:00:50.000000 mahjong-utils-0.5.0/kt/.git
+-rw-rw-rw-   0        0        0     2272 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/LICENSE
+-rw-rw-rw-   0        0        0     7412 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/build-scripts/
+-rw-rw-rw-   0        0        0      219 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build-scripts/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179386 mahjong-utils-0.5.0/kt/build-scripts/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179386 mahjong-utils-0.5.0/kt/build-scripts/src/main/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/
+-rw-rw-rw-   0        0        0     3528 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
+-rw-rw-rw-   0        0        0     1341 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179895 mahjong-utils-0.5.0/kt/gradle/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/gradle/wrapper/
+-rw-rw-rw-   0        0        0    59821 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.jar
+-rw-rw-rw-   0        0        0      207 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.properties
+-rw-rw-rw-   0        0        0      160 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle.properties
+-rw-rw-rw-   0        0        0     8304 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradlew
+-rwxrwxrwx   0        0        0     2763 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradlew.bat
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/kotlin-js-store/
+-rw-rw-rw-   0        0        0   104679 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/kotlin-js-store/yarn.lock
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/
+-rw-rw-rw-   0        0        0     2247 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0      765 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
+-rw-rw-rw-   0        0        0     3589 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
+-rw-rw-rw-   0        0        0     2402 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
+-rw-rw-rw-   0        0        0     1098 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1468 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     6239 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1243 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     5972 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
+-rw-rw-rw-   0        0        0      102 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/settings.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/
+-rw-rw-rw-   0        0        0     5458 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
+-rw-rw-rw-   0        0        0     7595 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     3866 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     6458 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
+-rw-rw-rw-   0        0        0     8108 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
+-rw-rw-rw-   0        0        0      442 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.217532 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/
+-rw-rw-rw-   0        0        0     3780 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
+-rw-rw-rw-   0        0        0     4359 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
+-rw-rw-rw-   0        0        0     6033 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
+-rw-rw-rw-   0        0        0     8193 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
+-rw-rw-rw-   0        0        0      308 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.219514 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/
+-rw-rw-rw-   0        0        0      412 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
+-rw-rw-rw-   0        0        0     3482 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
+-rw-rw-rw-   0        0        0      303 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     3755 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
+-rw-rw-rw-   0        0        0     6200 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
+-rw-rw-rw-   0        0        0     4268 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
+-rw-rw-rw-   0        0        0     4904 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
+-rw-rw-rw-   0        0        0    10782 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
+-rw-rw-rw-   0        0        0     6362 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
+-rw-rw-rw-   0        0        0     3285 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     7774 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
+-rw-rw-rw-   0        0        0     1683 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
+-rw-rw-rw-   0        0        0    10647 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/jvmTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.188968 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     2194 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     5806 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     2656 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
+-rw-rw-rw-   0        0        0    44661 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     9674 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
+-rw-rw-rw-   0        0        0     6902 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
+-rw-rw-rw-   0        0        0      573 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/mahjong_utils/
+-rw-rw-rw-   0        0        0      116 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.238312 mahjong-utils-0.5.0/mahjong_utils/hora/
+-rw-rw-rw-   0        0        0       44 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/__init__.py
+-rw-rw-rw-   0        0        0     2714 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/hora.py
+-rw-rw-rw-   0        0        0     6263 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/models.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.239616 mahjong-utils-0.5.0/mahjong_utils/lib/
+-rw-rw-rw-   0        0        0     2209 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/lib/__init__.py
+-rw-rw-rw-   0        0        0    22878 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/lib/libmahjongutils_api.i
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.246898 mahjong-utils-0.5.0/mahjong_utils/models/
+-rw-rw-rw-   0        0        0      176 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/furo.py
+-rw-rw-rw-   0        0        0     1360 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/hand.py
+-rw-rw-rw-   0        0        0     6769 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/hand_pattern.py
+-rw-rw-rw-   0        0        0     3136 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/mentsu.py
+-rw-rw-rw-   0        0        0     4718 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tatsu.py
+-rw-rw-rw-   0        0        0     6600 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tile.py
+-rw-rw-rw-   0        0        0      618 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tile_type.py
+-rw-rw-rw-   0        0        0      367 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/wind.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.248629 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/
+-rw-rw-rw-   0        0        0       55 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/models.py
+-rw-rw-rw-   0        0        0      924 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/point_by_han_hu.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.249674 mahjong-utils-0.5.0/mahjong_utils/shanten/
+-rw-rw-rw-   0        0        0       47 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/__init__.py
+-rw-rw-rw-   0        0        0    12095 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/models.py
+-rw-rw-rw-   0        0        0     4024 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.251687 mahjong-utils-0.5.0/mahjong_utils/yaku/
+-rw-rw-rw-   0        0        0      172 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/all_yaku.py
+-rw-rw-rw-   0        0        0     1353 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/common.py
+-rw-rw-rw-   0        0        0      649 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/extra.py
+-rw-rw-rw-   0        0        0      168 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/yaku.py
+-rw-rw-rw-   0        0        0     1156 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/yakuman.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.236336 mahjong-utils-0.5.0/mahjong_utils.egg-info/
+-rw-rw-rw-   0        0        0     9237 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3932 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 10:03:45.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:03:46.259989 mahjong-utils-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     5019 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.258316 mahjong-utils-0.5.0/tests/
+-rw-rw-rw-   0        0        0     1221 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_han_hu.py
+-rw-rw-rw-   0        0        0     5422 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_hora.py
+-rw-rw-rw-   0        0        0      297 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_lib.py
+-rw-rw-rw-   0        0        0     8938 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_shanten.py
```

### Comparing `mahjong-utils-0.4.3/PKG-INFO` & `mahjong-utils-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.4.3
+Version: 0.5.0
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.4.3/README.md` & `mahjong-utils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/.gitignore` & `mahjong-utils-0.5.0/kt/.gitignore`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/LICENSE` & `mahjong-utils-0.5.0/kt/LICENSE`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/README.md` & `mahjong-utils-0.5.0/kt/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts` & `mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/build.gradle.kts` & `mahjong-utils-0.5.0/kt/build.gradle.kts`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 plugins {
-    kotlin("multiplatform") version "1.7.21"
-    kotlin("plugin.serialization") version "1.7.21"
+    kotlin("multiplatform") version "1.8.21"
+    kotlin("plugin.serialization") version "1.8.10"
     id("build.publication")
 }
 
 repositories {
     mavenCentral()
 }
 
@@ -28,34 +28,22 @@
         isMingwX64 -> mingwX64("native")
         else -> throw GradleException("Host OS is not supported in Kotlin/Native.")
     }
 
     sourceSets {
         val commonMain by getting {
             dependencies {
-                implementation("org.jetbrains.kotlinx:kotlinx-serialization-core:1.4.1")
+                implementation("org.jetbrains.kotlinx:kotlinx-serialization-core:1.5.0")
             }
         }
         val commonTest by getting {
             dependencies {
                 implementation(kotlin("test")) // This brings all the platform dependencies automatically
             }
         }
     }
-
-    val publicationsFromMainHost = listOf(jvm(), js()).map { it.name } + "kotlinMultiplatform"
-    publishing {
-        publications {
-            matching { it.name in publicationsFromMainHost }.all {
-                val targetPublication = this@all
-                tasks.withType<AbstractPublishToMaven>()
-                    .matching { it.publication == targetPublication }
-                    .configureEach { onlyIf { findProperty("isMainHost") == "true" } }
-            }
-        }
-    }
 }
 
 tasks.wrapper {
     gradleVersion = "7.4.2"
     distributionType = Wrapper.DistributionType.ALL
 }
```

### Comparing `mahjong-utils-0.4.3/kt/gradle/wrapper/gradle-wrapper.jar` & `mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/gradlew` & `mahjong-utils-0.5.0/kt/gradlew`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/gradlew.bat` & `mahjong-utils-0.5.0/kt/gradlew.bat`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/kotlin-js-store/yarn.lock` & `mahjong-utils-0.5.0/kt/kotlin-js-store/yarn.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # THIS IS AN AUTOGENERATED FILE. DO NOT EDIT THIS FILE DIRECTLY.
 # yarn lockfile v1
 
 
+"@babel/code-frame@^7.10.4":
+  version "7.21.4"
+  resolved "https://registry.npmmirror.com/@babel/code-frame/-/code-frame-7.21.4.tgz#d0fa9e4413aca81f2b23b9442797bda1826edb39"
+  integrity sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==
+  dependencies:
+    "@babel/highlight" "^7.18.6"
+
+"@babel/helper-validator-identifier@^7.18.6":
+  version "7.19.1"
+  resolved "https://registry.npmmirror.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz#7eea834cf32901ffdc1a7ee555e2f9c27e249ca2"
+  integrity sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==
+
+"@babel/highlight@^7.18.6":
+  version "7.18.6"
+  resolved "https://registry.npmmirror.com/@babel/highlight/-/highlight-7.18.6.tgz#81158601e93e2563795adcbfbdf5d64be3f2ecdf"
+  integrity sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==
+  dependencies:
+    "@babel/helper-validator-identifier" "^7.18.6"
+    chalk "^2.0.0"
+    js-tokens "^4.0.0"
+
 "@colors/colors@1.5.0":
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/@colors/colors/-/colors-1.5.0.tgz#bb504579c1cae923e6576a4f5da43d25f97bdbd9"
   integrity sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==
 
 "@discoveryjs/json-ext@^0.5.0":
   version "0.5.7"
@@ -48,14 +69,56 @@
   version "0.3.17"
   resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.17.tgz#793041277af9073b0951a7fe0f0d8c4c98c36985"
   integrity sha512-MCNzAp77qzKca9+W/+I0+sEpaUnZoeasnghNeVc41VZCEKaCH73Vq3BZZ/SzWIgrqE4H4ceI+p+b6C0mHf9T4g==
   dependencies:
     "@jridgewell/resolve-uri" "3.1.0"
     "@jridgewell/sourcemap-codec" "1.4.14"
 
+"@rollup/plugin-commonjs@^21.0.1":
+  version "21.1.0"
+  resolved "https://registry.npmmirror.com/@rollup/plugin-commonjs/-/plugin-commonjs-21.1.0.tgz#45576d7b47609af2db87f55a6d4b46e44fc3a553"
+  integrity sha512-6ZtHx3VHIp2ReNNDxHjuUml6ur+WcQ28N1yHgCQwsbNkQg2suhxGMDQGJOn/KuDxKtd1xuZP5xSTwBA4GQ8hbA==
+  dependencies:
+    "@rollup/pluginutils" "^3.1.0"
+    commondir "^1.0.1"
+    estree-walker "^2.0.1"
+    glob "^7.1.6"
+    is-reference "^1.2.1"
+    magic-string "^0.25.7"
+    resolve "^1.17.0"
+
+"@rollup/plugin-node-resolve@^13.1.3":
+  version "13.3.0"
+  resolved "https://registry.npmmirror.com/@rollup/plugin-node-resolve/-/plugin-node-resolve-13.3.0.tgz#da1c5c5ce8316cef96a2f823d111c1e4e498801c"
+  integrity sha512-Lus8rbUo1eEcnS4yTFKLZrVumLPY+YayBdWXgFSHYhTT2iJbMhoaaBL3xl5NCdeRytErGr8tZ0L71BMRmnlwSw==
+  dependencies:
+    "@rollup/pluginutils" "^3.1.0"
+    "@types/resolve" "1.17.1"
+    deepmerge "^4.2.2"
+    is-builtin-module "^3.1.0"
+    is-module "^1.0.0"
+    resolve "^1.19.0"
+
+"@rollup/plugin-typescript@^8.3.0":
+  version "8.5.0"
+  resolved "https://registry.npmmirror.com/@rollup/plugin-typescript/-/plugin-typescript-8.5.0.tgz#7ea11599a15b0a30fa7ea69ce3b791d41b862515"
+  integrity sha512-wMv1/scv0m/rXx21wD2IsBbJFba8wGF3ErJIr6IKRfRj49S85Lszbxb4DCo8iILpluTjk2GAAu9CoZt4G3ppgQ==
+  dependencies:
+    "@rollup/pluginutils" "^3.1.0"
+    resolve "^1.17.0"
+
+"@rollup/pluginutils@^3.0.9", "@rollup/pluginutils@^3.1.0":
+  version "3.1.0"
+  resolved "https://registry.npmmirror.com/@rollup/pluginutils/-/pluginutils-3.1.0.tgz#706b4524ee6dc8b103b3c995533e5ad680c02b9b"
+  integrity sha512-GksZ6pr6TpIjHm8h9lSQ8pi8BE9VeubNT0OMJ3B5uZJ8pz73NPiqOtCog/x2/QzM1ENChPKxMDhiQuRHsqc+lg==
+  dependencies:
+    "@types/estree" "0.0.39"
+    estree-walker "^1.0.1"
+    picomatch "^2.2.2"
+
 "@socket.io/component-emitter@~3.1.0":
   version "3.1.0"
   resolved "https://registry.yarnpkg.com/@socket.io/component-emitter/-/component-emitter-3.1.0.tgz#96116f2a912e0c02817345b3c10751069920d553"
   integrity sha512-+9jVqKhRSpsc591z5vX+X5Yyw+he/HCB4iQ/RYxw35CEPaY1gnsNE43nf9n9AaYjAQrTiI/mOwKUKdUs9vf7Xg==
 
 "@types/cookie@^0.4.1":
   version "0.4.1"
@@ -84,14 +147,19 @@
     "@types/json-schema" "*"
 
 "@types/estree@*":
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.0.tgz#5fb2e536c1ae9bf35366eed879e827fa59ca41c2"
   integrity sha512-WulqXMDUTYAXCjZnk6JtIHPigp55cVtDgDrO2gHRwhyJto21+1zbVCtOYB2L1F9w4qCQ0rOGWBnBe0FNTiEJIQ==
 
+"@types/estree@0.0.39":
+  version "0.0.39"
+  resolved "https://registry.npmmirror.com/@types/estree/-/estree-0.0.39.tgz#e177e699ee1b8c22d23174caaa7422644389509f"
+  integrity sha512-EYNwp3bU+98cpU4lAWYYL7Zz+2gryWH1qbdDTidVd6hkiR6weksdbMadyXKXNPEkQFhXM+hVO9ZygomHXp+AIw==
+
 "@types/estree@^0.0.51":
   version "0.0.51"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-0.0.51.tgz#cfd70924a25a3fd32b218e5e420e6897e1ac4f40"
   integrity sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==
 
 "@types/json-schema@*", "@types/json-schema@^7.0.8":
   version "7.0.11"
@@ -99,14 +167,26 @@
   integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
 "@types/node@*", "@types/node@>=10.0.0":
   version "18.11.9"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-18.11.9.tgz#02d013de7058cea16d36168ef2fc653464cfbad4"
   integrity sha512-CRpX21/kGdzjOpFsZSkcrXMGIBWMGNIHXXBVFSH+ggkftxg+XYP20TESbh+zFvFj3EQOl5byk0HTRn1IL6hbqg==
 
+"@types/node@^12.12.14":
+  version "12.20.55"
+  resolved "https://registry.npmmirror.com/@types/node/-/node-12.20.55.tgz#c329cbd434c42164f846b909bd6f85b5537f6240"
+  integrity sha512-J8xLz7q2OFulZ2cyGTLE1TbbZcjpno7FaN6zdJNrgAdrJ+DZzh/uFR6YrTb4C+nXakvud8Q4+rbhoIWlYQbUFQ==
+
+"@types/resolve@1.17.1":
+  version "1.17.1"
+  resolved "https://registry.npmmirror.com/@types/resolve/-/resolve-1.17.1.tgz#3afd6ad8967c77e4376c598a82ddd58f46ec45d6"
+  integrity sha512-yy7HuzQhj0dhGpD8RLXSZWEkLsV9ibvxvi6EiJ3bkqLAO1RGo0WbkWQiwpRlSFymTJRz0d3k5LM3kkx8ArDbLw==
+  dependencies:
+    "@types/node" "*"
+
 "@ungap/promise-all-settled@1.1.2":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@ungap/promise-all-settled/-/promise-all-settled-1.1.2.tgz#aa58042711d6e3275dd37dc597e5d31e8c290a44"
   integrity sha512-sL/cEvJWAnClXw0wHk85/2L0G6Sj8UB0Ctc1TEMbKSsmpRosqhwj9gWgFRZSrBr2f9tiXISwNhCPmlfqUqyb9Q==
 
 "@webassemblyjs/ast@1.11.1":
   version "1.11.1"
@@ -270,19 +350,24 @@
     negotiator "0.6.3"
 
 acorn-import-assertions@^1.7.6:
   version "1.8.0"
   resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz#ba2b5939ce62c238db6d93d81c9b111b29b855e9"
   integrity sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==
 
-acorn@^8.4.1, acorn@^8.5.0:
+acorn@^8.5.0:
   version "8.8.1"
   resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.1.tgz#0a3f9cbecc4ec3bea6f0a80b66ae8dd2da250b73"
   integrity sha512-7zFpHzhnqYKrkYdUjF1HI1bzd0VygEGX8lFk4k5zVMqHEoES+P+7TKI+EvLO9WVMJ8eekdO0aDEK044xTXwPPA==
 
+acorn@^8.7.1:
+  version "8.8.2"
+  resolved "https://registry.npmmirror.com/acorn/-/acorn-8.8.2.tgz#1b2f25db02af965399b9776b0c2c391276d37c4a"
+  integrity sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==
+
 ajv-keywords@^3.5.2:
   version "3.5.2"
   resolved "https://registry.yarnpkg.com/ajv-keywords/-/ajv-keywords-3.5.2.tgz#31f29da5ab6e00d1c2d329acf7b5929614d5014d"
   integrity sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==
 
 ajv@^6.12.5:
   version "6.12.6"
@@ -300,14 +385,21 @@
   integrity sha512-JoX0apGbHaUJBNl6yF+p6JAFYZ666/hhCGKN5t9QFjbJQKUU/g8MNbFDbvfrgKXvI1QpZplPOnwIo99lX/AAmA==
 
 ansi-regex@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/ansi-regex/-/ansi-regex-5.0.1.tgz#082cb2c89c9fe8659a311a53bd6a4dc5301db304"
   integrity sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==
 
+ansi-styles@^3.2.1:
+  version "3.2.1"
+  resolved "https://registry.npmmirror.com/ansi-styles/-/ansi-styles-3.2.1.tgz#41fbb20243e50b12be0f04b8dedbf07520ce841d"
+  integrity sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==
+  dependencies:
+    color-convert "^1.9.0"
+
 ansi-styles@^4.0.0, ansi-styles@^4.1.0:
   version "4.3.0"
   resolved "https://registry.yarnpkg.com/ansi-styles/-/ansi-styles-4.3.0.tgz#edd803628ae71c04c85ae7a0906edad34b648937"
   integrity sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==
   dependencies:
     color-convert "^2.0.1"
 
@@ -320,14 +412,19 @@
     picomatch "^2.0.4"
 
 argparse@^2.0.1:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/argparse/-/argparse-2.0.1.tgz#246f50f3ca78a3240f6c997e8a9bd1eac49e4b38"
   integrity sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==
 
+atob@^2.1.2:
+  version "2.1.2"
+  resolved "https://registry.npmmirror.com/atob/-/atob-2.1.2.tgz#6d9517eb9e030d2436666651e86bd9f6f13533c9"
+  integrity sha512-Wm6ukoaOGJi/73p/cl2GvLjTI5JM1k/O14isD73YML8StrH/7/lRFgmg8nICZgD3bZZvjwCGxtMOD3wWNAu8cg==
+
 balanced-match@^1.0.0:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/balanced-match/-/balanced-match-1.0.2.tgz#e83e3a7e3f300b34cb9d87f615fa0cbf357690ee"
   integrity sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==
 
 base64id@2.0.0, base64id@~2.0.0:
   version "2.0.0"
@@ -395,14 +492,19 @@
     update-browserslist-db "^1.0.9"
 
 buffer-from@^1.0.0:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
+builtin-modules@^3.3.0:
+  version "3.3.0"
+  resolved "https://registry.npmmirror.com/builtin-modules/-/builtin-modules-3.3.0.tgz#cae62812b89801e9656336e46223e030386be7b6"
+  integrity sha512-zhaCDicdLuWN5UbN5IMnFqNMhNfo919sH85y2/ea+5Yg9TsTkeZxpL+JLbp6cgYFS4sRLp3YV4S6yDuqVWHYOw==
+
 bytes@3.1.2:
   version "3.1.2"
   resolved "https://registry.yarnpkg.com/bytes/-/bytes-3.1.2.tgz#8b0beeb98605adf1b128fa4386403c009e0221a5"
   integrity sha512-/Nf7TyzTx6S3yRJObOAV7956r8cr2+Oj8AC5dt8wSP3BQAoeX58NoHyCU8P8zGkNXStjTSi6fzO6F0pBdcYbEg==
 
 call-bind@^1.0.0:
   version "1.0.2"
@@ -418,14 +520,23 @@
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001400:
   version "1.0.30001434"
   resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001434.tgz#ec1ec1cfb0a93a34a0600d37903853030520a4e5"
   integrity sha512-aOBHrLmTQw//WFa2rcF1If9fa3ypkC1wzqqiKHgfdrXTWcU8C4gKVZT77eQAPWN1APys3+uQ0Df07rKauXGEYA==
 
+chalk@^2.0.0:
+  version "2.4.2"
+  resolved "https://registry.npmmirror.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
+  integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
+  dependencies:
+    ansi-styles "^3.2.1"
+    escape-string-regexp "^1.0.5"
+    supports-color "^5.3.0"
+
 chalk@^4.1.0:
   version "4.1.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-4.1.2.tgz#aac4e2b7734a740867aeb16bf02aad556a1e7a01"
   integrity sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==
   dependencies:
     ansi-styles "^4.1.0"
     supports-color "^7.1.0"
@@ -464,21 +575,33 @@
   resolved "https://registry.yarnpkg.com/clone-deep/-/clone-deep-4.0.1.tgz#c19fd9bdbbf85942b4fd979c84dcf7d5f07c2387"
   integrity sha512-neHB9xuzh/wk0dIHweyAXv2aPGZIVk3pLMe+/RNzINf17fe0OG96QroktYAUm7SM1PBnzTabaLboqqxDyMU+SQ==
   dependencies:
     is-plain-object "^2.0.4"
     kind-of "^6.0.2"
     shallow-clone "^3.0.0"
 
+color-convert@^1.9.0:
+  version "1.9.3"
+  resolved "https://registry.npmmirror.com/color-convert/-/color-convert-1.9.3.tgz#bb71850690e1f136567de629d2d5471deda4c1e8"
+  integrity sha512-QfAUtd+vFdAtFQcC8CCyYt1fYWxSqAiK2cSD6zDB8N3cpsEBAvRxp9zOGg6G/SHHJYAT88/az/IuDGALsNVbGg==
+  dependencies:
+    color-name "1.1.3"
+
 color-convert@^2.0.1:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/color-convert/-/color-convert-2.0.1.tgz#72d3a68d598c9bdb3af2ad1e84f21d896abd4de3"
   integrity sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==
   dependencies:
     color-name "~1.1.4"
 
+color-name@1.1.3:
+  version "1.1.3"
+  resolved "https://registry.npmmirror.com/color-name/-/color-name-1.1.3.tgz#a7d0558bd89c42f795dd42328f740831ca53bc25"
+  integrity sha512-72fSenhMw2HZMTVHeCA9KCmpEIbzWiQsjN+BHcBbS9vr1mtt+vJjPdksIBNUmKAW8TFUDPJK5SUU3QhE9NEXDw==
+
 color-name@~1.1.4:
   version "1.1.4"
   resolved "https://registry.yarnpkg.com/color-name/-/color-name-1.1.4.tgz#c2a09a87acbde69543de6f63fa3995c826c536a2"
   integrity sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==
 
 colorette@^2.0.14:
   version "2.0.19"
@@ -491,14 +614,19 @@
   integrity sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==
 
 commander@^7.0.0:
   version "7.2.0"
   resolved "https://registry.yarnpkg.com/commander/-/commander-7.2.0.tgz#a36cb57d0b501ce108e4d20559a150a391d97ab7"
   integrity sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==
 
+commondir@^1.0.1:
+  version "1.0.1"
+  resolved "https://registry.npmmirror.com/commondir/-/commondir-1.0.1.tgz#ddd800da0c66127393cca5950ea968a3aaf1253b"
+  integrity sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==
+
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
   integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
 connect@^3.7.0:
   version "3.7.0"
@@ -562,14 +690,24 @@
     ms "2.1.2"
 
 decamelize@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/decamelize/-/decamelize-4.0.0.tgz#aa472d7bf660eb15f3494efd531cab7f2a709837"
   integrity sha512-9iE1PgSik9HeIIw2JO94IidnE3eBoQrFJ3w7sFuzSX4DpmZ3v5sZpUiV5Swcf6mQEF+Y0ru8Neo+p+nyh2J+hQ==
 
+decode-uri-component@^0.2.0:
+  version "0.2.2"
+  resolved "https://registry.npmmirror.com/decode-uri-component/-/decode-uri-component-0.2.2.tgz#e69dbe25d37941171dd540e024c444cd5188e1e9"
+  integrity sha512-FqUYQ+8o158GyGTrMFJms9qh3CqTKvAqgqsTnkLI8sKu0028orqBhxNMFkFen0zGyg6epACD32pjVk58ngIErQ==
+
+deepmerge@^4.2.2:
+  version "4.3.1"
+  resolved "https://registry.npmmirror.com/deepmerge/-/deepmerge-4.3.1.tgz#44b5f2147cd3b00d4b56137685966f26fd25dd4a"
+  integrity sha512-3sUqbMEc77XqpdNO7FRyRog+eW3ph+GYCbj+rK+uYyRMuwsVy0rMiVtPn+QJlKFvWP/1PYpapqYn0Me2knFn+A==
+
 depd@2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/depd/-/depd-2.0.0.tgz#b696163cc757560d09cf22cc8fad1571b79e76df"
   integrity sha512-g7nH6P6dyDioJogAAGprGpCtVImJhpPk/roCzdb3fIh61/s/nPsfR6onyMwkCAR/OlC3yBC0lESvUoQEAssIrw==
 
 destroy@1.2.0:
   version "1.2.0"
@@ -633,18 +771,18 @@
     base64id "2.0.0"
     cookie "~0.4.1"
     cors "~2.8.5"
     debug "~4.3.1"
     engine.io-parser "~5.0.3"
     ws "~8.2.3"
 
-enhanced-resolve@^5.9.3:
-  version "5.12.0"
-  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz#300e1c90228f5b570c4d35babf263f6da7155634"
-  integrity sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==
+enhanced-resolve@^5.10.0:
+  version "5.14.0"
+  resolved "https://registry.npmmirror.com/enhanced-resolve/-/enhanced-resolve-5.14.0.tgz#0b6c676c8a3266c99fa281e4433a706f5c0c61c4"
+  integrity sha512-+DCows0XNwLDcUhbFJPdlQEVnT2zXlCv7hPxemTz86/O+B/hCQ+mb7ydkPKiflpVraqLPCAfu7lDy+hBXueojw==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 ent@~2.2.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/ent/-/ent-2.2.0.tgz#e964219325a21d05f44466a2f686ed6ce5f5dd1d"
@@ -671,14 +809,19 @@
   integrity sha512-NiSupZ4OeuGwr68lGIeym/ksIZMJodUGOSCZ/FSnTxcrekbvqrgdUxlJOMpijaKZVjAJrWrGs/6Jy8OMuyj9ow==
 
 escape-string-regexp@4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/escape-string-regexp/-/escape-string-regexp-4.0.0.tgz#14ba83a5d373e3d311e5afca29cf5bfad965bf34"
   integrity sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==
 
+escape-string-regexp@^1.0.5:
+  version "1.0.5"
+  resolved "https://registry.npmmirror.com/escape-string-regexp/-/escape-string-regexp-1.0.5.tgz#1b61c0562190a8dff6ae3bb2cf0200ca130b86d4"
+  integrity sha512-vbRorB5FUQWvla16U8R/qgaFIya2qGzwDrNmCZuYKrbdSUMG6I1ZCGQRefkRVhuOkIGVne7BQ35DSfo1qvJqFg==
+
 eslint-scope@5.1.1:
   version "5.1.1"
   resolved "https://registry.yarnpkg.com/eslint-scope/-/eslint-scope-5.1.1.tgz#e786e59a66cb92b3f6c1fb0d508aab174848f48c"
   integrity sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==
   dependencies:
     esrecurse "^4.3.0"
     estraverse "^4.1.1"
@@ -696,14 +839,24 @@
   integrity sha512-39nnKffWz8xN1BU/2c79n9nB9HDzo0niYUqx6xyqUnyoAnQyyWpOTdZEeiCch8BBu515t4wp9ZmgVfVhn9EBpw==
 
 estraverse@^5.2.0:
   version "5.3.0"
   resolved "https://registry.yarnpkg.com/estraverse/-/estraverse-5.3.0.tgz#2eea5290702f26ab8fe5370370ff86c965d21123"
   integrity sha512-MMdARuVEQziNTeJD8DgMqmhwR11BRQ/cBP+pLtYdSTnf3MIO8fFeiINEbX36ZdNlfU/7A9f3gUw49B3oQsvwBA==
 
+estree-walker@^1.0.1:
+  version "1.0.1"
+  resolved "https://registry.npmmirror.com/estree-walker/-/estree-walker-1.0.1.tgz#31bc5d612c96b704106b477e6dd5d8aa138cb700"
+  integrity sha512-1fMXF3YP4pZZVozF8j/ZLfvnR8NSIljt56UhbZ5PeeDmmGHpgpdwQt7ITlGvYaQukCvuBRMLEiKiYC+oeIg4cg==
+
+estree-walker@^2.0.1:
+  version "2.0.2"
+  resolved "https://registry.npmmirror.com/estree-walker/-/estree-walker-2.0.2.tgz#52f010178c2a4c117a7757cfe942adb7d2da4cac"
+  integrity sha512-Rfkk/Mp/DL7JVje3u18FxFujQlTNR2q6QfMSMB7AvCBx91NGj/ba3kCfza0f6dVDbw7YlRf/nDrn7pQrCCyQ/w==
+
 eventemitter3@^4.0.0:
   version "4.0.7"
   resolved "https://registry.yarnpkg.com/eventemitter3/-/eventemitter3-4.0.7.tgz#2de9b68f6528d5644ef5c59526a1b4a07306169f"
   integrity sha512-8guHBZCwKnFhYdHr2ysuRWErTwhoN2X8XELRlrRwpmfeY2jjuUN4taQMsULKUVo1K4DvZl+0pgfyoysHxvmvEw==
 
 events@^3.2.0:
   version "3.3.0"
@@ -777,15 +930,15 @@
   integrity sha512-5nqDSxl8nn5BSNxyR3n4I6eDmbolI6WT+QqR547RwxQapgjQBmtktdP+HTBb/a/zLsbzERTONyUB5pefh5TtjQ==
 
 follow-redirects@^1.0.0:
   version "1.15.2"
   resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.15.2.tgz#b460864144ba63f2681096f274c4e57026da2c13"
   integrity sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==
 
-format-util@1.0.5:
+format-util@1.0.5, format-util@^1.0.5:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/format-util/-/format-util-1.0.5.tgz#1ffb450c8a03e7bccffe40643180918cc297d271"
   integrity sha512-varLbTj0e0yVyRpqQhuWV+8hlePAgaoFRhNFj50BNjEIrw1/DphHSObtqwskVCPWNgzwPoQrZAbfa/SBiicNeg==
 
 fs-extra@^8.1.0:
   version "8.1.0"
   resolved "https://registry.yarnpkg.com/fs-extra/-/fs-extra-8.1.0.tgz#49d43c45a88cd9677668cb7be1b46efdb8d2e1c0"
@@ -844,15 +997,15 @@
     fs.realpath "^1.0.0"
     inflight "^1.0.4"
     inherits "2"
     minimatch "^3.0.4"
     once "^1.3.0"
     path-is-absolute "^1.0.0"
 
-glob@^7.1.3, glob@^7.1.7:
+glob@^7.1.3, glob@^7.1.6, glob@^7.1.7:
   version "7.2.3"
   resolved "https://registry.yarnpkg.com/glob/-/glob-7.2.3.tgz#b8df0fb802bbfa8e89bd1d938b4e16578ed44f2b"
   integrity sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==
   dependencies:
     fs.realpath "^1.0.0"
     inflight "^1.0.4"
     inherits "2"
@@ -861,14 +1014,19 @@
     path-is-absolute "^1.0.0"
 
 graceful-fs@^4.1.2, graceful-fs@^4.1.6, graceful-fs@^4.2.0, graceful-fs@^4.2.4, graceful-fs@^4.2.6, graceful-fs@^4.2.9:
   version "4.2.10"
   resolved "https://registry.yarnpkg.com/graceful-fs/-/graceful-fs-4.2.10.tgz#147d3a006da4ca3ce14728c7aefc287c367d7a6c"
   integrity sha512-9ByhssR2fPVsNZj478qUUbKfmL0+t5BDVyjShtyZZLiK7ZDAArFFfopyOTj0M05wE2tJPisA4iTnnXl2YoPvOA==
 
+has-flag@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmmirror.com/has-flag/-/has-flag-3.0.0.tgz#b5d454dc2199ae225699f3467e5a07f3b955bafd"
+  integrity sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==
+
 has-flag@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/has-flag/-/has-flag-4.0.0.tgz#944771fd9c81c81265c4d6941860da06bb59479b"
   integrity sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==
 
 has-symbols@^1.0.3:
   version "1.0.3"
@@ -950,21 +1108,40 @@
 is-binary-path@~2.1.0:
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/is-binary-path/-/is-binary-path-2.1.0.tgz#ea1f7f3b80f064236e83470f86c09c254fb45b09"
   integrity sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==
   dependencies:
     binary-extensions "^2.0.0"
 
+is-builtin-module@^3.1.0:
+  version "3.2.1"
+  resolved "https://registry.npmmirror.com/is-builtin-module/-/is-builtin-module-3.2.1.tgz#f03271717d8654cfcaf07ab0463faa3571581169"
+  integrity sha512-BSLE3HnV2syZ0FK0iMA/yUGplUeMmNz4AW5fnTunbCIqZi4vG3WjJT9FHMy5D69xmAYBHXQhJdALdpwVxV501A==
+  dependencies:
+    builtin-modules "^3.3.0"
+
+is-core-module@^2.11.0:
+  version "2.12.0"
+  resolved "https://registry.npmmirror.com/is-core-module/-/is-core-module-2.12.0.tgz#36ad62f6f73c8253fd6472517a12483cf03e7ec4"
+  integrity sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==
+  dependencies:
+    has "^1.0.3"
+
 is-core-module@^2.9.0:
   version "2.11.0"
   resolved "https://registry.yarnpkg.com/is-core-module/-/is-core-module-2.11.0.tgz#ad4cb3e3863e814523c96f3f58d26cc570ff0144"
   integrity sha512-RRjxlvLDkD1YJwDbroBHMb+cukurkDWNyHx7D3oNB5x9rb5ogcksMC5wHCadcXoo67gVr/+3GFySh3134zi6rw==
   dependencies:
     has "^1.0.3"
 
+is-docker@^2.0.0:
+  version "2.2.1"
+  resolved "https://registry.npmmirror.com/is-docker/-/is-docker-2.2.1.tgz#33eeabe23cfe86f14bde4408a02c0cfb853acdaa"
+  integrity sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==
+
 is-extglob@^2.1.1:
   version "2.1.1"
   resolved "https://registry.yarnpkg.com/is-extglob/-/is-extglob-2.1.1.tgz#a88c02535791f02ed37c76a1b9ea9773c833f8c2"
   integrity sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==
 
 is-fullwidth-code-point@^3.0.0:
   version "3.0.0"
@@ -974,14 +1151,19 @@
 is-glob@^4.0.1, is-glob@~4.0.1:
   version "4.0.3"
   resolved "https://registry.yarnpkg.com/is-glob/-/is-glob-4.0.3.tgz#64f61e42cbbb2eec2071a9dac0b28ba1e65d5084"
   integrity sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==
   dependencies:
     is-extglob "^2.1.1"
 
+is-module@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmmirror.com/is-module/-/is-module-1.0.0.tgz#3258fb69f78c14d5b815d664336b4cffb6441591"
+  integrity sha512-51ypPSPCoTEIN9dy5Oy+h4pShgJmPCygKfyRCISBI+JoWT/2oJvK8QPxmwv7b/p239jXrm9M1mlQbyKJ5A152g==
+
 is-number@^7.0.0:
   version "7.0.0"
   resolved "https://registry.yarnpkg.com/is-number/-/is-number-7.0.0.tgz#7535345b896734d5f80c4d06c50955527a14f12b"
   integrity sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==
 
 is-plain-obj@^2.1.0:
   version "2.1.0"
@@ -991,19 +1173,33 @@
 is-plain-object@^2.0.4:
   version "2.0.4"
   resolved "https://registry.yarnpkg.com/is-plain-object/-/is-plain-object-2.0.4.tgz#2c163b3fafb1b606d9d17928f05c2a1c38e07677"
   integrity sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==
   dependencies:
     isobject "^3.0.1"
 
+is-reference@^1.2.1:
+  version "1.2.1"
+  resolved "https://registry.npmmirror.com/is-reference/-/is-reference-1.2.1.tgz#8b2dac0b371f4bc994fdeaba9eb542d03002d0b7"
+  integrity sha512-U82MsXXiFIrjCK4otLT+o2NA2Cd2g5MLoOVXUZjIOhLurrRxpEXzI8O0KZHr3IjLvlAH1kTPYSuqer5T9ZVBKQ==
+  dependencies:
+    "@types/estree" "*"
+
 is-unicode-supported@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/is-unicode-supported/-/is-unicode-supported-0.1.0.tgz#3f26c76a809593b52bfa2ecb5710ed2779b522a7"
   integrity sha512-knxG2q4UC3u8stRGyAVJCOdxFmv5DZiRcdlIaAQXAbSfJya+OhopNotLQrstBhququ4ZpuKbDc/8S6mgXgPFPw==
 
+is-wsl@^2.2.0:
+  version "2.2.0"
+  resolved "https://registry.npmmirror.com/is-wsl/-/is-wsl-2.2.0.tgz#74a4c76e77ca9fd3f932f290c17ea326cd157271"
+  integrity sha512-fKzAra0rGJUUBwGBgNkHZuToZcn+TtXHpeCgmkMJMMYx1sQDYaCSyjJBSCa2nH1DGm7s3n1oBnohoVTBaN7Lww==
+  dependencies:
+    is-docker "^2.0.0"
+
 isbinaryfile@^4.0.8:
   version "4.0.10"
   resolved "https://registry.yarnpkg.com/isbinaryfile/-/isbinaryfile-4.0.10.tgz#0c5b5e30c2557a2f06febd37b7322946aaee42b3"
   integrity sha512-iHrqe5shvBUcFbmZq9zOQHBoeOhZJu6RQGrDpBgenUm/Am+F3JM2MgQj+rK3Z601fzrL5gLZWtAPH2OBaSVcyw==
 
 isexe@^2.0.0:
   version "2.0.0"
@@ -1011,23 +1207,37 @@
   integrity sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==
 
 isobject@^3.0.1:
   version "3.0.1"
   resolved "https://registry.yarnpkg.com/isobject/-/isobject-3.0.1.tgz#4e431e92b11a9731636aa1f9c8d1ccbcfdab78df"
   integrity sha512-WhB9zCku7EGTj/HQQRz5aUQEUeoQZH2bWcltRErOpymJ4boYE6wL9Tbr23krRPSZ+C5zqNSrSw+Cc7sZZ4b7vg==
 
+jest-worker@^26.2.1:
+  version "26.6.2"
+  resolved "https://registry.npmmirror.com/jest-worker/-/jest-worker-26.6.2.tgz#7f72cbc4d643c365e27b9fd775f9d0eaa9c7a8ed"
+  integrity sha512-KWYVV1c4i+jbMpaBC+U++4Va0cp8OisU185o73T1vo99hqi7w8tSJfUXYswwqqrjzwxa6KpRK54WhPvwf5w6PQ==
+  dependencies:
+    "@types/node" "*"
+    merge-stream "^2.0.0"
+    supports-color "^7.0.0"
+
 jest-worker@^27.4.5:
   version "27.5.1"
   resolved "https://registry.yarnpkg.com/jest-worker/-/jest-worker-27.5.1.tgz#8d146f0900e8973b106b6f73cc1e9a8cb86f8db0"
   integrity sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==
   dependencies:
     "@types/node" "*"
     merge-stream "^2.0.0"
     supports-color "^8.0.0"
 
+js-tokens@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmmirror.com/js-tokens/-/js-tokens-4.0.0.tgz#19203fb59991df98e3a287050d4647cdeaf32499"
+  integrity sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==
+
 js-yaml@4.1.0:
   version "4.1.0"
   resolved "https://registry.yarnpkg.com/js-yaml/-/js-yaml-4.1.0.tgz#c1fb65f8f5017901cdd2c951864ba18458a10602"
   integrity sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==
   dependencies:
     argparse "^2.0.1"
 
@@ -1152,14 +1362,21 @@
   dependencies:
     date-format "^4.0.14"
     debug "^4.3.4"
     flatted "^3.2.7"
     rfdc "^1.3.0"
     streamroller "^3.1.3"
 
+magic-string@^0.25.7:
+  version "0.25.9"
+  resolved "https://registry.npmmirror.com/magic-string/-/magic-string-0.25.9.tgz#de7f9faf91ef8a1c91d02c2e5314c8277dbcdd1c"
+  integrity sha512-RmF0AsMzgt25qzqqLc1+MbHmhdx0ojF2Fvs4XnOqz2ZOBXzzkEwc/dJQZCYHAn7v1jbVOjAZfK8msRn4BxO4VQ==
+  dependencies:
+    sourcemap-codec "^1.4.8"
+
 media-typer@0.3.0:
   version "0.3.0"
   resolved "https://registry.yarnpkg.com/media-typer/-/media-typer-0.3.0.tgz#8710d7af0aa626f8fffa1ce00168545263255748"
   integrity sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==
 
 merge-stream@^2.0.0:
   version "2.0.0"
@@ -1367,15 +1584,15 @@
   integrity sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==
 
 picocolors@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/picocolors/-/picocolors-1.0.0.tgz#cb5bdc74ff3f51892236eaf79d68bc44564ab81c"
   integrity sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==
 
-picomatch@^2.0.4, picomatch@^2.2.1:
+picomatch@^2.0.4, picomatch@^2.2.1, picomatch@^2.2.2:
   version "2.3.1"
   resolved "https://registry.yarnpkg.com/picomatch/-/picomatch-2.3.1.tgz#3ba3833733646d9d3e4995946c1365a67fb07a42"
   integrity sha512-JU3teHTNjmE2VCGFzuY8EXzCDVwEqB2a8fsIvwaStHhAWJEeVd1o1QD80CU6+ZdEXXSLbSsuLwJjkCBWqRQUVA==
 
 pkg-dir@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/pkg-dir/-/pkg-dir-4.2.0.tgz#f099133df7ede422e81d1d8448270eeb3e4261f3"
@@ -1454,14 +1671,23 @@
     resolve-from "^5.0.0"
 
 resolve-from@^5.0.0:
   version "5.0.0"
   resolved "https://registry.yarnpkg.com/resolve-from/-/resolve-from-5.0.0.tgz#c35225843df8f776df21c57557bc087e9dfdfc69"
   integrity sha512-qYg9KP24dD5qka9J47d0aVky0N+b4fTU89LN9iDnjB5waksiC49rvMB0PrUJQGoTmH50XPiqOvAjDfaijGxYZw==
 
+resolve@^1.17.0, resolve@^1.19.0:
+  version "1.22.2"
+  resolved "https://registry.npmmirror.com/resolve/-/resolve-1.22.2.tgz#0ed0943d4e301867955766c9f3e1ae6d01c6845f"
+  integrity sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==
+  dependencies:
+    is-core-module "^2.11.0"
+    path-parse "^1.0.7"
+    supports-preserve-symlinks-flag "^1.0.0"
+
 resolve@^1.9.0:
   version "1.22.1"
   resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.1.tgz#27cb2ebb53f91abb49470a928bba7558066ac177"
   integrity sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==
   dependencies:
     is-core-module "^2.9.0"
     path-parse "^1.0.7"
@@ -1475,14 +1701,39 @@
 rimraf@^3.0.0, rimraf@^3.0.2:
   version "3.0.2"
   resolved "https://registry.yarnpkg.com/rimraf/-/rimraf-3.0.2.tgz#f1a5402ba6220ad52cc1282bac1ae3aa49fd061a"
   integrity sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==
   dependencies:
     glob "^7.1.3"
 
+rollup-plugin-sourcemaps@^0.6.3:
+  version "0.6.3"
+  resolved "https://registry.npmmirror.com/rollup-plugin-sourcemaps/-/rollup-plugin-sourcemaps-0.6.3.tgz#bf93913ffe056e414419607f1d02780d7ece84ed"
+  integrity sha512-paFu+nT1xvuO1tPFYXGe+XnQvg4Hjqv/eIhG8i5EspfYYPBKL57X7iVbfv55aNVASg3dzWvES9dmWsL2KhfByw==
+  dependencies:
+    "@rollup/pluginutils" "^3.0.9"
+    source-map-resolve "^0.6.0"
+
+rollup-plugin-terser@^7.0.2:
+  version "7.0.2"
+  resolved "https://registry.npmmirror.com/rollup-plugin-terser/-/rollup-plugin-terser-7.0.2.tgz#e8fbba4869981b2dc35ae7e8a502d5c6c04d324d"
+  integrity sha512-w3iIaU4OxcF52UUXiZNsNeuXIMDvFrr+ZXK6bFZ0Q60qyVfq4uLptoS4bbq3paG3x216eQllFZX7zt6TIImguQ==
+  dependencies:
+    "@babel/code-frame" "^7.10.4"
+    jest-worker "^26.2.1"
+    serialize-javascript "^4.0.0"
+    terser "^5.0.0"
+
+rollup@^2.68.0:
+  version "2.79.1"
+  resolved "https://registry.npmmirror.com/rollup/-/rollup-2.79.1.tgz#bedee8faef7c9f93a2647ac0108748f497f081c7"
+  integrity sha512-uKxbd0IhMZOhjAiD5oAFp7BqvkA4Dv47qpOCtaNvng4HBwdbWtdOh8f5nZNuk2rp51PMGk3bzfWu5oayNEuYnw==
+  optionalDependencies:
+    fsevents "~2.3.2"
+
 safe-buffer@^5.1.0:
   version "5.2.1"
   resolved "https://registry.yarnpkg.com/safe-buffer/-/safe-buffer-5.2.1.tgz#1eaf9fa9bdb1fdd4ec75f58f9cdb4e6b7827eec6"
   integrity sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==
 
 "safer-buffer@>= 2.1.2 < 3", "safer-buffer@>= 2.1.2 < 3.0.0":
   version "2.1.2"
@@ -1501,14 +1752,21 @@
 serialize-javascript@6.0.0, serialize-javascript@^6.0.0:
   version "6.0.0"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-6.0.0.tgz#efae5d88f45d7924141da8b5c3a7a7e663fefeb8"
   integrity sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==
   dependencies:
     randombytes "^2.1.0"
 
+serialize-javascript@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmmirror.com/serialize-javascript/-/serialize-javascript-4.0.0.tgz#b525e1238489a5ecfc42afacc3fe99e666f4b1aa"
+  integrity sha512-GaNA54380uFefWghODBWEGisLZFj00nS5ACs6yHa9nLqlLpVLO8ChDGeKRjZnV4Nh4n0Qi7nhYZD/9fCPzEqkw==
+  dependencies:
+    randombytes "^2.1.0"
+
 setprototypeof@1.2.0:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/setprototypeof/-/setprototypeof-1.2.0.tgz#66c9a24a73f9fc28cbe66b09fed3d33dcaf1b424"
   integrity sha512-E5LDX7Wrp85Kil5bhZv46j8jOeboKq5JMmYM3gVGdGH8xFpPWXUMsNrlODCrkoxMEeNi/XZIwuRvY4XNwYMJpw==
 
 shallow-clone@^3.0.0:
   version "3.0.1"
@@ -1573,27 +1831,40 @@
   resolved "https://registry.yarnpkg.com/source-map-loader/-/source-map-loader-4.0.0.tgz#bdc6b118bc6c87ee4d8d851f2d4efcc5abdb2ef5"
   integrity sha512-i3KVgM3+QPAHNbGavK+VBq03YoJl24m9JWNbLgsjTj8aJzXG9M61bantBTNBt7CNwY2FYf+RJRYJ3pzalKjIrw==
   dependencies:
     abab "^2.0.6"
     iconv-lite "^0.6.3"
     source-map-js "^1.0.2"
 
+source-map-resolve@^0.6.0:
+  version "0.6.0"
+  resolved "https://registry.npmmirror.com/source-map-resolve/-/source-map-resolve-0.6.0.tgz#3d9df87e236b53f16d01e58150fc7711138e5ed2"
+  integrity sha512-KXBr9d/fO/bWo97NXsPIAW1bFSBOuCnjbNTBMO7N59hsv5i9yzRDfcYwwt0l04+VqnKC+EwzvJZIP/qkuMgR/w==
+  dependencies:
+    atob "^2.1.2"
+    decode-uri-component "^0.2.0"
+
 source-map-support@0.5.21, source-map-support@~0.5.20:
   version "0.5.21"
   resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.21.tgz#04fe7c7f9e1ed2d662233c28cb2b35b9f63f6e4f"
   integrity sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==
   dependencies:
     buffer-from "^1.0.0"
     source-map "^0.6.0"
 
 source-map@^0.6.0, source-map@^0.6.1:
   version "0.6.1"
   resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.6.1.tgz#74722af32e9614e9c287a8d0bbde48b5e2f1a263"
   integrity sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==
 
+sourcemap-codec@^1.4.8:
+  version "1.4.8"
+  resolved "https://registry.npmmirror.com/sourcemap-codec/-/sourcemap-codec-1.4.8.tgz#ea804bd94857402e6992d05a38ef1ae35a9ab4c4"
+  integrity sha512-9NykojV5Uih4lgo5So5dtw+f0JgJX30KCNI8gwhz2J9A15wD0Ml6tjHKwf6fTSa6fAdVBdZeNOs9eJ71qCk8vA==
+
 statuses@2.0.1:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/statuses/-/statuses-2.0.1.tgz#55cb000ccf1d48728bd23c685a063998cf1a1b63"
   integrity sha512-RwNA9Z/7PrK06rYLIzFMlaF+l73iwpzsqRIFgbMLbTcLD6cOao82TaWefPXQvB2fOC4AjuYSEndS7N/mTCbkdQ==
 
 statuses@~1.5.0:
   version "1.5.0"
@@ -1633,15 +1904,22 @@
 supports-color@8.1.1, supports-color@^8.0.0:
   version "8.1.1"
   resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-8.1.1.tgz#cd6fc17e28500cff56c1b86c0a7fd4a54a73005c"
   integrity sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==
   dependencies:
     has-flag "^4.0.0"
 
-supports-color@^7.1.0:
+supports-color@^5.3.0:
+  version "5.5.0"
+  resolved "https://registry.npmmirror.com/supports-color/-/supports-color-5.5.0.tgz#e2e69a44ac8772f78a1ec0b35b689df6530efc8f"
+  integrity sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==
+  dependencies:
+    has-flag "^3.0.0"
+
+supports-color@^7.0.0, supports-color@^7.1.0:
   version "7.2.0"
   resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-7.2.0.tgz#1b7dcdcb32b8138801b3e478ba6a51caa89648da"
   integrity sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==
   dependencies:
     has-flag "^4.0.0"
 
 supports-preserve-symlinks-flag@^1.0.0:
@@ -1661,14 +1939,24 @@
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.14"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.0"
     terser "^5.14.1"
 
+terser@^5.0.0:
+  version "5.17.3"
+  resolved "https://registry.npmmirror.com/terser/-/terser-5.17.3.tgz#7f908f16b3cdf3f6c0f8338e6c1c674837f90d25"
+  integrity sha512-AudpAZKmZHkG9jueayypz4duuCFJMMNGRMwaPvQKWfxKedh8Z2x3OCoDqIIi1xx5+iwx1u6Au8XQcc9Lke65Yg==
+  dependencies:
+    "@jridgewell/source-map" "^0.3.2"
+    acorn "^8.5.0"
+    commander "^2.20.0"
+    source-map-support "~0.5.20"
+
 terser@^5.14.1:
   version "5.16.0"
   resolved "https://registry.yarnpkg.com/terser/-/terser-5.16.0.tgz#29362c6f5506e71545c73b069ccd199bb28f7f54"
   integrity sha512-KjTV81QKStSfwbNiwlBXfcgMcOloyuRdb62/iLFPGBcVNF4EXjhdYBhYHmbJpiBrVxZhDvltE11j+LBQUxEEJg==
   dependencies:
     "@jridgewell/source-map" "^0.3.2"
     acorn "^8.5.0"
@@ -1690,22 +1978,37 @@
     is-number "^7.0.0"
 
 toidentifier@1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/toidentifier/-/toidentifier-1.0.1.tgz#3be34321a88a820ed1bd80dfaa33e479fbb8dd35"
   integrity sha512-o5sSPKEkg/DIQNmH43V0/uerLrpzVedkUh8tGNvaeXpfpuwjKenlSox/2O/BTlZUtEe+JG7s5YhEz608PlAHRA==
 
+tslib@^2.3.1:
+  version "2.5.0"
+  resolved "https://registry.npmmirror.com/tslib/-/tslib-2.5.0.tgz#42bfed86f5787aeb41d031866c8f402429e0fddf"
+  integrity sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==
+
 type-is@~1.6.18:
   version "1.6.18"
   resolved "https://registry.yarnpkg.com/type-is/-/type-is-1.6.18.tgz#4e552cd05df09467dcbc4ef739de89f2cf37c131"
   integrity sha512-TkRKr9sUTxEH8MdfuCSP7VizJyzRNMjj2J2do2Jr3Kym598JVdEksuzPQCnlFPW4ky9Q+iA+ma9BGm06XQBy8g==
   dependencies:
     media-typer "0.3.0"
     mime-types "~2.1.24"
 
+typescript@4.7.4:
+  version "4.7.4"
+  resolved "https://registry.npmmirror.com/typescript/-/typescript-4.7.4.tgz#1a88596d1cf47d59507a1bcdfb5b9dfe4d488235"
+  integrity sha512-C0WQT0gezHuw6AdY1M2jxUO83Rjf0HP7Sk1DtXj6j1EwkQNZrHAg2XPWlq62oqEhYvONq5pkC2Y9oPljWToLmQ==
+
+typescript@^3.7.2:
+  version "3.9.10"
+  resolved "https://registry.npmmirror.com/typescript/-/typescript-3.9.10.tgz#70f3910ac7a51ed6bef79da7800690b19bf778b8"
+  integrity sha512-w6fIxVE/H1PkLKcCPsFqKE7Kv7QUwhU8qQY2MueZXWx5cPZdwFupLgKK3vntcK98BtNHZtAF4LA/yl2a7k8R6Q==
+
 ua-parser-js@^0.7.30:
   version "0.7.32"
   resolved "https://registry.yarnpkg.com/ua-parser-js/-/ua-parser-js-0.7.32.tgz#cd8c639cdca949e30fa68c44b7813ef13e36d211"
   integrity sha512-f9BESNVhzlhEFf2CHMSj40NWOjYPl1YKYbrvIr/hFTDEmLq7SRbWvm7FcdcpCYT95zrOhC7gZSxjdnnTpBcwVw==
 
 universalify@^0.1.0:
   version "0.1.2"
@@ -1743,17 +2046,17 @@
   integrity sha512-BNGbWLfd0eUPabhkXUVm0j8uuvREyTh5ovRa/dyow/BqAbZJyC+5fU+IzQOzmAKzYqYRAISoRhdQr3eIZ/PXqg==
 
 void-elements@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/void-elements/-/void-elements-2.0.1.tgz#c066afb582bb1cb4128d60ea92392e94d5e9dbec"
   integrity sha512-qZKX4RnBzH2ugr8Lxa7x+0V6XD9Sb/ouARtiasEQCHB1EVU4NXtmHsDDrx1dO4ne5fc3J6EW05BP1Dl0z0iung==
 
-watchpack@^2.3.1:
+watchpack@^2.4.0:
   version "2.4.0"
-  resolved "https://registry.yarnpkg.com/watchpack/-/watchpack-2.4.0.tgz#fa33032374962c78113f93c7f2fb4c54c9862a5d"
+  resolved "https://registry.npmmirror.com/watchpack/-/watchpack-2.4.0.tgz#fa33032374962c78113f93c7f2fb4c54c9862a5d"
   integrity sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==
   dependencies:
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.1.2"
 
 webpack-cli@4.10.0:
   version "4.10.0"
@@ -1789,42 +2092,42 @@
     wildcard "^2.0.0"
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
-webpack@5.73.0:
-  version "5.73.0"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.73.0.tgz#bbd17738f8a53ee5760ea2f59dce7f3431d35d38"
-  integrity sha512-svjudQRPPa0YiOYa2lM/Gacw0r6PvxptHj4FuEKQ2kX05ZLkjbVc5MnPs6its5j7IZljnIqSVo/OsY2X0IpHGA==
+webpack@5.74.0:
+  version "5.74.0"
+  resolved "https://registry.npmmirror.com/webpack/-/webpack-5.74.0.tgz#02a5dac19a17e0bb47093f2be67c695102a55980"
+  integrity sha512-A2InDwnhhGN4LYctJj6M1JEaGL7Luj6LOmyBHjcI8529cm5p6VXiTIW2sn6ffvEAKmveLzvu4jrihwXtPojlAA==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^0.0.51"
     "@webassemblyjs/ast" "1.11.1"
     "@webassemblyjs/wasm-edit" "1.11.1"
     "@webassemblyjs/wasm-parser" "1.11.1"
-    acorn "^8.4.1"
+    acorn "^8.7.1"
     acorn-import-assertions "^1.7.6"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.9.3"
+    enhanced-resolve "^5.10.0"
     es-module-lexer "^0.9.0"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.2.9"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
     schema-utils "^3.1.0"
     tapable "^2.1.1"
     terser-webpack-plugin "^5.1.3"
-    watchpack "^2.3.1"
+    watchpack "^2.4.0"
     webpack-sources "^3.2.3"
 
 which@^1.2.1:
   version "1.3.1"
   resolved "https://registry.yarnpkg.com/which/-/which-1.3.1.tgz#a45043d54f5805316da8d62f9f50918d3da70b0a"
   integrity sha512-HxJdYWq1MTIQbJ3nw0cqssHoTNU267KlrDuGZ1WYlxDStUtKUhOaJmh112/TZmHxxUfuJqPXSOm7tDyas0OSIQ==
   dependencies:
```

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/build.gradle.kts` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/build.gradle.kts`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 plugins {
-    kotlin("multiplatform") version "1.7.21"
-    kotlin("plugin.serialization") version "1.7.21"
+    kotlin("multiplatform") version "1.8.21"
+    kotlin("plugin.serialization") version "1.8.10"
     id("dev.petuska.npm.publish") version "3.2.0"
 }
 
 group = rootProject.group
 version = rootProject.version
 
 repositories {
@@ -46,25 +46,25 @@
         }
     }
 
     sourceSets {
         val commonMain by getting {
             dependencies {
                 implementation(rootProject)
-                implementation("org.jetbrains.kotlinx:kotlinx-serialization-core:1.4.1")
+                implementation("org.jetbrains.kotlinx:kotlinx-serialization-core:1.5.0")
             }
         }
         val commonTest by getting {
             dependencies {
                 implementation(kotlin("test"))
             }
         }
         val nativeMain by getting {
             dependencies {
-                implementation("org.jetbrains.kotlinx:kotlinx-serialization-json:1.4.1")
+                implementation("org.jetbrains.kotlinx:kotlinx-serialization-json:1.5.0")
             }
         }
         val jsMain by getting {
             dependencies {
                 implementation("org.jetbrains.kotlinx:kotlinx-serialization-json:1.4.1")
             }
         }
```

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         // 十三面
         13 - yaochu.size
     }
 }
 
 internal val TILE_CLING = buildMap<Tile, Set<Tile>> {
     repeat(3) {
-        val type = TileType.values()[it]
+        val type = TileType.valueOf(it)
         for (j in 1..9) {
             val t = Tile.get(type, j)
             this[t] = listOf(-2, -1, 0, 1, 2)
                 .filter { k -> j + k in 1..9 }
                 .map { k -> Tile.get(type, j + k) }
                 .toSet()
         }
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 // 这里用的编码和Tile.code不一样
 private fun encode(t: Tile): Int {
     return t.type.ordinal * 9 + t.realNum - 1
 }
 
 private fun decode(code: Int): Tile {
-    val type = TileType.values()[code / 9]
+    val type = TileType.valueOf(code / 9)
     val num = code % 9 + 1
     return Tile.get(type, num)
 }
 
 private class RegularHandPatternSearcher(
     tiles: List<Tile>,
     private val furo: List<Furo> = emptyList(),
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     tiles: List<Tile>, furo: List<Furo> = emptyList(), agari: Tile, tsumo: Boolean,
     dora: Int = 0, selfWind: Wind? = null, roundWind: Wind? = null, extraYaku: Set<Yaku> = emptySet()
 ): Hora {
     if (tiles.size / 3 + furo.size != 4) {
         throw IllegalArgumentException("invalid length of tiles")
     }
 
-    val shantenResult = shanten(tiles, furo, false)
+    val shantenResult = shanten(tiles, furo, calcAdvanceNum = false, bestShantenOnly = true, allowAnkan = false)
     return hora(shantenResult, agari, tsumo, dora, selfWind, roundWind, extraYaku)
 
 }
 
 /**
  * 和牌分析
  *
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,27 @@
      * 索
      */
     S,
 
     /**
      * 字
      */
-    Z
+    Z;
+
+    companion object {
+        fun valueOf(ordinal: Int): TileType {
+            return when (ordinal) {
+                0 -> M
+                1 -> P
+                2 -> S
+                3 -> Z
+                else -> throw IllegalArgumentException("invalid ordinal value: $ordinal")
+            }
+        }
+    }
 }
 
 /**
  * 麻将牌
  */
 @Serializable(with = TileSerializer::class)
 data class Tile private constructor(
@@ -204,15 +216,15 @@
          * 所有牌
          */
         val all = pool.filterNotNull().toSet()
 
         /**
          * 所有牌
          */
-        val allExcludeAkaDora = all.filter { it.num != 0 }
+        val allExcludeAkaDora = all.filter { it.num != 0 }.toSet()
 
         /**
          * 所有幺九牌
          */
         val allYaochu = buildSet<Tile> {
             for (type in listOf(TileType.M, TileType.P, TileType.S)) {
                 add(get(type, 1))
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 package mahjongutils.shanten
 
 import mahjongutils.models.Tile
-import mahjongutils.models.countAsCodeArray
 import mahjongutils.models.countAsMap
 import mahjongutils.models.hand.ChitoiHandPattern
 import mahjongutils.models.hand.Hand
 
 private fun buildChitoiPattern(tiles: List<Tile>): ChitoiHandPattern {
     val cnt = tiles.countAsMap()
 
@@ -40,19 +39,17 @@
         shantenNum = 6 - pattern.pairs.size
         advance = (pattern.remaining - pattern.pairs).toSet()
     } else {
         shantenNum = 6 - pattern.pairs.size + (7 - tileSet.size)
         advance = (Tile.allExcludeAkaDora - pattern.pairs).toSet()
     }
 
-    val goodShapeAdvance = if (shantenNum == 1) emptySet<Tile>() else null
     val shantenInfo = ShantenWithoutGot(
         shantenNum = shantenNum,
-        advance = advance.toSet(),
-        goodShapeAdvance = goodShapeAdvance
+        advance = advance.toSet()
     )
     return Pair(shantenInfo, pattern)
 }
 
 private fun handleChitoiShantenWithGot(
     tiles: List<Tile>,
     bestShantenOnly: Boolean = false
@@ -116,13 +113,13 @@
     var (shantenInfo, pattern) = if (tiles.size == 13) {
         handleChitoiShantenWithoutGot(tiles)
     } else {
         handleChitoiShantenWithGot(tiles, bestShantenOnly)
     }
 
     if (calcAdvanceNum) {
-        shantenInfo = shantenInfo.fillAdvanceNum(tiles.countAsCodeArray())
+        shantenInfo = shantenInfo.fillNum(getTileCount(tiles))
     }
 
     val hand = Hand(tiles = tiles, furo = emptyList(), patterns = listOf(pattern))
     return ChitoiShantenResult(hand = hand, shantenInfo = shantenInfo)
 }
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
  */
 fun furoChanceShanten(
     tiles: List<Tile>,
     chanceTile: Tile,
     allowChi: Boolean = true,
     bestShantenOnly: Boolean = false,
     allowKuikae: Boolean = false
-): FuroChanceShantenResult = furoChanceShanten(tiles, chanceTile, allowChi, true, bestShantenOnly, allowKuikae)
+): FuroChanceShantenResult = furoChanceShanten(
+    tiles, chanceTile, allowChi, true, bestShantenOnly, allowKuikae
+)
 
 /**
  * 副露判断向听分析
  * @param tiles 门前的牌
  * @param chanceTile 副露机会牌（能够吃、碰的牌）
  * @param allowChi 是否允许吃
  * @param calcAdvanceNum 是否计算进张数
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     val patterns = buildKokushiPattern(tiles)
     val (shantenNum, bestPatterns) = selectBestPatterns(patterns, KokushiHandPattern::calcShanten)
 
     val pat = bestPatterns.first()
     if (pat.repeated != null) {
         // 非十三面
         val advance = Tile.allYaochu - pat.yaochu
-        val goodShapeAdvance = if (shantenNum == 1) emptySet<Tile>() else null
-        val shantenInfo = ShantenWithoutGot(shantenNum, advance, goodShapeAdvance = goodShapeAdvance)
+        val shantenInfo = ShantenWithoutGot(shantenNum, advance)
         return Pair(shantenInfo, bestPatterns)
     } else {
         // 十三面
         val advance = Tile.allYaochu
         val goodShapeAdvance = if (shantenNum == 1) advance else null
         val shantenInfo = ShantenWithoutGot(shantenNum, advance, goodShapeAdvance = goodShapeAdvance)
         return Pair(shantenInfo, bestPatterns)
@@ -116,13 +115,13 @@
     var (shantenInfo, patterns) = if (tiles.size == 13) {
         handleKokushiShantenWithoutGot(tiles)
     } else {
         handleKokushiShantenWithGot(tiles, bestShantenOnly)
     }
 
     if (calcAdvanceNum) {
-        shantenInfo = shantenInfo.fillAdvanceNum(tiles.countAsCodeArray())
+        shantenInfo = shantenInfo.fillNum(tiles.countAsCodeArray())
     }
 
     val hand = Hand(tiles = tiles, furo = emptyList(), patterns = patterns)
     return KokushiShantenResult(hand = hand, shantenInfo = shantenInfo)
 }
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 package mahjongutils.shanten
 
+import mahjongutils.models.Furo
 import mahjongutils.models.Tile
+import mahjongutils.models.countAsCodeArray
 import mahjongutils.models.hand.HandPattern
 
 
 internal fun ensureLegalTiles(
     tiles: List<Tile>,
     allowAnyK: Boolean = true,
     allowWithGot: Boolean = true,
@@ -49,37 +51,53 @@
             bestPattern.add(pat)
         }
     }
 
     return Pair(bestShanten, bestPattern)
 }
 
-private fun ShantenWithoutGot.fillAdvanceNumByRemaining(remaining: IntArray): ShantenWithoutGot {
-    val advanceNum = advance.sumOf { remaining[it.code] }
-    val goodShapeAdvanceNum = goodShapeAdvance?.sumOf { remaining[it.code] }
-
-    return copy(advanceNum = advanceNum, goodShapeAdvanceNum = goodShapeAdvanceNum)
+internal fun getTileCount(tiles: Collection<Tile>, furo: Collection<Furo> = emptyList()): IntArray {
+    return (tiles + furo.flatMap { it.tiles }).countAsCodeArray()
 }
 
-internal inline fun <reified T : Shanten> T.fillAdvanceNum(tileCount: IntArray): T {
+internal fun getRemainingFromTileCount(tileCount: IntArray): IntArray {
     val remaining = IntArray(Tile.MAX_TILE_CODE + 1) { 4 }
     for (i in tileCount.indices) {
         remaining[i] -= tileCount[i]
     }
+    return remaining
+}
+
+internal inline fun <reified T : CommonShanten> T.fillNum(tileCount: IntArray): T {
+    val remaining = getRemainingFromTileCount(tileCount)
+    return fillNumByRemaining(remaining)
+}
 
+internal fun <T : CommonShanten> T.fillNumByRemaining(remaining: IntArray): T {
     return when (this) {
         is ShantenWithoutGot -> {
-            this.fillAdvanceNumByRemaining(remaining) as T
+            copy(
+                advanceNum = advance.sumOf { remaining[it.code] },
+                goodShapeAdvanceNum = goodShapeAdvance?.sumOf { remaining[it.code] },
+                improvement = improvement?.mapValues { (k, v) ->
+                    remaining[k.code] -= 1
+                    val v = v.map { imp -> imp.copy(advanceNum = imp.advance.sumOf { remaining[it.code] }) }.toSet()
+                    remaining[k.code] += 1
+
+                    v
+                },
+                improvementNum = improvement?.keys?.sumOf { remaining[it.code] }
+            ) as T
         }
 
         is ShantenWithGot -> {
             copy(
-                discardToAdvance = discardToAdvance.mapValues { (k, v) -> v.fillAdvanceNumByRemaining(remaining) },
-                ankanToAdvance = ankanToAdvance.mapValues { (k, v) -> v.fillAdvanceNumByRemaining(remaining) },
+                discardToAdvance = discardToAdvance.mapValues { (_, v) -> v.fillNumByRemaining(remaining) },
+                ankanToAdvance = ankanToAdvance.mapValues { (_, v) -> v.fillNumByRemaining(remaining) },
             ) as T
         }
 
         else -> {
             error("unexpected type")
         }
     }
-}
+}
```

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt` & `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,18 @@
     @Test
     fun test9() {
         val hora = hora(
             tiles = Tile.parseTiles("111122223333m99s"),
             agari = Tile.get("9s"),
             tsumo = false
         )
+        assertEquals(hora.han, 3)
+        assertEquals(hora.hu, 40)
+        assertEquals(ParentPoint(7700, 0), hora.parentPoint)
+        assertEquals(ChildPoint(5200, 0, 0), hora.childPoint)
     }
 
     @Test
     fun test10() {
         val hora = hora(
             tiles = Tile.parseTiles("234p11z"),
             furo = listOf(Furo("0110s"), Furo("0110m"), Furo("0990m")),
```

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt`

 * *Files 15% similar despite different names*

```diff
@@ -8,30 +8,40 @@
 
 class TestFuroChanceShanten {
     @Test
     fun test1() {
         val result = furoChanceShanten(Tile.parseTiles("8999m"), Tile.get("9m"))
         assertEquals(0, result.shantenInfo.shantenNum)
 
-        val shantenInfo = result.shantenInfo as ShantenWithFuroChance
+        val shantenInfo = result.shantenInfo
         assertEquals(
             ShantenWithoutGot(
                 shantenNum = 0,
                 advance = Tile.parseTiles("78m").toSet(),
                 advanceNum = 7
             ), shantenInfo.pass
         )
         assertEquals(
             ShantenWithGot(
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("8m") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = setOf(),
-                        advanceNum = 0
+                        advanceNum = 0,
+                        improvement = Tile.allExcludeAkaDora.filter { it !== Tile.get("9m") }.associateWith {
+                            setOf(
+                                Improvement(
+                                    discard = Tile.get("9m"),
+                                    advance = setOf(it),
+                                    advanceNum = if (it == Tile.get("8m")) 2 else 3
+                                )
+                            )
+                        },
+                        improvementNum = 131,
                     ),
                     Tile.get("9m") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = setOf(Tile.get("8m")),
                         advanceNum = 3
                     )
                 )
```

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,37 @@
 import kotlin.test.assertEquals
 
 class TestShanten {
     private fun tester(
         tiles: String, expected: Shanten,
         calcAdvanceNum: Boolean = true,
         bestShantenOnly: Boolean = false,
+        calcImprovement: Boolean = true,
     ) {
-        val result = shanten(Tile.parseTiles(tiles), emptyList(), calcAdvanceNum, bestShantenOnly)
+        val result = shanten(
+            Tile.parseTiles(tiles),
+            emptyList(),
+            calcAdvanceNum = calcAdvanceNum,
+            bestShantenOnly = bestShantenOnly,
+            calcImprovement = calcImprovement
+        )
         assertEquals(expected, result.shantenInfo)
     }
 
     private fun regularTester(
         tiles: String, expected: Shanten,
         calcAdvanceNum: Boolean = true,
         bestShantenOnly: Boolean = false,
     ) {
-        val result = regularShanten(Tile.parseTiles(tiles), emptyList(), calcAdvanceNum, bestShantenOnly)
+        val result = regularShanten(
+            Tile.parseTiles(tiles),
+            emptyList(),
+            calcAdvanceNum = calcAdvanceNum,
+            bestShantenOnly = bestShantenOnly
+        )
         assertEquals(expected, result.shantenInfo)
     }
 
     private fun chitoiTester(
         tiles: String, expected: Shanten,
         calcAdvanceNum: Boolean = true,
         bestShantenOnly: Boolean = false,
@@ -101,18 +113,72 @@
                 advance = Tile.parseTiles("36s12z").toSet(),
                 advanceNum = 13,
                 goodShapeAdvance = Tile.parseTiles("12z").toSet(),
                 goodShapeAdvanceNum = 6
             )
         )
         tester(
+            "22s23455666p345m", ShantenWithoutGot(
+                shantenNum = 0,
+                advance = Tile.parseTiles("5p2s").toSet(),
+                advanceNum = 4,
+                improvement = mapOf(
+                    Tile.get("1p") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("47p").toSet(),
+                            advanceNum = 7
+                        )
+                    ),
+                    Tile.get("3p") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("5p"),
+                            advance = Tile.parseTiles("14p").toSet(),
+                            advanceNum = 7
+                        )
+                    ),
+                    Tile.get("4p") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 10
+                        )
+                    ),
+                    Tile.get("6p") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("5p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 11
+                        )
+                    ),
+                    Tile.get("7p") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 10
+                        )
+                    ),
+                    Tile.get("3s") to setOf(
+                        Improvement(
+                            discard = Tile.Companion.get("2s"),
+                            advance = Tile.parseTiles("14s").toSet(),
+                            advanceNum = 8
+                        )
+                    ),
+                ),
+                improvementNum = 19
+            )
+        )
+        tester(
             "1112345678999p", ShantenWithoutGot(
                 shantenNum = 0,
                 advance = Tile.parseTiles("123456789p").toSet(),
-                advanceNum = 23
+                advanceNum = 23,
+                improvement = emptyMap(),
+                improvementNum = 0
             )
         )
         tester(
             "114514p1919810s", ShantenWithoutGot(
                 shantenNum = 2,
                 advance = Tile.parseTiles("234567p3456789s").toSet(),
                 advanceNum = 45,
@@ -140,14 +206,16 @@
             )
         )
         kokushiTester(
             "119m19p19s123456z", ShantenWithoutGot(
                 shantenNum = 0,
                 advance = Tile.parseTiles("7z").toSet(),
                 advanceNum = 4,
+                improvement = emptyMap(),
+                improvementNum = 0
             )
         )
         chitoiTester(
             "1111223344556z", ShantenWithoutGot(
                 shantenNum = 2,
                 advance = (Tile.all.filter { it.num != 0 } - Tile.parseTiles("12345z").toSet()).toSet(),
                 advanceNum = 115
@@ -164,35 +232,198 @@
                         shantenNum = 0,
                         advance = Tile.parseTiles("1567s").toSet(),
                         advanceNum = 11
                     ),
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1357s").toSet(),
-                        advanceNum = 9
+                        advanceNum = 9,
+                        improvement = mapOf(
+                            Tile.get("2s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("6s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12567s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                        ),
+                        improvementNum = 5
                     ),
                     Tile.get("5s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("17s").toSet(),
-                        advanceNum = 7
+                        advanceNum = 7,
+                        improvement = mapOf(
+                            Tile.get("2s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("1s"),
+                                    advance = Tile.parseTiles("23567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("3s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("1s"),
+                                    advance = Tile.parseTiles("267s").toSet(),
+                                    advanceNum = 9
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("127s").toSet(),
+                                    advanceNum = 9
+                                ),
+                            ),
+                            Tile.get("5s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("6s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                        ),
+                        improvementNum = 7
                     ),
                     Tile.get("6s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1235s").toSet(),
-                        advanceNum = 7
+                        advanceNum = 7,
+                        improvement = mapOf(
+                            Tile.get("6s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            )
+                        ),
+                        improvementNum = 3
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("25s").toSet(),
-                        advanceNum = 3
+                        advanceNum = 3,
+                        improvement = mapOf(
+                            Tile.get("1s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("3s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("4s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12567s").toSet(),
+                                    advanceNum = 13
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("12367s").toSet(),
+                                    advanceNum = 13
+                                )
+                            ),
+                            Tile.get("6s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("2367s").toSet(),
+                                    advanceNum = 9
+                                )
+                            ),
+                            Tile.get("7s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("13578s").toSet(),
+                                    advanceNum = 12
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("12367s").toSet(),
+                                    advanceNum = 12
+                                ),
+                            ),
+                            Tile.get("8s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("78s").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        improvementNum = 15
                     ),
                     Tile.get("4s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("25s").toSet(),
-                        advanceNum = 3
+                        advanceNum = 3,
+                        improvement = mapOf(
+                            Tile.get("1s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("124567s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("3s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("4567s").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("4s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("6s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12456s").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("7s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("134578s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("8s") to setOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("78s").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        improvementNum = 15
                     ),
                 ), ankanToAdvance = mapOf(
                     Tile.get("4s") to ShantenWithoutGot(
                         shantenNum = 1,
                         advance = Tile.parseTiles("1235678s").toSet(),
                         advanceNum = 18,
                         goodShapeAdvance = Tile.parseTiles("1237s").toSet(),
@@ -324,29 +555,37 @@
         tester(
             "1112345678999s1z", ShantenWithGot(
                 shantenNum = 0, discardToAdvance = mapOf(
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("5s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("8s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("1z") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("123456789s").toSet(),
                         advanceNum = 23,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 1,
                         advance = Tile.parseTiles("123456789s1z").toSet(),
                         advanceNum = 26,
                         goodShapeAdvance = Tile.parseTiles("1234679s1z").toSet(),
                         goodShapeAdvanceNum = 20
@@ -383,15 +622,16 @@
                         shantenNum = 1,
                         advance = Tile.parseTiles("123456789s1z").toSet(),
                         advanceNum = 26,
                         goodShapeAdvance = Tile.parseTiles("1346789s1z").toSet(),
                         goodShapeAdvanceNum = 20
                     ),
                 )
-            )
+            ),
+            calcImprovement = false
         )
         tester(
             "11123456789999p", ShantenWithGot(
                 shantenNum = -1,
                 discardToAdvance = emptyMap()
             ),
             bestShantenOnly = true
@@ -507,88 +747,143 @@
                         advance = Tile.parseTiles("5p8p5s8s").toSet(),
                         advanceNum = 12,
                     ),
                 )
             )
         )
         tester(
-            "111p456p123s678p23s", ShantenWithGot(
+            "111456678p12233s",
+            ShantenWithGot(
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("1p") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("14s").toSet(),
                         advanceNum = 7,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("23s").toSet(),
                         advanceNum = 4,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("3s").toSet(),
                         advanceNum = 2,
+                        improvement = null,
+                        improvementNum = null
                     ),
                     Tile.get("3s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("2s").toSet(),
                         advanceNum = 2,
-                    ),
-                    Tile.get("6p") to ShantenWithoutGot(
-                        shantenNum = 1,
-                        advance = Tile.parseTiles("3456789p1234s").toSet(),
-                        advanceNum = 33,
-                        goodShapeAdvance = Tile.parseTiles("3456789p1234s").toSet(),
-                        goodShapeAdvanceNum = 33,
-                    ),
-                    Tile.get("4p") to ShantenWithoutGot(
-                        shantenNum = 1,
-                        advance = Tile.parseTiles("4p5p6p7p8p9p1s2s3s4s").toSet(),
-                        advanceNum = 29,
-                        goodShapeAdvance = Tile.parseTiles("4p5p6p7p8p9p1s2s3s4s").toSet(),
-                        goodShapeAdvanceNum = 29,
-                    ),
-                    Tile.get("8p") to ShantenWithoutGot(
-                        shantenNum = 1,
-                        advance = Tile.parseTiles("3p4p5p6p7p8p1s2s3s4s").toSet(),
-                        advanceNum = 29,
-                        goodShapeAdvance = Tile.parseTiles("3p4p5p6p7p8p1s2s3s4s").toSet(),
-                        goodShapeAdvanceNum = 29,
-                    ),
-                    Tile.get("5p") to ShantenWithoutGot(
-                        shantenNum = 1,
-                        advance = Tile.parseTiles("4p5p6p9p1s2s3s4s").toSet(),
-                        advanceNum = 23,
-                        goodShapeAdvance = Tile.parseTiles("4p5p6p9p1s4s").toSet(),
-                        goodShapeAdvanceNum = 19,
-                    ),
-                    Tile.get("7p") to ShantenWithoutGot(
-                        shantenNum = 1,
-                        advance = Tile.parseTiles("3p6p7p8p1s2s3s4s").toSet(),
-                        advanceNum = 23,
-                        goodShapeAdvance = Tile.parseTiles("3p6p7p8p1s4s").toSet(),
-                        goodShapeAdvanceNum = 19,
-                    ),
+                        improvement = null,
+                        improvementNum = null
+                    )
                 )
-            )
+            ),
+            bestShantenOnly = true,
+            calcImprovement = false
         )
         tester(
             "4456m3334556p345s", ShantenWithGot(
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("4m") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("457p").toSet(),
                         advanceNum = 9,
+                        improvement = mapOf(
+                            Tile.get("2p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("5p"),
+                                    advance = Tile.parseTiles("1247p").toSet(),
+                                    advanceNum = 14
+                                )
+                            )
+                        ),
+                        improvementNum = 4
                     ),
                     Tile.get("5p") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("47m").toSet(),
                         advanceNum = 6,
+                        improvement = mapOf(
+                            Tile.get("3m") to setOf(
+                                Improvement(
+                                    discard = Tile.get("6p"),
+                                    advance = Tile.parseTiles("25m").toSet(),
+                                    advanceNum = 7
+                                ),
+                                Improvement(
+                                    discard = Tile.get("3p"),
+                                    advance = Tile.parseTiles("25m").toSet(),
+                                    advanceNum = 7
+                                ),
+                            ),
+                            Tile.get("5m") to setOf(
+                                Improvement(
+                                    discard = Tile.get("6p"),
+                                    advance = Tile.parseTiles("36m").toSet(),
+                                    advanceNum = 7
+                                ),
+                                Improvement(
+                                    discard = Tile.get("3p"),
+                                    advance = Tile.parseTiles("36m").toSet(),
+                                    advanceNum = 7
+                                ),
+                            ),
+                            Tile.get("1p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("12p").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                            Tile.get("2p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("1247p").toSet(),
+                                    advanceNum = 14
+                                )
+                            ),
+                            Tile.get("4p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("2457p").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("5p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("457p").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("7p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("24578p").toSet(),
+                                    advanceNum = 16
+                                )
+                            ),
+                            Tile.get("8p") to setOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("78p").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        improvementNum = 28
                     ),
                 )
             ),
             bestShantenOnly = true
         )
         tester(
             "35m11223399p7799s", ShantenWithGot(
```

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt` & `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/hora/hora.py` & `mahjong-utils-0.5.0/mahjong_utils/hora/hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/hora/models.py` & `mahjong-utils-0.5.0/mahjong_utils/hora/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/lib/__init__.py` & `mahjong-utils-0.5.0/mahjong_utils/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/lib/libmahjongutils_api.i` & `mahjong-utils-0.5.0/mahjong_utils/lib/libmahjongutils_api.i`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,26 @@
   libmahjongutils_KNativePtr pinned;
 } libmahjongutils_kref_kotlin_Boolean;
 typedef struct {
   libmahjongutils_KNativePtr pinned;
 } libmahjongutils_kref_kotlin_Unit;
 typedef struct {
   libmahjongutils_KNativePtr pinned;
+} libmahjongutils_kref_kotlin_UByte;
+typedef struct {
+  libmahjongutils_KNativePtr pinned;
+} libmahjongutils_kref_kotlin_UShort;
+typedef struct {
+  libmahjongutils_KNativePtr pinned;
+} libmahjongutils_kref_kotlin_UInt;
+typedef struct {
+  libmahjongutils_KNativePtr pinned;
+} libmahjongutils_kref_kotlin_ULong;
+typedef struct {
+  libmahjongutils_KNativePtr pinned;
 } libmahjongutils_kref_mahjongutils_Entry;
 typedef struct {
   libmahjongutils_KNativePtr pinned;
 } libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs;
 typedef struct {
   libmahjongutils_KNativePtr pinned;
 } libmahjongutils_kref_kotlin_collections_List;
@@ -126,33 +138,61 @@
 
 typedef struct {
 
   void (*DisposeStablePointer)(libmahjongutils_KNativePtr ptr);
   void (*DisposeString)(const char* string);
   libmahjongutils_KBoolean (*IsInstance)(libmahjongutils_KNativePtr ref, const libmahjongutils_KType* type);
   libmahjongutils_kref_kotlin_Byte (*createNullableByte)(libmahjongutils_KByte);
+  libmahjongutils_KByte (*getNonNullValueOfByte)(libmahjongutils_kref_kotlin_Byte);
   libmahjongutils_kref_kotlin_Short (*createNullableShort)(libmahjongutils_KShort);
+  libmahjongutils_KShort (*getNonNullValueOfShort)(libmahjongutils_kref_kotlin_Short);
   libmahjongutils_kref_kotlin_Int (*createNullableInt)(libmahjongutils_KInt);
+  libmahjongutils_KInt (*getNonNullValueOfInt)(libmahjongutils_kref_kotlin_Int);
   libmahjongutils_kref_kotlin_Long (*createNullableLong)(libmahjongutils_KLong);
+  libmahjongutils_KLong (*getNonNullValueOfLong)(libmahjongutils_kref_kotlin_Long);
   libmahjongutils_kref_kotlin_Float (*createNullableFloat)(libmahjongutils_KFloat);
+  libmahjongutils_KFloat (*getNonNullValueOfFloat)(libmahjongutils_kref_kotlin_Float);
   libmahjongutils_kref_kotlin_Double (*createNullableDouble)(libmahjongutils_KDouble);
+  libmahjongutils_KDouble (*getNonNullValueOfDouble)(libmahjongutils_kref_kotlin_Double);
   libmahjongutils_kref_kotlin_Char (*createNullableChar)(libmahjongutils_KChar);
+  libmahjongutils_KChar (*getNonNullValueOfChar)(libmahjongutils_kref_kotlin_Char);
   libmahjongutils_kref_kotlin_Boolean (*createNullableBoolean)(libmahjongutils_KBoolean);
+  libmahjongutils_KBoolean (*getNonNullValueOfBoolean)(libmahjongutils_kref_kotlin_Boolean);
   libmahjongutils_kref_kotlin_Unit (*createNullableUnit)(void);
+  libmahjongutils_kref_kotlin_UByte (*createNullableUByte)(libmahjongutils_KUByte);
+  libmahjongutils_KUByte (*getNonNullValueOfUByte)(libmahjongutils_kref_kotlin_UByte);
+  libmahjongutils_kref_kotlin_UShort (*createNullableUShort)(libmahjongutils_KUShort);
+  libmahjongutils_KUShort (*getNonNullValueOfUShort)(libmahjongutils_kref_kotlin_UShort);
+  libmahjongutils_kref_kotlin_UInt (*createNullableUInt)(libmahjongutils_KUInt);
+  libmahjongutils_KUInt (*getNonNullValueOfUInt)(libmahjongutils_kref_kotlin_UInt);
+  libmahjongutils_kref_kotlin_ULong (*createNullableULong)(libmahjongutils_KULong);
+  libmahjongutils_KULong (*getNonNullValueOfULong)(libmahjongutils_kref_kotlin_ULong);
 
 
   struct {
     struct {
       struct {
-        libmahjongutils_kref_mahjongutils_Entry (*get_ENTRY)();
         struct {
           libmahjongutils_KType* (*_type)(void);
           const char* (*call)(libmahjongutils_kref_mahjongutils_Entry thiz, const char* name, const char* rawParams);
         } Entry;
         struct {
+          struct {
+            libmahjongutils_KType* (*_type)(void);
+            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz);
+            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz);
+            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs (*deserialize)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
+            void (*serialize)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs value);
+          } $serializer;
+          struct {
+            libmahjongutils_KType* (*_type)(void);
+            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_Companion (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_Companion thiz);
+          } Companion;
           libmahjongutils_KType* (*_type)(void);
           libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs (*FuroChanceShantenArgs)(libmahjongutils_KInt seen1, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_mahjongutils_models_Tile chanceTile, libmahjongutils_KBoolean allowChi, libmahjongutils_KBoolean bestShantenOnly, libmahjongutils_KBoolean allowKuikae, libmahjongutils_kref_kotlinx_serialization_internal_SerializationConstructorMarker serializationConstructorMarker);
           libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs (*FuroChanceShantenArgs_)(libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_mahjongutils_models_Tile chanceTile, libmahjongutils_KBoolean allowChi, libmahjongutils_KBoolean bestShantenOnly, libmahjongutils_KBoolean allowKuikae);
           libmahjongutils_KBoolean (*get_allowChi)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_KBoolean (*get_allowKuikae)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_KBoolean (*get_bestShantenOnly)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_kref_mahjongutils_models_Tile (*get_chanceTile)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
@@ -162,55 +202,55 @@
           libmahjongutils_KBoolean (*component3)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_KBoolean (*component4)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_KBoolean (*component5)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs (*copy)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_mahjongutils_models_Tile chanceTile, libmahjongutils_KBoolean allowChi, libmahjongutils_KBoolean bestShantenOnly, libmahjongutils_KBoolean allowKuikae);
           libmahjongutils_KBoolean (*equals)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz, libmahjongutils_kref_kotlin_Any other);
           libmahjongutils_KInt (*hashCode)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
           const char* (*toString)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs thiz);
+        } FuroChanceShantenArgs;
+        struct {
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz);
-            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz);
-            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs (*deserialize)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
-            void (*serialize)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs value);
+            libmahjongutils_kref_mahjongutils_HanHu_$serializer (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz);
+            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz);
+            libmahjongutils_kref_mahjongutils_HanHu (*deserialize)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
+            void (*serialize)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_HanHu value);
           } $serializer;
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_Companion (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_FuroChanceShantenArgs_Companion thiz);
+            libmahjongutils_kref_mahjongutils_HanHu_Companion (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_HanHu_Companion thiz);
           } Companion;
-        } FuroChanceShantenArgs;
-        struct {
           libmahjongutils_KType* (*_type)(void);
           libmahjongutils_kref_mahjongutils_HanHu (*HanHu)(libmahjongutils_KInt seen1, libmahjongutils_KInt han, libmahjongutils_KInt hu, libmahjongutils_kref_kotlinx_serialization_internal_SerializationConstructorMarker serializationConstructorMarker);
           libmahjongutils_kref_mahjongutils_HanHu (*HanHu_)(libmahjongutils_KInt han, libmahjongutils_KInt hu);
           libmahjongutils_KInt (*get_han)(libmahjongutils_kref_mahjongutils_HanHu thiz);
           libmahjongutils_KInt (*get_hu)(libmahjongutils_kref_mahjongutils_HanHu thiz);
           libmahjongutils_KInt (*component1)(libmahjongutils_kref_mahjongutils_HanHu thiz);
           libmahjongutils_KInt (*component2)(libmahjongutils_kref_mahjongutils_HanHu thiz);
           libmahjongutils_kref_mahjongutils_HanHu (*copy)(libmahjongutils_kref_mahjongutils_HanHu thiz, libmahjongutils_KInt han, libmahjongutils_KInt hu);
           libmahjongutils_KBoolean (*equals)(libmahjongutils_kref_mahjongutils_HanHu thiz, libmahjongutils_kref_kotlin_Any other);
           libmahjongutils_KInt (*hashCode)(libmahjongutils_kref_mahjongutils_HanHu thiz);
           const char* (*toString)(libmahjongutils_kref_mahjongutils_HanHu thiz);
+        } HanHu;
+        struct {
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_HanHu_$serializer (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz);
-            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz);
-            libmahjongutils_kref_mahjongutils_HanHu (*deserialize)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
-            void (*serialize)(libmahjongutils_kref_mahjongutils_HanHu_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_HanHu value);
+            libmahjongutils_kref_mahjongutils_HoraArgs_$serializer (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz);
+            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz);
+            libmahjongutils_kref_mahjongutils_HoraArgs (*deserialize)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
+            void (*serialize)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_HoraArgs value);
           } $serializer;
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_HanHu_Companion (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_HanHu_Companion thiz);
+            libmahjongutils_kref_mahjongutils_HoraArgs_Companion (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_HoraArgs_Companion thiz);
           } Companion;
-        } HanHu;
-        struct {
           libmahjongutils_KType* (*_type)(void);
           libmahjongutils_kref_mahjongutils_HoraArgs (*HoraArgs)(libmahjongutils_KInt seen1, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_kref_mahjongutils_shanten_CommonShantenResult shantenResult, libmahjongutils_kref_mahjongutils_models_Tile agari, libmahjongutils_KBoolean tsumo, libmahjongutils_KInt dora, libmahjongutils_kref_mahjongutils_models_Wind selfWind, libmahjongutils_kref_mahjongutils_models_Wind roundWind, libmahjongutils_kref_kotlin_collections_Set extraYaku, libmahjongutils_kref_kotlinx_serialization_internal_SerializationConstructorMarker serializationConstructorMarker);
           libmahjongutils_kref_mahjongutils_HoraArgs (*HoraArgs_)(libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_kref_mahjongutils_shanten_CommonShantenResult shantenResult, libmahjongutils_kref_mahjongutils_models_Tile agari, libmahjongutils_KBoolean tsumo, libmahjongutils_KInt dora, libmahjongutils_kref_mahjongutils_models_Wind selfWind, libmahjongutils_kref_mahjongutils_models_Wind roundWind, libmahjongutils_kref_kotlin_collections_Set extraYaku);
           libmahjongutils_kref_mahjongutils_models_Tile (*get_agari)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_KInt (*get_dora)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_kref_kotlin_collections_Set (*get_extraYaku)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_kref_kotlin_collections_List (*get_furo)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
@@ -228,54 +268,42 @@
           libmahjongutils_kref_mahjongutils_models_Wind (*component7)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_kref_mahjongutils_models_Wind (*component8)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_kref_kotlin_collections_Set (*component9)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           libmahjongutils_kref_mahjongutils_HoraArgs (*copy)(libmahjongutils_kref_mahjongutils_HoraArgs thiz, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_kref_mahjongutils_shanten_CommonShantenResult shantenResult, libmahjongutils_kref_mahjongutils_models_Tile agari, libmahjongutils_KBoolean tsumo, libmahjongutils_KInt dora, libmahjongutils_kref_mahjongutils_models_Wind selfWind, libmahjongutils_kref_mahjongutils_models_Wind roundWind, libmahjongutils_kref_kotlin_collections_Set extraYaku);
           libmahjongutils_KBoolean (*equals)(libmahjongutils_kref_mahjongutils_HoraArgs thiz, libmahjongutils_kref_kotlin_Any other);
           libmahjongutils_KInt (*hashCode)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
           const char* (*toString)(libmahjongutils_kref_mahjongutils_HoraArgs thiz);
+        } HoraArgs;
+        struct {
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_HoraArgs_$serializer (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz);
-            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz);
-            libmahjongutils_kref_mahjongutils_HoraArgs (*deserialize)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
-            void (*serialize)(libmahjongutils_kref_mahjongutils_HoraArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_HoraArgs value);
+            libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz);
+            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz);
+            libmahjongutils_kref_mahjongutils_ShantenArgs (*deserialize)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
+            void (*serialize)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_ShantenArgs value);
           } $serializer;
           struct {
             libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_HoraArgs_Companion (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_HoraArgs_Companion thiz);
+            libmahjongutils_kref_mahjongutils_ShantenArgs_Companion (*_instance)();
+            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_ShantenArgs_Companion thiz);
           } Companion;
-        } HoraArgs;
-        struct {
           libmahjongutils_KType* (*_type)(void);
           libmahjongutils_kref_mahjongutils_ShantenArgs (*ShantenArgs)(libmahjongutils_KInt seen1, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_KBoolean bestShantenOnly, libmahjongutils_kref_kotlinx_serialization_internal_SerializationConstructorMarker serializationConstructorMarker);
           libmahjongutils_kref_mahjongutils_ShantenArgs (*ShantenArgs_)(libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_KBoolean bestShantenOnly);
           libmahjongutils_KBoolean (*get_bestShantenOnly)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_kref_kotlin_collections_List (*get_furo)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_kref_kotlin_collections_List (*get_tiles)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_kref_kotlin_collections_List (*component1)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_kref_kotlin_collections_List (*component2)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_KBoolean (*component3)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           libmahjongutils_kref_mahjongutils_ShantenArgs (*copy)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz, libmahjongutils_kref_kotlin_collections_List tiles, libmahjongutils_kref_kotlin_collections_List furo, libmahjongutils_KBoolean bestShantenOnly);
           libmahjongutils_KBoolean (*equals)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz, libmahjongutils_kref_kotlin_Any other);
           libmahjongutils_KInt (*hashCode)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
           const char* (*toString)(libmahjongutils_kref_mahjongutils_ShantenArgs thiz);
-          struct {
-            libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_descriptors_SerialDescriptor (*get_descriptor)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz);
-            libmahjongutils_kref_kotlin_Array (*childSerializers)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz);
-            libmahjongutils_kref_mahjongutils_ShantenArgs (*deserialize)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Decoder decoder);
-            void (*serialize)(libmahjongutils_kref_mahjongutils_ShantenArgs_$serializer thiz, libmahjongutils_kref_kotlinx_serialization_encoding_Encoder encoder, libmahjongutils_kref_mahjongutils_ShantenArgs value);
-          } $serializer;
-          struct {
-            libmahjongutils_KType* (*_type)(void);
-            libmahjongutils_kref_mahjongutils_ShantenArgs_Companion (*_instance)();
-            libmahjongutils_kref_kotlinx_serialization_KSerializer (*serializer)(libmahjongutils_kref_mahjongutils_ShantenArgs_Companion thiz);
-          } Companion;
         } ShantenArgs;
+        libmahjongutils_kref_mahjongutils_Entry (*get_ENTRY)();
       } mahjongutils;
     } root;
   } kotlin;
 } libmahjongutils_ExportedSymbols;
 extern libmahjongutils_ExportedSymbols* libmahjongutils_symbols(void);
```

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/furo.py` & `mahjong-utils-0.5.0/mahjong_utils/models/furo.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/hand.py` & `mahjong-utils-0.5.0/mahjong_utils/models/hand.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/hand_pattern.py` & `mahjong-utils-0.5.0/mahjong_utils/models/hand_pattern.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/mentsu.py` & `mahjong-utils-0.5.0/mahjong_utils/models/mentsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/tatsu.py` & `mahjong-utils-0.5.0/mahjong_utils/models/tatsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/tile.py` & `mahjong-utils-0.5.0/mahjong_utils/models/tile.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/models/tile_type.py` & `mahjong-utils-0.5.0/mahjong_utils/models/tile_type.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/models.py` & `mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/point_by_han_hu/point_by_han_hu.py` & `mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/point_by_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/shanten/models.py` & `mahjong-utils-0.5.0/mahjong_utils/shanten/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Set, Dict, Generic, TypeVar
+from typing import Optional, Set, Dict, Generic, TypeVar, List
 
 from pydantic import BaseModel
 from typing_extensions import Self
 
 from mahjong_utils.models.hand import Hand, T_HandPattern
 from mahjong_utils.models.hand_pattern import RegularHandPattern, ChitoiHandPattern, KokushiHandPattern, HandPattern
 from mahjong_utils.models.tatsu import Tatsu
@@ -32,41 +32,83 @@
             return ShantenWithoutGot.__decode__(data)
         elif data['type'] == 'ShantenWithGot':
             return ShantenWithGot.__decode__(data)
         else:
             raise ValueError("invalid type: " + data['type'])
 
 
+class Improvement(BaseModel):
+    discard: Tile
+    advance: Set[Tile]
+    advance_num: int
+
+    def __encode__(self) -> dict:
+        return dict(
+            discard=self.discard.__encode__(),
+            advance=[t.__encode__() for t in self.advance],
+            advanceNum=self.advance_num
+        )
+
+    @classmethod
+    def __decode__(cls, data: dict) -> "Improvement":
+        return Improvement(
+            discard=Tile.__decode__(data["discard"]),
+            advance=set(Tile.__decode__(x) for x in data["advance"]),
+            advance_num=data["advanceNum"]
+        )
+
+
 class ShantenWithoutGot(CommonShanten):
     advance: Set[Tile]
     advance_num: int
     good_shape_advance: Optional[Set[Tile]]
     good_shape_advance_num: Optional[int]
+    improvement: Optional[Dict[Tile, List[Improvement]]]
+    improvement_num: Optional[int]
 
     def __encode__(self) -> dict:
+        improvement = None
+
+        if self.improvement is not None:
+            improvement = dict()
+            for t in self.improvement:
+                improvement[t.__encode__()] = [x.__encode__() for x in self.improvement[t]]
+
         return dict(
             type="ShantenWithoutGot",
             shantenNum=self.shanten,
             advance=[t.__encode__() for t in self.advance],
             advanceNum=self.advance_num,
             goodShapeAdvance=[t.__encode__() for t in self.good_shape_advance]
             if self.good_shape_advance is not None else None,
-            goodShapeAdvanceNum=self.good_shape_advance_num
+            goodShapeAdvanceNum=self.good_shape_advance_num,
+            improvement=improvement,
+            improvementNum=self.improvement_num,
         )
 
     @classmethod
     def __decode__(cls, data: dict) -> "ShantenWithoutGot":
+        improvement = None
+
+        if data["improvement"] is not None:
+            improvement = dict()
+            for t in data["improvement"]:
+                improvement[Tile.__decode__(t)] = [Improvement.__decode__(x) for x in data["improvement"][t]]
+
         return ShantenWithoutGot(
             shanten=data["shantenNum"],
             advance=set(Tile.__decode__(x) for x in data["advance"]),
             advance_num=data["advanceNum"],
             good_shape_advance=set(Tile.__decode__(x) for x in data["goodShapeAdvance"])
             if data["goodShapeAdvance"] is not None else None,
             good_shape_advance_num=data["goodShapeAdvanceNum"]
             if data["goodShapeAdvanceNum"] is not None else None,
+            improvement=improvement,
+            improvement_num=data["improvementNum"]
+            if data["improvementNum"] is not None else None,
         )
 
 
 class ShantenWithGot(CommonShanten):
     discard_to_advance: Dict[Tile, ShantenWithoutGot]
     ankan_to_advance: Dict[Tile, ShantenWithoutGot]
 
@@ -161,14 +203,22 @@
         return getattr(self.shanten_info, "good_shape_advance", None)
 
     @property
     def good_shape_advance_num(self) -> Optional[int]:
         return getattr(self.shanten_info, "good_shape_advance_num", None)
 
     @property
+    def improvement(self) -> Optional[Dict[Tile, Set[Improvement]]]:
+        return getattr(self.shanten_info, "improvement", None)
+
+    @property
+    def improvement_num(self) -> Optional[int]:
+        return getattr(self.shanten_info, "improvement_num", None)
+
+    @property
     def discard_to_advance(self) -> Optional[Dict[Tile, ShantenWithoutGot]]:
         return getattr(self.shanten_info, "discard_to_advance", None)
 
     @property
     def ankan_to_advance(self) -> Optional[Dict[Tile, ShantenWithoutGot]]:
         return getattr(self.shanten_info, "ankan_to_advance", None)
```

### Comparing `mahjong-utils-0.4.3/mahjong_utils/shanten/shanten.py` & `mahjong-utils-0.5.0/mahjong_utils/shanten/shanten.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/yaku/all_yaku.py` & `mahjong-utils-0.5.0/mahjong_utils/yaku/all_yaku.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/yaku/common.py` & `mahjong-utils-0.5.0/mahjong_utils/yaku/common.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/yaku/extra.py` & `mahjong-utils-0.5.0/mahjong_utils/yaku/extra.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils/yaku/yakuman.py` & `mahjong-utils-0.5.0/mahjong_utils/yaku/yakuman.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/mahjong_utils.egg-info/PKG-INFO` & `mahjong-utils-0.5.0/mahjong_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.4.3
+Version: 0.5.0
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.4.3/mahjong_utils.egg-info/SOURCES.txt` & `mahjong-utils-0.5.0/mahjong_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/setup.py` & `mahjong-utils-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mahjong-utils",
-    version="0.4.3",
+    version="0.5.0",
     author="ssttkkl",
     author_email="huang.wen.long@hotmail.com",
     license="MIT",
     url="https://github.com/ssttkkl/mahjong-utils",
     description="日麻小工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mahjong-utils-0.4.3/tests/test_han_hu.py` & `mahjong-utils-0.5.0/tests/test_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/tests/test_hora.py` & `mahjong-utils-0.5.0/tests/test_hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.4.3/tests/test_shanten.py` & `mahjong-utils-0.5.0/tests/test_shanten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from mahjong_utils.models.tile import parse_tiles, all_yaochu, Tile
 from mahjong_utils.shanten import shanten, kokushi_shanten, regular_shanten, furo_chance_shanten
 
 
 def shanten_tester(tiles, expected_shanten,
                    expected_advance,
                    expected_advance_num,
-                   expected_good_shape_advance_num=None, *,
+                   expected_good_shape_advance_num=None,
+                   expected_improvement_num=None,
+                   *,
                    test_func=shanten):
     tiles = parse_tiles(tiles)
     result = test_func(tiles)
 
     assert result.shanten == expected_shanten
     assert result.advance == expected_advance
     assert result.advance_num == expected_advance_num
     assert result.good_shape_advance_num == expected_good_shape_advance_num
+    assert result.improvement_num == expected_improvement_num
     assert result.discard_to_advance is None
 
 
 # noinspection PyTypeChecker
 def test_regular_shanten():
     shanten_tester("34568m235p68s", 2, {*parse_tiles("3678m12345p678s"), }, 40, test_func=regular_shanten)
     shanten_tester("112233p44556s12z", 1, {*parse_tiles("36s12z"), }, 13, 6, test_func=regular_shanten)
-    shanten_tester("1112345678999p", 0, {*parse_tiles("123456789p"), }, 23, test_func=regular_shanten)
+    shanten_tester("1112345678999p", 0, {*parse_tiles("123456789p"), }, 23, None, 0, test_func=regular_shanten)
     shanten_tester("114514p1919810s", 2, {*parse_tiles("234567p3456789s"), }, 45, test_func=regular_shanten)
 
 
 # noinspection PyTypeChecker
 def test_shanten():
     shanten_tester("34568m235p68s", 2, {*parse_tiles("3678m12345p678s"), }, 40)
     shanten_tester("3344z6699p11345s", 1, {*parse_tiles("345s"), }, 9, 0)
     shanten_tester("112233p44556s12z", 1, {*parse_tiles("36s12z"), }, 13, 6)
-    shanten_tester("1112345678999p", 0, {*parse_tiles("123456789p"), }, 23)
+    shanten_tester("1112345678999p", 0, {*parse_tiles("123456789p"), }, 23, None, 0)
     shanten_tester("114514p1919810s", 2, {*parse_tiles("234567p3456789s"), }, 45)
     shanten_tester("119m19p19266s135z", 3, {*parse_tiles("2467z"), }, 16)
     shanten_tester("19m19p19266s1235z", 3, all_yaochu, 42)
     shanten_tester("1119m19p19s12355z", 2, {*parse_tiles("467z"), }, 12)
-    shanten_tester("119m19p19s123456z", 0, {*parse_tiles("7z"), }, 4)
+    shanten_tester("119m19p19s123456z", 0, {*parse_tiles("7z"), }, 4, None, 0)
 
 
 def shanten_with_got_tester(tiles, expected_shanten, expected_discard_to_advance, test_func=shanten):
     tiles = parse_tiles(tiles)
     result = test_func(tiles)
 
     actual_discard_to_advance = dict()
```

