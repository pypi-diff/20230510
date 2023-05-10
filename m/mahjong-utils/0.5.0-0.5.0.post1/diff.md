# Comparing `tmp/mahjong-utils-0.5.0.tar.gz` & `tmp/mahjong-utils-0.5.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahjong-utils-0.5.0.tar", last modified: Wed May 10 10:03:46 2023, max compression
+gzip compressed data, was "mahjong-utils-0.5.0.post1.tar", last modified: Wed May 10 11:15:57 2023, max compression
```

## Comparing `mahjong-utils-0.5.0.tar` & `mahjong-utils-0.5.0.post1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.259481 mahjong-utils-0.5.0/
--rw-rw-rw-   0        0        0       61 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9237 2023-05-10 10:03:46.258950 mahjong-utils-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8982 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/
--rw-rw-rw-   0        0        0       27 2023-05-10 10:00:50.000000 mahjong-utils-0.5.0/kt/.git
--rw-rw-rw-   0        0        0     2272 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/LICENSE
--rw-rw-rw-   0        0        0     7412 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/build-scripts/
--rw-rw-rw-   0        0        0      219 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build-scripts/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179386 mahjong-utils-0.5.0/kt/build-scripts/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179386 mahjong-utils-0.5.0/kt/build-scripts/src/main/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/
--rw-rw-rw-   0        0        0     3528 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
--rw-rw-rw-   0        0        0     1341 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.179895 mahjong-utils-0.5.0/kt/gradle/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/gradle/wrapper/
--rw-rw-rw-   0        0        0    59821 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.jar
--rw-rw-rw-   0        0        0      207 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.properties
--rw-rw-rw-   0        0        0      160 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradle.properties
--rw-rw-rw-   0        0        0     8304 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradlew
--rwxrwxrwx   0        0        0     2763 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/gradlew.bat
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.200107 mahjong-utils-0.5.0/kt/kotlin-js-store/
--rw-rw-rw-   0        0        0   104679 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/kotlin-js-store/yarn.lock
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/
--rw-rw-rw-   0        0        0     2247 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0      765 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
--rw-rw-rw-   0        0        0     3589 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
--rw-rw-rw-   0        0        0     2402 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
--rw-rw-rw-   0        0        0     1098 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1468 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     6239 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1243 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     5972 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
--rw-rw-rw-   0        0        0      102 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/settings.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/
--rw-rw-rw-   0        0        0     5458 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
--rw-rw-rw-   0        0        0     7595 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     3866 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.204680 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     6458 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
--rw-rw-rw-   0        0        0     8108 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
--rw-rw-rw-   0        0        0      442 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.217532 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/
--rw-rw-rw-   0        0        0     3780 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
--rw-rw-rw-   0        0        0     4359 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
--rw-rw-rw-   0        0        0     6033 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
--rw-rw-rw-   0        0        0     8193 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
--rw-rw-rw-   0        0        0      308 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.219514 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/
--rw-rw-rw-   0        0        0      412 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
--rw-rw-rw-   0        0        0     3482 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
--rw-rw-rw-   0        0        0      303 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     3755 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
--rw-rw-rw-   0        0        0     6200 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
--rw-rw-rw-   0        0        0     4268 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
--rw-rw-rw-   0        0        0     4904 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
--rw-rw-rw-   0        0        0    10782 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
--rw-rw-rw-   0        0        0     6362 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
--rw-rw-rw-   0        0        0     3285 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     7774 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
--rw-rw-rw-   0        0        0     1683 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
--rw-rw-rw-   0        0        0    10647 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/jvmTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.180456 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.188968 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     2194 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     5806 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     2656 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
--rw-rw-rw-   0        0        0    44661 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     9674 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
--rw-rw-rw-   0        0        0     6902 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
--rw-rw-rw-   0        0        0      573 2023-05-10 10:00:51.000000 mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.220571 mahjong-utils-0.5.0/mahjong_utils/
--rw-rw-rw-   0        0        0      116 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.238312 mahjong-utils-0.5.0/mahjong_utils/hora/
--rw-rw-rw-   0        0        0       44 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/__init__.py
--rw-rw-rw-   0        0        0     2714 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/hora.py
--rw-rw-rw-   0        0        0     6263 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/hora/models.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.239616 mahjong-utils-0.5.0/mahjong_utils/lib/
--rw-rw-rw-   0        0        0     2209 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/lib/__init__.py
--rw-rw-rw-   0        0        0    22878 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/lib/libmahjongutils_api.i
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.246898 mahjong-utils-0.5.0/mahjong_utils/models/
--rw-rw-rw-   0        0        0      176 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/furo.py
--rw-rw-rw-   0        0        0     1360 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/hand.py
--rw-rw-rw-   0        0        0     6769 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/hand_pattern.py
--rw-rw-rw-   0        0        0     3136 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/mentsu.py
--rw-rw-rw-   0        0        0     4718 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tatsu.py
--rw-rw-rw-   0        0        0     6600 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tile.py
--rw-rw-rw-   0        0        0      618 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/tile_type.py
--rw-rw-rw-   0        0        0      367 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/models/wind.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.248629 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/
--rw-rw-rw-   0        0        0       55 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/__init__.py
--rw-rw-rw-   0        0        0      605 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/models.py
--rw-rw-rw-   0        0        0      924 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/point_by_han_hu.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.249674 mahjong-utils-0.5.0/mahjong_utils/shanten/
--rw-rw-rw-   0        0        0       47 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/__init__.py
--rw-rw-rw-   0        0        0    12095 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/models.py
--rw-rw-rw-   0        0        0     4024 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/shanten/shanten.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.251687 mahjong-utils-0.5.0/mahjong_utils/yaku/
--rw-rw-rw-   0        0        0      172 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/all_yaku.py
--rw-rw-rw-   0        0        0     1353 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/common.py
--rw-rw-rw-   0        0        0      649 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/extra.py
--rw-rw-rw-   0        0        0      168 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/yaku.py
--rw-rw-rw-   0        0        0     1156 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/mahjong_utils/yaku/yakuman.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.236336 mahjong-utils-0.5.0/mahjong_utils.egg-info/
--rw-rw-rw-   0        0        0     9237 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3932 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 10:03:45.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 10:03:46.000000 mahjong-utils-0.5.0/mahjong_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 10:03:46.259989 mahjong-utils-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     5019 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:03:46.258316 mahjong-utils-0.5.0/tests/
--rw-rw-rw-   0        0        0     1221 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_han_hu.py
--rw-rw-rw-   0        0        0     5422 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_hora.py
--rw-rw-rw-   0        0        0      297 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_lib.py
--rw-rw-rw-   0        0        0     8938 2023-05-10 10:00:48.000000 mahjong-utils-0.5.0/tests/test_shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/
+-rw-rw-rw-   0        0        0       61 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9243 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     8982 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/
+-rw-rw-rw-   0        0        0       27 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/.git
+-rw-rw-rw-   0        0        0     2272 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/LICENSE
+-rw-rw-rw-   0        0        0     7412 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/build-scripts/
+-rw-rw-rw-   0        0        0      219 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build-scripts/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/build-scripts/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/
+-rw-rw-rw-   0        0        0     3528 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
+-rw-rw-rw-   0        0        0     1341 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/gradle/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/
+-rw-rw-rw-   0        0        0    59821 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.jar
+-rw-rw-rw-   0        0        0      207 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.properties
+-rw-rw-rw-   0        0        0      160 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle.properties
+-rw-rw-rw-   0        0        0     8304 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradlew
+-rwxrwxrwx   0        0        0     2763 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradlew.bat
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/kotlin-js-store/
+-rw-rw-rw-   0        0        0   104679 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/kotlin-js-store/yarn.lock
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/
+-rw-rw-rw-   0        0        0     2247 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0      765 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
+-rw-rw-rw-   0        0        0     3589 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
+-rw-rw-rw-   0        0        0     2402 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
+-rw-rw-rw-   0        0        0     1098 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1468 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     6239 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1243 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     5972 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
+-rw-rw-rw-   0        0        0      102 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/settings.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/
+-rw-rw-rw-   0        0        0     5458 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
+-rw-rw-rw-   0        0        0     7595 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     3866 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     6458 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
+-rw-rw-rw-   0        0        0     8108 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
+-rw-rw-rw-   0        0        0      442 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/
+-rw-rw-rw-   0        0        0     3780 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
+-rw-rw-rw-   0        0        0     4359 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
+-rw-rw-rw-   0        0        0     6033 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
+-rw-rw-rw-   0        0        0     8193 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
+-rw-rw-rw-   0        0        0      308 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/
+-rw-rw-rw-   0        0        0      412 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
+-rw-rw-rw-   0        0        0     3482 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
+-rw-rw-rw-   0        0        0      303 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     3755 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
+-rw-rw-rw-   0        0        0     6200 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
+-rw-rw-rw-   0        0        0     4268 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
+-rw-rw-rw-   0        0        0     4904 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
+-rw-rw-rw-   0        0        0    10782 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
+-rw-rw-rw-   0        0        0     6362 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
+-rw-rw-rw-   0        0        0     3285 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     7774 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
+-rw-rw-rw-   0        0        0     1683 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
+-rw-rw-rw-   0        0        0    10647 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     2194 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     5806 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     2656 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
+-rw-rw-rw-   0        0        0    44661 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     9674 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
+-rw-rw-rw-   0        0        0     6902 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
+-rw-rw-rw-   0        0        0      573 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/
+-rw-rw-rw-   0        0        0      116 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/hora/
+-rw-rw-rw-   0        0        0       44 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/__init__.py
+-rw-rw-rw-   0        0        0     2714 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/hora.py
+-rw-rw-rw-   0        0        0     6263 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/models.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/lib/
+-rw-rw-rw-   0        0        0     2209 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/lib/__init__.py
+-rw-rw-rw-   0        0        0    22878 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/lib/libmahjongutils_api.i
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/models/
+-rw-rw-rw-   0        0        0      176 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/furo.py
+-rw-rw-rw-   0        0        0     1360 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/hand.py
+-rw-rw-rw-   0        0        0     6769 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/hand_pattern.py
+-rw-rw-rw-   0        0        0     3136 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/mentsu.py
+-rw-rw-rw-   0        0        0     4718 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tatsu.py
+-rw-rw-rw-   0        0        0     6600 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tile.py
+-rw-rw-rw-   0        0        0      618 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tile_type.py
+-rw-rw-rw-   0        0        0      367 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/wind.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/
+-rw-rw-rw-   0        0        0       55 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/models.py
+-rw-rw-rw-   0        0        0      924 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/point_by_han_hu.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/
+-rw-rw-rw-   0        0        0       47 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/__init__.py
+-rw-rw-rw-   0        0        0    12099 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/models.py
+-rw-rw-rw-   0        0        0     4024 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/
+-rw-rw-rw-   0        0        0      172 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/all_yaku.py
+-rw-rw-rw-   0        0        0     1353 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/common.py
+-rw-rw-rw-   0        0        0      649 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/extra.py
+-rw-rw-rw-   0        0        0      168 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yaku.py
+-rw-rw-rw-   0        0        0     1156 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yakuman.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/
+-rw-rw-rw-   0        0        0     9243 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3932 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0     5025 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/tests/
+-rw-rw-rw-   0        0        0     1221 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_han_hu.py
+-rw-rw-rw-   0        0        0     5422 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_hora.py
+-rw-rw-rw-   0        0        0      297 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_lib.py
+-rw-rw-rw-   0        0        0     8938 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_shanten.py
```

### Comparing `mahjong-utils-0.5.0/PKG-INFO` & `mahjong-utils-0.5.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.5.0
+Version: 0.5.0.post1
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.5.0/README.md` & `mahjong-utils-0.5.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/.gitignore` & `mahjong-utils-0.5.0.post1/kt/.gitignore`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/LICENSE` & `mahjong-utils-0.5.0.post1/kt/LICENSE`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/README.md` & `mahjong-utils-0.5.0.post1/kt/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts` & `mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/build.gradle.kts` & `mahjong-utils-0.5.0.post1/kt/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/gradle/wrapper/gradle-wrapper.jar` & `mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/gradlew` & `mahjong-utils-0.5.0.post1/kt/gradlew`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/gradlew.bat` & `mahjong-utils-0.5.0.post1/kt/gradlew.bat`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/kotlin-js-store/yarn.lock` & `mahjong-utils-0.5.0.post1/kt/kotlin-js-store/yarn.lock`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/build.gradle.kts` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt` & `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt` & `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/hora/hora.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/hora/hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/hora/models.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/hora/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/lib/__init__.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/lib/libmahjongutils_api.i` & `mahjong-utils-0.5.0.post1/mahjong_utils/lib/libmahjongutils_api.i`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/furo.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/furo.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/hand.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/hand.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/hand_pattern.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/hand_pattern.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/mentsu.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/mentsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/tatsu.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/tatsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/tile.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/tile.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/models/tile_type.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/models/tile_type.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/models.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/point_by_han_hu/point_by_han_hu.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/point_by_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/shanten/models.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/shanten/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         )
 
 
 class ShantenWithFuroChance(Shanten):
     pass_: Optional[ShantenWithoutGot]
     chi: Dict[Tatsu, ShantenWithGot]
     pon: Optional[ShantenWithGot]
-    minkan: Optional[ShantenWithGot]
+    minkan: Optional[ShantenWithoutGot]
 
     def __encode__(self) -> dict:
         return {
             'type': "ShantenWithFuroChance",
             'shantenNum': self.shanten,
             'pass': self.pass_.__encode__()
             if self.pass_ is not None else None,
@@ -203,15 +203,15 @@
         return getattr(self.shanten_info, "good_shape_advance", None)
 
     @property
     def good_shape_advance_num(self) -> Optional[int]:
         return getattr(self.shanten_info, "good_shape_advance_num", None)
 
     @property
-    def improvement(self) -> Optional[Dict[Tile, Set[Improvement]]]:
+    def improvement(self) -> Optional[Dict[Tile, List[Improvement]]]:
         return getattr(self.shanten_info, "improvement", None)
 
     @property
     def improvement_num(self) -> Optional[int]:
         return getattr(self.shanten_info, "improvement_num", None)
 
     @property
```

### Comparing `mahjong-utils-0.5.0/mahjong_utils/shanten/shanten.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/shanten/shanten.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/yaku/all_yaku.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/all_yaku.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/yaku/common.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/common.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/yaku/extra.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/extra.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils/yaku/yakuman.py` & `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yakuman.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/mahjong_utils.egg-info/PKG-INFO` & `mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.5.0
+Version: 0.5.0.post1
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.5.0/mahjong_utils.egg-info/SOURCES.txt` & `mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/setup.py` & `mahjong-utils-0.5.0.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mahjong-utils",
-    version="0.5.0",
+    version="0.5.0.post1",
     author="ssttkkl",
     author_email="huang.wen.long@hotmail.com",
     license="MIT",
     url="https://github.com/ssttkkl/mahjong-utils",
     description="日麻小工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mahjong-utils-0.5.0/tests/test_han_hu.py` & `mahjong-utils-0.5.0.post1/tests/test_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/tests/test_hora.py` & `mahjong-utils-0.5.0.post1/tests/test_hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0/tests/test_shanten.py` & `mahjong-utils-0.5.0.post1/tests/test_shanten.py`

 * *Files identical despite different names*

