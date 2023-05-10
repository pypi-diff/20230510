# Comparing `tmp/glean-sdk-52.6.0.tar.gz` & `tmp/glean-sdk-52.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-sdk-52.6.0.tar", last modified: Thu Apr 20 18:39:29 2023, max compression
+gzip compressed data, was "glean-sdk-52.7.0.tar", last modified: Wed May 10 09:42:29 2023, max compression
```

## Comparing `glean-sdk-52.6.0.tar` & `glean-sdk-52.7.0.tar`

### file list

```diff
@@ -1,862 +1,862 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.buildconfig.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.491710 glean-sdk-52.6.0/.cargo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.cargo/config
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.491710 glean-sdk-52.6.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37462 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.circleci/jazzy.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.detekt.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2006 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.dictionary
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.flake8
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.flake8rc
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.491710 glean-sdk-52.6.0/.github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.github/CODEOWNERS
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.github/dependabot.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.491710 glean-sdk-52.6.0/.github/workflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.github/workflows/cargo-vet.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.swiftlint.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18277 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.taskcluster.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/.yamllint
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92301 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32171 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/Cargo.lock
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)   266141 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/DEPENDENCIES.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6581 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    96766 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      572 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/README.iOS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3773 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/about.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.495710 glean-sdk-52.6.0/bin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/about.md.hbs
--rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/about.xml.hbs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/build-rust-docs.bat
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5594 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/build-rust-docs.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      527 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/build-swift-docs.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2062 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/build-xcframework.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1764 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/check-artifact.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56317 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/codecov.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      976 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/dependency-summary.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4788 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/prepare-release.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      591 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/publish-glean-swift.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      510 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/run-ios-build.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      540 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/run-ios-sample-app-build.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      538 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/run-ios-sample-app-test.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      508 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/run-ios-tests.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      504 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/rust-wrapper-hack.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3777 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/spellcheck.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3005 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/update-glean-parser-version.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1377 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/bin/update-schema.sh
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.495710 glean-sdk-52.6.0/build-scripts/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3896 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build-scripts/publish_to_maven_local_if_modified.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build-scripts/shared.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build-scripts/substitute-local-glean.gradle
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      369 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build-scripts/xc-cargo.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1865 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build-scripts/xc-universal-binary.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7594 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/build.gradle
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1139 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/deny.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.471710 glean-sdk-52.6.0/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.495710 glean-sdk-52.6.0/docs/dev/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2072 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/SUMMARY.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/android/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2895 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/development-with-android-components.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      798 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/glean-parser-substitution.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1624 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/locally-published-components-in-fenix.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/sdk-ndk-versions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3702 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/android/setup-android-build-environment.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/api/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/book.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4991 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/ci.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/code_coverage.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/contributing.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/dependency-management.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1586 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/dependency-vetting.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5402 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/documentation-guidelines.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/index.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/core/internal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1343 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/clearing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/database.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/debug-pings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/directory-structure.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3016 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/implementations.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9164 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/payload.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/reserved-ping-names.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5389 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/internal/upload.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2054 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/logging-levels.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/core/new-metric-type/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type/kotlin.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3744 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type/platform.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type/python.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type/rust.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type/swift.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6707 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/core/new-metric-type.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11073 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/cut-a-new-release.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3841 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/docs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/glean.jpeg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/ios/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1577 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/ios/debug-glean-on-ios.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/ios/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1208 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/ios/setup-ios-build-environment.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.499710 glean-sdk-52.6.0/docs/dev/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/python/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7149 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/python/setting-up-python-build-environment.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/testing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/dev/upgrading-glean-parser.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.503710 glean-sdk-52.6.0/docs/shared/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/blockquote-info.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/blockquote-stop.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/blockquote-warning.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6518 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/glean.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/mermaid-init.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6335 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/mermaid.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1122951 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/mermaid.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/tab_footer.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/tab_header.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4063 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/shared/tabs.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.503710 glean-sdk-52.6.0/docs/user/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4831 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4723 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/SUMMARY.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.503710 glean-sdk-52.6.0/docs/user/_includes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/_includes/glean-js-redirect-collected-metrics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      287 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/_includes/label-errors.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/_includes/label-limits.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/_includes/labels-parameter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1276 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/_includes/lifetimes-parameters.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/appendix/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/appendix/changelog/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/appendix/changelog/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9084 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/appendix/contribution-guidelines.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3343 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/appendix/glossary.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/appendix/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8966 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/appendix/twig.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/book.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6721 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/chart-distributions-ui.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21881 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/chart-distributions.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   173077 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/chart.min.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/glean.jpeg
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48749 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/highlight.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/language-bindings/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/language-bindings/android/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3555 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/android/android-build-configuration-options.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2505 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/android/android-offline-builds.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/android/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8823 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/android/instrument-android-crashes-example.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4194 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/index.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/language-bindings/ios/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/ios/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/ios/ios-build-configuration-options.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/language-bindings/javascript/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/javascript/cli.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/javascript/index.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/language-bindings/javascript/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/javascript/plugins/encryption.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/language-bindings/javascript/plugins/index.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/docs/user/reference/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/reference/debug/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3356 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/debugViewTag.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1469 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3334 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/logPings.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.507710 glean-sdk-52.6.0/docs/user/reference/debug/screenshots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   281896 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/screenshots/debug_view_tag_screenshot_swift.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   298030 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/screenshots/log_pings_screenshot_swift.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   315960 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/screenshots/source_tags_screenshot_swift.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4172 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/debug/sourceTags.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.511710 glean-sdk-52.6.0/docs/user/reference/general/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/experiments-api.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1424 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19303 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/initializing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3298 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/register-custom-pings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2882 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/shutdown.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/general/toggling-upload-status.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.511710 glean-sdk-52.6.0/docs/user/reference/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5251 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/boolean.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7690 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/counter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11088 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/custom_distribution.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9945 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/datetime.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10097 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/event.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5331 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/labeled_booleans.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9183 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/labeled_counters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7292 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/labeled_strings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11734 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/memory_distribution.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6687 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/quantity.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10624 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/rate.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8214 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/string.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8863 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/string_list.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5863 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/text.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15425 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/timespan.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/timing_distribution.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8225 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/url.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8262 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/metrics/uuid.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.511710 glean-sdk-52.6.0/docs/user/reference/pings/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7240 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/pings/index.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/reference/yaml/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/yaml/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10678 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/yaml/metrics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4157 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/yaml/pings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/reference/yaml/tags.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/user/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5199 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/enable-data-ingestion.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6887 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/javascript.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5252 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/kotlin.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7175 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/python.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/qt.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/rust.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/swift.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/user/collected-metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12881 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/collected-metrics/metrics.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/user/debugging/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5922 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/debugging/android.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2903 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/debugging/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9495 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/debugging/ios.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/debugging/javascript.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/debugging/python.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4310 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/integrating-glean-for-product-managers.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    76710 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metric-lifetime-timeline.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.515710 glean-sdk-52.6.0/docs/user/user/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18606 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/adding-new-metrics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/error-reporting.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2439 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/metrics-remote-settings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5258 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/testing-metrics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3047 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/metrics/validation-checklist.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.519710 glean-sdk-52.6.0/docs/user/user/pings/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/baseline.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6458 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/custom.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2243 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/deletion-request.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3484 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/events.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12681 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/index.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7452 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/metrics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2879 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/ping-schedules-and-timings.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    87580 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/ping_timing.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4318 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/sent-by-glean.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/docs/user/user/pings/testing-custom-pings.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.519710 glean-sdk-52.6.0/glean-core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6866 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ARCHITECTURE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1906 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.519710 glean-sdk-52.6.0/glean-core/android/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/build.gradle
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15289 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/dependency-licenses.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1131 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/proguard-rules-consumer.pro
--rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/proguard-rules.pro
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/publish.gradle
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android/src/main/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/AndroidManifest.xml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/main/java/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Dispatchers.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23701 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Glean.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1756 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/Configuration.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6298 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/GleanDebugActivity.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/BaseUploader.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4741 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/HttpURLConnectionUploader.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/PingUploader.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/Upload.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/Aliases.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/BooleanMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CounterMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1995 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CustomDistributionMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DatetimeMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      861 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DenominatorMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3487 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/EventMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/HistogramBase.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4843 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/LabeledMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/MemoryDistributionMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/NumeratorMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3130 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/PingType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/QuantityMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/RateMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringListMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TextMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1132 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimespanMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2219 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimingDistributionMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UrlMetricType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1251 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UuidMetricType.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/GleanLifecycleObserver.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16434 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/MetricsPingScheduler.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5466 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/PingUploadWorker.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/ErrorType.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2089 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestLocalServer.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2908 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestRule.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      683 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DataPathUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5257 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DateUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/GzipUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1323 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/JsonUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2107 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/LocaleUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      828 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/ThreadUtils.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1646 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/WorkManagerUtils.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/test/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/test/java/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/test/java/android/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/test/java/android/util/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/android/util/Log.java
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3987 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanFromJavaTest.java
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36390 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11692 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/TestUtil.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12856 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/GleanDebugActivityTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.527710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1546 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/BaseUploaderTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7832 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/HttpURLConnectionUploaderTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.531710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7208 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/CustomPingTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6386 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/DeletionPingTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.531710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2195 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/AccumulationsBeforeGleanInitTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/BooleanMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5259 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CounterMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CustomDistributionMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4422 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/DatetimeMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18328 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/EventMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16861 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/LabeledMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7157 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/MemoryDistributionMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8749 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/PingTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5500 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/QuantityMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3373 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/RateMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7437 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringListMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4560 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12105 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimespanMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12735 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimingDistributionMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4942 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UrlMetricTypeTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4032 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UuidMetricTypeTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.531710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32702 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/MetricsPingSchedulerTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2494 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/PingUploadWorkerTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.531710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/ShadowLog.java
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1010 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DataPathUtilsTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DateUtilsTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/GzipUtilsTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2068 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/JsonUtilsTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/KArgumentCaptor.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/android/src/test/resources/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/android/src/test/resources/mockito-extensions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/resources/mockito-extensions/org.mockito.plugins.MockMaker
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android/src/test/resources/robolectric.properties
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android-native/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4376 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/build.gradle
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15289 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/dependency-licenses.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/proguard-rules-consumer.pro
--rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/proguard-rules.pro
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7614 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/publish.gradle
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.475710 glean-sdk-52.6.0/glean-core/android-native/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.523710 glean-sdk-52.6.0/glean-core/android-native/src/main/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/android-native/src/main/AndroidManifest.xml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/build/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      364 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/build/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/build/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/build/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/build/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3367 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/build/src/lib.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/build.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/bundle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/bundle/Cargo.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/bundle/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/bundle/src/lib.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/bundle-android/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/bundle-android/Cargo.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Config/Configuration.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean/Debug/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7256 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Debug/GleanDebugTools.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1219 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Dispatchers.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Glean.h
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20405 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Glean.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/GleanMetrics.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Info.plist
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/BooleanMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/CounterMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3603 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/DatetimeMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/EventMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4399 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/LabeledMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/MemoryDistributionMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/Ping.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/QuantityMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1898 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/RateMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      753 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/StringListMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/StringMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      681 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TextMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1962 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TimespanMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TimingDistributionMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2464 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/UrlMetric.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2025 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/UuidMetric.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/Glean/Net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8412 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Net/HttpPingUploader.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/Glean/Scheduler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1487 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Scheduler/GleanLifecycleObserver.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10362 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Scheduler/MetricsPingScheduler.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/Glean/Utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Logger.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7359 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Sysctl.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2409 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Unreachable.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6417 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Utils.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51892 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.pbxproj
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/xcshareddata/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.535710 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3541 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/Glean.xcscheme
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/GleanTests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Config/ConfigurationTests.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.539710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Debug/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3928 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Debug/GleanDebugUtilityTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13549 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/GleanTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Info.plist
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.543710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/BooleanMetricTypeTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/CounterMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6530 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/DatetimeMetricTypeTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11062 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/EventMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7967 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/LabeledMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4791 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/MemoryDistributionMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5941 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/PingTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3304 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/QuantityMetricTypeTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/RateMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5453 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/StringListMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/StringMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7367 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/TimespanMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6516 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/TimingDistributionMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4364 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/UrlMetricTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2879 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/UuidMetricTests.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.543710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7588 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/BaselinePingTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6306 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/DeletionRequestPingTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4074 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/HttpPingUploaderTests.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.543710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Scheduler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14876 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Scheduler/MetricsPingSchedulerTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4939 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/TestUtils.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.543710 glean-sdk-52.6.0/glean-core/ios/GleanTests/Utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/GleanTests/Utils/DataPathUtilsTests.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/base.xcconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/debug.xcconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/release.xcconfig
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5959 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/ios/sdk_generator.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/megazord.uniffi.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22145 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/pings.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.543710 glean-sdk-52.6.0/glean-core/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      376 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/glean/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_builtins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_ffi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10319 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5189 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_process_dispatcher.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/glean/_subprocess/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_subprocess/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14517 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/glean.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/glean/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3787 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/datetime.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3303 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3225 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/labeled.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/ping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/string.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4395 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/timespan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4475 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/timing_distribution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1628 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/metrics/uuid.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/glean/net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/net/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/net/base_uploader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3212 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/net/http_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4982 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/net/ping_upload_worker.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/net/ping_uploader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/glean/testing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2883 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/glean/testing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/requirements_dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9281 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.547710 glean-sdk-52.6.0/glean-core/python/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2889 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.551710 glean-sdk-52.6.0/glean-core/python/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8088 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/data/core.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/data/events_with_types.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/data/glinter.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/data/pings.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.551710 glean-sdk-52.6.0/glean-core/python/tests/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2163 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_boolean.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3757 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_counter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3059 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_datetime.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12498 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6873 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_labeled.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_memory_distribution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3639 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_quantity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_string.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3795 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_string_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_timespan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5858 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_timing_distribution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3418 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6456 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/metrics/test_uuid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26265 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/test_glean.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/test_loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6584 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/test_network.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      509 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/python/tests/test_subprocess.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.551710 glean-sdk-52.6.0/glean-core/rlb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.551710 glean-sdk-52.6.0/glean-core/rlb/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/examples/long-running.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1925 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/examples/prototype.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.551710 glean-sdk-52.6.0/glean-core/rlb/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/common_test.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5503 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/configuration.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1425 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/core_metrics.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9430 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/lib.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.555710 glean-sdk-52.6.0/glean-core/rlb/src/net/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      895 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/net/http_uploader.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7703 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/net/mod.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.555710 glean-sdk-52.6.0/glean-core/rlb/src/private/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7269 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/private/event.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1188 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/private/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2929 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/private/ping.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3836 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/system.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46441 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/src/test.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.555710 glean-sdk-52.6.0/glean-core/rlb/tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.555710 glean-sdk-52.6.0/glean-core/rlb/tests/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/common/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/init_fails.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2051 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/never_init.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2238 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/no_time_to_init.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3008 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/overflowing_preinit.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/persist_ping_lifetime.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/persist_ping_lifetime_nopanic.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6920 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/schema.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2454 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/simple.rs
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      729 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/test-shutdown-blocking.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7395 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/rlb/tests/upload_timing.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4701 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/common_metric_data.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34609 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/core/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7409 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/core_metrics.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1776 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/coverage.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65434 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/database/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10925 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/debug.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/dispatcher/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6930 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/dispatcher/global.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18377 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/dispatcher/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4755 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/error.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8362 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/error_recording.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/event_database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48620 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/event_database/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2603 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/fd_logger.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16554 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/glean.udl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/glean_metrics.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.559710 glean-sdk-52.6.0/glean-core/src/histogram/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6962 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/histogram/exponential.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/histogram/functional.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/histogram/linear.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3957 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/histogram/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8635 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/internal_metrics.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2105 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/internal_pings.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41219 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/lib.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36226 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/lib_unit_tests.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.563710 glean-sdk-52.6.0/glean-core/src/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3994 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/boolean.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/counter.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7537 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/custom_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10531 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/datetime.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4445 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/denominator.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6200 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/event.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9572 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/experiment.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10013 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/labeled.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9666 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/memory_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1837 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/memory_unit.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/metrics_enabled_config.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11590 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/numerator.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7190 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/ping.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3691 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/quantity.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5836 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/rate.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/recorded_experiment.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5307 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/string.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6385 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/string_list.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/text.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3795 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/time_unit.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10280 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/timespan.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18625 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/timing_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10166 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/url.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4936 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/metrics/uuid.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.563710 glean-sdk-52.6.0/glean-core/src/ping/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13588 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/ping/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23631 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/scheduler.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.563710 glean-sdk-52.6.0/glean-core/src/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9355 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/storage/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2856 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/system.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.567710 glean-sdk-52.6.0/glean-core/src/traits/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/boolean.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/counter.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1994 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/custom_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/datetime.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3815 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/event.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/labeled.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1804 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/memory_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/numerator.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/ping.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/quantity.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1823 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/rate.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1574 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/string.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/string_list.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/text.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/timespan.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2531 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/timing_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/url.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1528 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/traits/uuid.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.567710 glean-sdk-52.6.0/glean-core/src/upload/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14903 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/upload/directory.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    62488 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/upload/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3830 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/upload/policy.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9798 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/upload/request.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3150 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/upload/result.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10750 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/src/util.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.567710 glean-sdk-52.6.0/glean-core/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2829 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/boolean.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.567710 glean-sdk-52.6.0/glean-core/tests/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5168 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/common/mod.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5334 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/counter.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13448 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/custom_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5974 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/datetime.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14362 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/event.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14418 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/labeled.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5865 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/memory_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7889 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/ping.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/ping_maker.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3611 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/quantity.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/rate.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3314 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/storage.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/string.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/string_list.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3470 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/text.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10155 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/timespan.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13005 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/timing_distribution.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3375 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/tests/uuid.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)      205 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean-core/uniffi.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18137 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/glean.1.schema.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/glean_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    96766 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29148 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-20 18:39:29.000000 glean-sdk-52.6.0/glean_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/gradle/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/gradle/wrapper/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    55616 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle/wrapper/gradle-wrapper.properties
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/gradle-plugin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle-plugin/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2094 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle-plugin/build.gradle
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/gradle-plugin/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/gradle-plugin/src/main/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/gradle-plugin/src/main/groovy/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/gradle-plugin/src/main/groovy/mozilla/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.479710 glean-sdk-52.6.0/gradle-plugin/src/main/groovy/mozilla/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26966 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/GleanGradlePlugin.groovy
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1037 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradle.properties
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5960 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradlew
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2842 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/gradlew.bat
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/build.gradle
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3426 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/proguard-rules.pro
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/androidTest/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2001 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/MainActivityTest.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/BaselinePingTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3317 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/DeletionRequestPingTest.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2963 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/SharedTestUtils.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/main/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/main/java/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/main/java/org/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/glean/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/glean/GleanApplication.kt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3224 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/glean/MainActivity.kt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/android/app/src/main/res/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/main/res/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2654 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/layout/activity_main.xml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-hdpi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.571710 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-mdpi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2096 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xhdpi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4569 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxhdpi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxxhdpi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9250 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/android/app/src/main/res/values/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1174 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/values/strings.xml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/android/app/src/main/res/xml/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/src/main/res/xml/backup_rules.xml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/android/app/tags.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/ios/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      705 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/base.xcconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/debug.xcconfig
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4062 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/AppDelegate.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Assets.xcassets/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1590 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Assets.xcassets/Contents.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Base.lproj/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Base.lproj/Main.storyboard
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Info.plist
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3290 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app/ViewController.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31215 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.pbxproj
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3382 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/glean-sample-app.xcscheme
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.575710 glean-sdk-52.6.0/samples/ios/app/glean-sample-appTests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appTests/Info.plist
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appTests/glean_sample_appTests.swift
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5083 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/BaselinePingTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3083 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/DeletionRequestPingTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3827 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/EventPingTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/Info.plist
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/MockServer.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/ViewControllerTest.swift
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/release.xcconfig
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5959 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/ios/app/sdk_generator.sh
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/samples/rust/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/rust/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/rust/build.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/rust/metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/rust/pings.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/samples/rust/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/samples/rust/src/main.rs
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2305 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/settings.gradle
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/supply-chain/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/supply-chain/audits.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7108 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/supply-chain/config.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28276 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/supply-chain/imports.lock
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/android-build/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/android-build/kind.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/beetmover/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/beetmover/kind.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/config.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/docker-image/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/docker-image/kind.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/module-build/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/module-build/kind.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/rust/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/rust/kind.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/ci/signing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/ci/signing/kind.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.483710 glean-sdk-52.6.0/taskcluster/docker/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.579710 glean-sdk-52.6.0/taskcluster/docker/linux/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4439 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/docker/linux/Dockerfile
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      187 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/docker/linux/runbuild.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      624 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/docker/linux/runlocally.sh
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/taskcluster/glean_taskgraph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2041 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/build_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/job.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/build_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3269 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/multi_dep.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/target_tasks.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2778 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/beetmover.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1374 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/module_build.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1191 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/multi_dep.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1548 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/signing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2880 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/glean_taskgraph/worker_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/requirements.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42663 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/taskcluster/scripts/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4934 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/scripts/cross-compile-setup.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/scripts/macos.manifest
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1444 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/taskcluster/scripts/rustup-setup.sh
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.487710 glean-sdk-52.6.0/tools/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.487710 glean-sdk-52.6.0/tools/analysis/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/tools/analysis/ping-patterns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2523 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/analysis/ping-patterns/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/analysis/ping-patterns/config.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15791 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/analysis/ping-patterns/ping-patterns.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/Cargo.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1874 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/src/main.rs
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 18:39:29.583711 glean-sdk-52.6.0/xcconfig/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2456 2023-04-20 18:39:04.000000 glean-sdk-52.6.0/xcconfig/common.xcconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.415633 glean-sdk-52.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.buildconfig.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.299633 glean-sdk-52.7.0/.cargo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.cargo/config
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.299633 glean-sdk-52.7.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37462 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      341 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.circleci/jazzy.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.detekt.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2006 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.dictionary
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.flake8
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.flake8rc
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.303633 glean-sdk-52.7.0/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.github/CODEOWNERS
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.github/dependabot.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.303633 glean-sdk-52.7.0/.github/workflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.github/workflows/cargo-vet.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.swiftlint.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18277 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.taskcluster.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/.yamllint
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    93022 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32171 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/Cargo.lock
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   266141 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/DEPENDENCIES.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6581 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    97487 2023-05-10 09:42:29.415633 glean-sdk-52.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      572 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/README.iOS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3773 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/about.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.303633 glean-sdk-52.7.0/bin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/about.md.hbs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/about.xml.hbs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/build-rust-docs.bat
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5594 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/build-rust-docs.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      527 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/build-swift-docs.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2062 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/build-xcframework.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1764 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/check-artifact.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56317 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/codecov.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      976 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/dependency-summary.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4788 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/prepare-release.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      591 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/publish-glean-swift.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      510 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/run-ios-build.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      540 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/run-ios-sample-app-build.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      538 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/run-ios-sample-app-test.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      508 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/run-ios-tests.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      504 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/rust-wrapper-hack.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3777 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/spellcheck.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3005 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/update-glean-parser-version.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1377 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/bin/update-schema.sh
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.307633 glean-sdk-52.7.0/build-scripts/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build-scripts/publish_to_maven_local_if_modified.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build-scripts/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build-scripts/substitute-local-glean.gradle
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      369 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build-scripts/xc-cargo.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1865 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build-scripts/xc-universal-binary.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7596 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/build.gradle
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1139 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/deny.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.307633 glean-sdk-52.7.0/docs/dev/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2072 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/SUMMARY.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.307633 glean-sdk-52.7.0/docs/dev/android/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2895 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/development-with-android-components.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      798 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/glean-parser-substitution.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1624 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/locally-published-components-in-fenix.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/sdk-ndk-versions.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3702 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/android/setup-android-build-environment.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.307633 glean-sdk-52.7.0/docs/dev/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/api/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/book.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4991 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/ci.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/code_coverage.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5424 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/contributing.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.311633 glean-sdk-52.7.0/docs/dev/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/dependency-management.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1586 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/dependency-vetting.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5402 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/documentation-guidelines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/index.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.311633 glean-sdk-52.7.0/docs/dev/core/internal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1343 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/clearing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2097 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/database.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/debug-pings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/directory-structure.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3016 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/implementations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9164 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/payload.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/reserved-ping-names.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5389 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/internal/upload.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2054 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/logging-levels.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.311633 glean-sdk-52.7.0/docs/dev/core/new-metric-type/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type/kotlin.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3744 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type/platform.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type/rust.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type/swift.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6707 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/core/new-metric-type.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11073 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/cut-a-new-release.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3841 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/docs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/glean.jpeg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.311633 glean-sdk-52.7.0/docs/dev/ios/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1577 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/ios/debug-glean-on-ios.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/ios/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1208 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/ios/setup-ios-build-environment.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.311633 glean-sdk-52.7.0/docs/dev/python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/python/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7149 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/python/setting-up-python-build-environment.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/dev/upgrading-glean-parser.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.315633 glean-sdk-52.7.0/docs/shared/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/blockquote-info.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/blockquote-stop.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/blockquote-warning.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6518 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/glean.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/mermaid-init.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6335 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/mermaid.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1122951 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/mermaid.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/tab_footer.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/tab_header.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4063 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/shared/tabs.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.315633 glean-sdk-52.7.0/docs/user/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4831 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4723 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/SUMMARY.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.315633 glean-sdk-52.7.0/docs/user/_includes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/_includes/glean-js-redirect-collected-metrics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      287 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/_includes/label-errors.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/_includes/label-limits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/_includes/labels-parameter.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1276 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/_includes/lifetimes-parameters.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/appendix/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/appendix/changelog/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/appendix/changelog/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9084 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/appendix/contribution-guidelines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3343 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/appendix/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/appendix/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8966 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/appendix/twig.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/book.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6721 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/chart-distributions-ui.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21881 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/chart-distributions.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   173077 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/chart.min.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/glean.jpeg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    48749 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/highlight.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/language-bindings/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/language-bindings/android/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3555 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/android/android-build-configuration-options.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2505 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/android/android-offline-builds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/android/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8823 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/android/instrument-android-crashes-example.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4194 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/index.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/language-bindings/ios/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/ios/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/ios/ios-build-configuration-options.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/language-bindings/javascript/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/javascript/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/javascript/index.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/language-bindings/javascript/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/javascript/plugins/encryption.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/language-bindings/javascript/plugins/index.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/docs/user/reference/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/reference/debug/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3356 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/debugViewTag.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1469 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3334 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/logPings.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.319633 glean-sdk-52.7.0/docs/user/reference/debug/screenshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   281896 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/screenshots/debug_view_tag_screenshot_swift.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298030 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/screenshots/log_pings_screenshot_swift.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   315960 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/screenshots/source_tags_screenshot_swift.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4172 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/debug/sourceTags.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.323633 glean-sdk-52.7.0/docs/user/reference/general/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/experiments-api.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1424 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/initializing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3298 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/register-custom-pings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2882 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/shutdown.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/general/toggling-upload-status.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.323633 glean-sdk-52.7.0/docs/user/reference/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5251 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/boolean.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7690 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/counter.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11088 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/custom_distribution.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9945 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/datetime.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10097 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/event.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5331 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8241 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/labeled_booleans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9183 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/labeled_counters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7292 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/labeled_strings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11734 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/memory_distribution.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6687 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/quantity.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10624 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/rate.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8214 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/string.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8863 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/string_list.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5863 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/text.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15425 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/timespan.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20616 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/timing_distribution.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8225 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/url.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8262 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/metrics/uuid.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.323633 glean-sdk-52.7.0/docs/user/reference/pings/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7240 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/pings/index.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/reference/yaml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/yaml/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10678 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/yaml/metrics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4157 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/yaml/pings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/reference/yaml/tags.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/user/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5199 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/enable-data-ingestion.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6887 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/javascript.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5252 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/kotlin.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7175 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/qt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/rust.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/swift.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/user/collected-metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12881 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/collected-metrics/metrics.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/user/debugging/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5922 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/debugging/android.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2903 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/debugging/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9495 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/debugging/ios.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/debugging/javascript.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/debugging/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4310 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/integrating-glean-for-product-managers.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    76710 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metric-lifetime-timeline.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.327633 glean-sdk-52.7.0/docs/user/user/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18606 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/adding-new-metrics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/error-reporting.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2439 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/metrics-remote-settings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5258 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/testing-metrics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3047 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/metrics/validation-checklist.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.331633 glean-sdk-52.7.0/docs/user/user/pings/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/baseline.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6458 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/custom.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2243 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/deletion-request.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3484 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/events.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12681 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7452 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/metrics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2879 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/ping-schedules-and-timings.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    87580 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/ping_timing.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4318 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/sent-by-glean.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/docs/user/user/pings/testing-custom-pings.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.331633 glean-sdk-52.7.0/glean-core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6866 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ARCHITECTURE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1906 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1699 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.331633 glean-sdk-52.7.0/glean-core/android/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10544 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/build.gradle
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15289 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/dependency-licenses.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1131 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/proguard-rules-consumer.pro
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/proguard-rules.pro
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/publish.gradle
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android/src/main/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/AndroidManifest.xml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/glean-core/android/src/main/java/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Dispatchers.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23734 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Glean.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1946 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/Configuration.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6298 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/GleanDebugActivity.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/BaseUploader.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4741 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/HttpURLConnectionUploader.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/PingUploader.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/Upload.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1707 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/Aliases.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/BooleanMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CounterMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1995 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CustomDistributionMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DatetimeMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      861 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DenominatorMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3487 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/EventMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/HistogramBase.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4843 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/LabeledMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/MemoryDistributionMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/NumeratorMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3130 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/PingType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/QuantityMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/RateMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringListMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TextMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1132 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimespanMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2219 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimingDistributionMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UrlMetricType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1251 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UuidMetricType.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1541 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/GleanLifecycleObserver.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16434 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/MetricsPingScheduler.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5466 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/PingUploadWorker.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/ErrorType.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2089 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestLocalServer.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2908 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestRule.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      683 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DataPathUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5257 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DateUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/GzipUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1323 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/JsonUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2107 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/LocaleUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      828 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/ThreadUtils.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1646 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/WorkManagerUtils.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/test/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/test/java/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/test/java/android/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/test/java/android/util/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/android/util/Log.java
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3987 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanFromJavaTest.java
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36390 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11692 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/TestUtil.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.339633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12856 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/GleanDebugActivityTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.343633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1546 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/BaseUploaderTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7832 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/HttpURLConnectionUploaderTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.343633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7208 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/CustomPingTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6386 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/DeletionPingTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.343633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2195 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/AccumulationsBeforeGleanInitTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3882 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/BooleanMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5259 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CounterMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CustomDistributionMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4422 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/DatetimeMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18328 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/EventMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16861 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/LabeledMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7157 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/MemoryDistributionMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8749 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/PingTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5500 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/QuantityMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3373 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/RateMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7437 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringListMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4560 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12105 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimespanMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12735 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimingDistributionMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4942 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UrlMetricTypeTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4032 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UuidMetricTypeTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.343633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32702 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/MetricsPingSchedulerTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2494 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/PingUploadWorkerTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/ShadowLog.java
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1010 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DataPathUtilsTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DateUtilsTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/GzipUtilsTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2068 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/JsonUtilsTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/KArgumentCaptor.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/android/src/test/resources/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/android/src/test/resources/mockito-extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/resources/mockito-extensions/org.mockito.plugins.MockMaker
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android/src/test/resources/robolectric.properties
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android-native/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4376 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/build.gradle
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15289 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/dependency-licenses.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/proguard-rules-consumer.pro
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/proguard-rules.pro
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7614 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/publish.gradle
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.283633 glean-sdk-52.7.0/glean-core/android-native/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.335633 glean-sdk-52.7.0/glean-core/android-native/src/main/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/android-native/src/main/AndroidManifest.xml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/build/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      364 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/build/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/build/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/build/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/build/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3367 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/build/src/lib.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/build.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/bundle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/bundle/Cargo.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/bundle/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/bundle/src/lib.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/bundle-android/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/bundle-android/Cargo.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/ios/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.347633 glean-sdk-52.7.0/glean-core/ios/Glean/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1728 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Config/Configuration.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean/Debug/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7256 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Debug/GleanDebugTools.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1219 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Dispatchers.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Glean.h
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20451 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Glean.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/GleanMetrics.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Info.plist
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/BooleanMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/CounterMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3603 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/DatetimeMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/EventMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4399 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/LabeledMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/MemoryDistributionMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/Ping.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/QuantityMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1898 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/RateMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      753 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/StringListMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/StringMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      681 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TextMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1962 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TimespanMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TimingDistributionMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2464 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/UrlMetric.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2025 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/UuidMetric.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean/Net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8412 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Net/HttpPingUploader.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/Glean/Scheduler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1487 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Scheduler/GleanLifecycleObserver.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10362 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Scheduler/MetricsPingScheduler.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/Glean/Utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Logger.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7359 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Sysctl.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2409 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Unreachable.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6417 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Utils.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51892 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.pbxproj
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.287633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/xcshareddata/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.351633 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3541 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/Glean.xcscheme
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/GleanTests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Config/ConfigurationTests.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Debug/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3928 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Debug/GleanDebugUtilityTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13549 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/GleanTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Info.plist
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.355633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/BooleanMetricTypeTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/CounterMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6530 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/DatetimeMetricTypeTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11062 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/EventMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7967 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/LabeledMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4791 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/MemoryDistributionMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5941 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/PingTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3304 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/QuantityMetricTypeTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/RateMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5453 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/StringListMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/StringMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7367 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/TimespanMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6516 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/TimingDistributionMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4364 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/UrlMetricTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2879 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/UuidMetricTests.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7588 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/BaselinePingTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6306 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/DeletionRequestPingTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4074 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/HttpPingUploaderTests.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Scheduler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14876 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Scheduler/MetricsPingSchedulerTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4939 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/TestUtils.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/ios/GleanTests/Utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/GleanTests/Utils/DataPathUtilsTests.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/base.xcconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/debug.xcconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/release.xcconfig
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5959 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/ios/sdk_generator.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/megazord.uniffi.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22678 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/pings.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      376 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/.gitignore
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/python/glean/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_builtins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1698 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_ffi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10319 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5189 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_process_dispatcher.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.359633 glean-sdk-52.7.0/glean-core/python/glean/_subprocess/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_subprocess/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14545 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/glean.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.363633 glean-sdk-52.7.0/glean-core/python/glean/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3787 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/datetime.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3303 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3225 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/labeled.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2079 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/ping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/string.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4395 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/timespan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4475 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/timing_distribution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1628 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/metrics/uuid.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.363633 glean-sdk-52.7.0/glean-core/python/glean/net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/net/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/net/base_uploader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3212 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/net/http_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5010 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/net/ping_upload_worker.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/net/ping_uploader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.363633 glean-sdk-52.7.0/glean-core/python/glean/testing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2883 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/glean/testing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/requirements_dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9281 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.363633 glean-sdk-52.7.0/glean-core/python/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2889 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.363633 glean-sdk-52.7.0/glean-core/python/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8088 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/data/core.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/data/events_with_types.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/data/glinter.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/data/pings.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.367633 glean-sdk-52.7.0/glean-core/python/tests/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2163 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_boolean.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3757 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_counter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3059 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_datetime.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12498 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6873 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_labeled.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_memory_distribution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3639 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_quantity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2768 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_string.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3795 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_string_list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_timespan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5858 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_timing_distribution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3418 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6456 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/metrics/test_uuid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26265 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/test_glean.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/test_loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6584 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/test_network.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      509 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/python/tests/test_subprocess.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.367633 glean-sdk-52.7.0/glean-core/rlb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.367633 glean-sdk-52.7.0/glean-core/rlb/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/examples/long-running.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1925 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/examples/prototype.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.371633 glean-sdk-52.7.0/glean-core/rlb/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/common_test.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5780 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/configuration.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1425 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/core_metrics.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9464 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/lib.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.371633 glean-sdk-52.7.0/glean-core/rlb/src/net/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      895 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/net/http_uploader.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7703 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/net/mod.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.371633 glean-sdk-52.7.0/glean-core/rlb/src/private/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7269 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/private/event.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1188 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/private/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2929 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/private/ping.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3836 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/system.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47172 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/src/test.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.371633 glean-sdk-52.7.0/glean-core/rlb/tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.371633 glean-sdk-52.7.0/glean-core/rlb/tests/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/common/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/init_fails.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2051 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/never_init.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2238 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/no_time_to_init.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3008 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/overflowing_preinit.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2812 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/persist_ping_lifetime.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/persist_ping_lifetime_nopanic.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6920 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/schema.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2454 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/simple.rs
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      729 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/test-shutdown-blocking.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7395 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/rlb/tests/upload_timing.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4701 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/common_metric_data.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34663 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/core/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7409 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/core_metrics.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1776 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/coverage.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65434 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/database/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10925 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/debug.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/dispatcher/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7202 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/dispatcher/global.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19223 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/dispatcher/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4755 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/error.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8362 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/error_recording.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/event_database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    48613 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/event_database/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2603 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/fd_logger.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16753 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/glean.udl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/glean_metrics.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.379633 glean-sdk-52.7.0/glean-core/src/histogram/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6962 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/histogram/exponential.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/histogram/functional.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/histogram/linear.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3957 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/histogram/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9242 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/internal_metrics.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2105 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/internal_pings.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42289 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/lib.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36226 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/lib_unit_tests.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.383633 glean-sdk-52.7.0/glean-core/src/metrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3994 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/boolean.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/counter.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7537 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/custom_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10531 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/datetime.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4445 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/denominator.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6200 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/event.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9572 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/experiment.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10013 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/labeled.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9666 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/memory_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1837 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/memory_unit.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/metrics_enabled_config.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11590 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3025 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/numerator.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7190 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/ping.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3691 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/quantity.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5836 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/rate.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1573 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/recorded_experiment.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5307 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/string.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6385 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/string_list.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/text.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3795 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/time_unit.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10280 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/timespan.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18625 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/timing_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10166 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/url.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4936 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/metrics/uuid.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.383633 glean-sdk-52.7.0/glean-core/src/ping/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13588 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/ping/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23631 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/scheduler.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.383633 glean-sdk-52.7.0/glean-core/src/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9355 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/storage/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2856 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/system.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.387633 glean-sdk-52.7.0/glean-core/src/traits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/boolean.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1497 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/counter.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1994 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/custom_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/datetime.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3815 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/event.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/labeled.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1804 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/memory_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/numerator.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/ping.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/quantity.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1823 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/rate.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1574 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/string.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/string_list.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/text.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/timespan.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2531 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/timing_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/url.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1528 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/traits/uuid.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.391633 glean-sdk-52.7.0/glean-core/src/upload/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14903 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/upload/directory.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    62488 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/upload/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3830 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/upload/policy.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9798 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/upload/request.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3150 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/upload/result.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10750 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/src/util.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.391633 glean-sdk-52.7.0/glean-core/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2829 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/boolean.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.391633 glean-sdk-52.7.0/glean-core/tests/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5193 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/common/mod.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5334 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/counter.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13448 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/custom_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5974 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/datetime.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14362 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/event.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14418 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/labeled.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5865 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/memory_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7889 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/ping.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/ping_maker.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3611 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/quantity.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/rate.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3314 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/storage.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/string.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/string_list.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3470 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/text.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10155 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/timespan.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13005 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/timing_distribution.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3375 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/tests/uuid.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      205 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean-core/uniffi.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18137 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/glean.1.schema.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/glean_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    97487 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29148 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-10 09:42:29.000000 glean-sdk-52.7.0/glean_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/gradle/wrapper/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55616 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle/wrapper/gradle-wrapper.properties
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/gradle-plugin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle-plugin/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2094 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle-plugin/build.gradle
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle-plugin/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle-plugin/src/main/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle-plugin/src/main/groovy/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle-plugin/src/main/groovy/mozilla/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/gradle-plugin/src/main/groovy/mozilla/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26966 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/GleanGradlePlugin.groovy
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1037 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradle.properties
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5960 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradlew
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2842 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/gradlew.bat
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/samples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/samples/android/app/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/build.gradle
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3426 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/proguard-rules.pro
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/androidTest/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2001 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/MainActivityTest.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/BaselinePingTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3317 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/DeletionRequestPingTest.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2963 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/SharedTestUtils.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.395633 glean-sdk-52.7.0/samples/android/app/src/main/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/main/java/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/main/java/org/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.291633 glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/glean/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/glean/GleanApplication.kt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3224 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/glean/MainActivity.kt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/samples/android/app/src/main/res/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2654 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/layout/activity_main.xml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-hdpi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-mdpi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2096 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xhdpi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4569 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxhdpi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxxhdpi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9250 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/values/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1174 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/values/strings.xml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/android/app/src/main/res/xml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/src/main/res/xml/backup_rules.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/android/app/tags.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/samples/ios/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/ios/app/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      705 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/base.xcconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/debug.xcconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.399633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4062 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/AppDelegate.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Assets.xcassets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1590 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Assets.xcassets/Contents.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Base.lproj/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Base.lproj/Main.storyboard
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Info.plist
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3290 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app/ViewController.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31215 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.pbxproj
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3382 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/glean-sample-app.xcscheme
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-appTests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appTests/Info.plist
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appTests/glean_sample_appTests.swift
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.403633 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5083 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/BaselinePingTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3083 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/DeletionRequestPingTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3827 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/EventPingTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/Info.plist
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/MockServer.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/ViewControllerTest.swift
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      696 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/release.xcconfig
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     5959 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/ios/app/sdk_generator.sh
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/samples/rust/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/rust/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/rust/build.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/rust/metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/rust/pings.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/samples/rust/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1610 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/samples/rust/src/main.rs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2305 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/settings.gradle
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-10 09:42:29.415633 glean-sdk-52.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/supply-chain/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/supply-chain/audits.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7108 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/supply-chain/config.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28276 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/supply-chain/imports.lock
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/android-build/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/android-build/kind.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/beetmover/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/beetmover/kind.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/config.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/docker-image/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/docker-image/kind.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/module-build/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/module-build/kind.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/rust/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/rust/kind.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/ci/signing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/ci/signing/kind.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/taskcluster/docker/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.407633 glean-sdk-52.7.0/taskcluster/docker/linux/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4439 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/docker/linux/Dockerfile
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      187 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/docker/linux/runbuild.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      624 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/docker/linux/runlocally.sh
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/taskcluster/glean_taskgraph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2041 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/build_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/job.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/build_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3269 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/multi_dep.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/target_tasks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2778 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/beetmover.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1374 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/module_build.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1191 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/multi_dep.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1548 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/signing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2880 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/glean_taskgraph/worker_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/requirements.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42663 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/taskcluster/scripts/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4934 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/scripts/cross-compile-setup.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/scripts/macos.manifest
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1444 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/taskcluster/scripts/rustup-setup.sh
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/tools/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.295633 glean-sdk-52.7.0/tools/analysis/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/tools/analysis/ping-patterns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2523 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/analysis/ping-patterns/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/analysis/ping-patterns/config.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    15791 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/analysis/ping-patterns/ping-patterns.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/Cargo.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.411633 glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1874 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/src/main.rs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 09:42:29.415633 glean-sdk-52.7.0/xcconfig/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2456 2023-05-10 09:42:09.000000 glean-sdk-52.7.0/xcconfig/common.xcconfig
```

### Comparing `glean-sdk-52.6.0/.buildconfig.yml` & `glean-sdk-52.7.0/.buildconfig.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-libraryVersion: 52.6.0
+libraryVersion: 52.7.0
 groupId: org.mozilla.telemetry
 projects:
   glean:
     path: glean-core/android
     artifactId: glean
     publications:
       - name: glean
```

### Comparing `glean-sdk-52.6.0/.circleci/config.yml` & `glean-sdk-52.7.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.detekt.yml` & `glean-sdk-52.7.0/.detekt.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.dictionary` & `glean-sdk-52.7.0/.dictionary`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.github/workflows/cargo-vet.yml` & `glean-sdk-52.7.0/.github/workflows/cargo-vet.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.gitignore` & `glean-sdk-52.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.swiftlint.yml` & `glean-sdk-52.7.0/.swiftlint.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/.taskcluster.yml` & `glean-sdk-52.7.0/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/CHANGELOG.md` & `glean-sdk-52.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # Unreleased changes
 
-[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...main)
+[Full changelog](https://github.com/mozilla/glean/compare/v52.7.0...main)
+
+# v52.7.0 (2023-05-10)
+
+[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...v52.7.0)
+
+* General
+  * Allow user to configure how verbose the internal logging is ([#2459](https://github.com/mozilla/glean/pull/2459))
+  * Added a timeout waiting for the dispatcher at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+  * Added a new Glean metric `glean.validation.shutdown_dispatcher_wait` measuring the wait time at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+* Kotlin
+  * Update Kotlin to version 1.8.21 ([#2462](https://github.com/mozilla/glean/pull/2462))
+  * Make debugging APIs available on Android ([Bug 1830937](https://bugzilla.mozilla.org/show_bug.cgi?id=1830937))
 
 # v52.6.0 (2023-04-20)
 
 [Full changelog](https://github.com/mozilla/glean/compare/v52.5.0...v52.6.0)
 
 * Rust
   * The Text metric type is now available in the Rust language bindings ([#2451](https://github.com/mozilla/glean/pull/2451))
```

### Comparing `glean-sdk-52.6.0/Cargo.lock` & `glean-sdk-52.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "glean"
-version = "52.6.0"
+version = "52.7.0"
 dependencies = [
  "chrono",
  "crossbeam-channel",
  "env_logger",
  "flate2",
  "glean-core",
  "inherent",
@@ -357,15 +357,15 @@
 version = "1.0.0"
 dependencies = [
  "glean-core",
 ]
 
 [[package]]
 name = "glean-core"
-version = "52.6.0"
+version = "52.7.0"
 dependencies = [
  "android_logger",
  "bincode",
  "chrono",
  "crossbeam-channel",
  "ctor",
  "env_logger",
```

### Comparing `glean-sdk-52.6.0/DEPENDENCIES.md` & `glean-sdk-52.7.0/DEPENDENCIES.md`

 * *Files 0% similar despite different names*

```diff
@@ -14274,22 +14274,22 @@
 00037c10: 4c69 6365 6e73 6520 322e 300a 3c73 7061  License 2.0.<spa
 00037c20: 6e20 6964 3d22 4d50 4c2d 322e 3022 3e3c  n id="MPL-2.0"><
 00037c30: 2f73 7061 6e3e 0a0a 5468 6520 666f 6c6c  /span>..The foll
 00037c40: 6f77 696e 6720 7465 7874 2061 7070 6c69  owing text appli
 00037c50: 6573 2074 6f20 636f 6465 206c 696e 6b65  es to code linke
 00037c60: 6420 6672 6f6d 2074 6865 7365 2064 6570  d from these dep
 00037c70: 656e 6465 6e63 6965 733a 0a0a 2a20 5b67  endencies:..* [g
-00037c80: 6c65 616e 2035 322e 362e 305d 2820 6874  lean 52.6.0]( ht
+00037c80: 6c65 616e 2035 322e 372e 305d 2820 6874  lean 52.7.0]( ht
 00037c90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00037ca0: 2f6d 6f7a 696c 6c61 2f67 6c65 616e 2029  /mozilla/glean )
 00037cb0: 0a2a 205b 676c 6561 6e2d 6275 696c 6420  .* [glean-build 
 00037cc0: 372e 312e 305d 2820 6874 7470 733a 2f2f  7.1.0]( https://
 00037cd0: 6769 7468 7562 2e63 6f6d 2f6d 6f7a 696c  github.com/mozil
 00037ce0: 6c61 2f67 6c65 616e 2029 0a2a 205b 676c  la/glean ).* [gl
-00037cf0: 6561 6e2d 636f 7265 2035 322e 362e 305d  ean-core 52.6.0]
+00037cf0: 6561 6e2d 636f 7265 2035 322e 372e 305d  ean-core 52.7.0]
 00037d00: 2820 6874 7470 733a 2f2f 6769 7468 7562  ( https://github
 00037d10: 2e63 6f6d 2f6d 6f7a 696c 6c61 2f67 6c65  .com/mozilla/gle
 00037d20: 616e 2029 0a2a 205b 7a65 6974 7374 656d  an ).* [zeitstem
 00037d30: 7065 6c20 302e 312e 315d 2820 6874 7470  pel 0.1.1]( http
 00037d40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
 00037d50: 6164 626f 792f 7a65 6974 7374 656d 7065  adboy/zeitstempe
 00037d60: 6c20 290a 0a60 6060 0a4d 6f7a 696c 6c61  l )..```.Mozilla
```

### Comparing `glean-sdk-52.6.0/LICENSE` & `glean-sdk-52.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/Makefile` & `glean-sdk-52.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/PKG-INFO` & `glean-sdk-52.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-sdk
-Version: 52.6.0
+Version: 52.7.0
 Summary: Mozilla's Glean Telemetry SDK: The Machine that Goes 'Ping!'
 Home-page: https://github.com/mozilla/glean
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -85,15 +85,27 @@
 [devbook]: https://mozilla.github.io/glean/dev/
 [rustdoc]: https://mozilla.github.io/glean/docs/index.html
 [ktdoc]: https://mozilla.github.io/glean/javadoc/glean/index.html
 
 
 # Unreleased changes
 
-[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...main)
+[Full changelog](https://github.com/mozilla/glean/compare/v52.7.0...main)
+
+# v52.7.0 (2023-05-10)
+
+[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...v52.7.0)
+
+* General
+  * Allow user to configure how verbose the internal logging is ([#2459](https://github.com/mozilla/glean/pull/2459))
+  * Added a timeout waiting for the dispatcher at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+  * Added a new Glean metric `glean.validation.shutdown_dispatcher_wait` measuring the wait time at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+* Kotlin
+  * Update Kotlin to version 1.8.21 ([#2462](https://github.com/mozilla/glean/pull/2462))
+  * Make debugging APIs available on Android ([Bug 1830937](https://bugzilla.mozilla.org/show_bug.cgi?id=1830937))
 
 # v52.6.0 (2023-04-20)
 
 [Full changelog](https://github.com/mozilla/glean/compare/v52.5.0...v52.6.0)
 
 * Rust
   * The Text metric type is now available in the Rust language bindings ([#2451](https://github.com/mozilla/glean/pull/2451))
```

### Comparing `glean-sdk-52.6.0/README.iOS.md` & `glean-sdk-52.7.0/README.iOS.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/README.md` & `glean-sdk-52.7.0/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/about.toml` & `glean-sdk-52.7.0/about.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/about.md.hbs` & `glean-sdk-52.7.0/bin/about.md.hbs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/build-rust-docs.bat` & `glean-sdk-52.7.0/bin/build-rust-docs.bat`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/build-rust-docs.sh` & `glean-sdk-52.7.0/bin/build-rust-docs.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/build-swift-docs.sh` & `glean-sdk-52.7.0/bin/build-swift-docs.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/build-xcframework.sh` & `glean-sdk-52.7.0/bin/build-xcframework.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/check-artifact.sh` & `glean-sdk-52.7.0/bin/check-artifact.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/codecov.sh` & `glean-sdk-52.7.0/bin/codecov.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/dependency-summary.sh` & `glean-sdk-52.7.0/bin/dependency-summary.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/prepare-release.sh` & `glean-sdk-52.7.0/bin/prepare-release.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/publish-glean-swift.sh` & `glean-sdk-52.7.0/bin/publish-glean-swift.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/run-ios-sample-app-build.sh` & `glean-sdk-52.7.0/bin/run-ios-sample-app-build.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/run-ios-sample-app-test.sh` & `glean-sdk-52.7.0/bin/run-ios-sample-app-test.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/spellcheck.sh` & `glean-sdk-52.7.0/bin/spellcheck.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/update-glean-parser-version.sh` & `glean-sdk-52.7.0/bin/update-glean-parser-version.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/bin/update-schema.sh` & `glean-sdk-52.7.0/bin/update-schema.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/build-scripts/publish_to_maven_local_if_modified.py` & `glean-sdk-52.7.0/build-scripts/publish_to_maven_local_if_modified.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/build-scripts/shared.py` & `glean-sdk-52.7.0/build-scripts/shared.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/build-scripts/substitute-local-glean.gradle` & `glean-sdk-52.7.0/build-scripts/substitute-local-glean.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/build-scripts/xc-universal-binary.sh` & `glean-sdk-52.7.0/build-scripts/xc-universal-binary.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/build.gradle` & `glean-sdk-52.7.0/build.gradle`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 // https://github.com/mozilla/application-services/blob/84e077d1534dc287bbd472da658ce22eea5af032/build.gradle
 
 buildscript {
     // Define the version of the used dependencies in a single place, to ease
     // changing them. Please note that, for using in Android-Components, the
     // versions below must match the ones in that repository.
     ext.versions = [
-        android_gradle_plugin: '7.4.1',
+        android_gradle_plugin: '7.4.2',
         coroutines: '1.6.4',
         jna: '5.13.0',
         junit: '4.12',
         mockito: '3.11.2',
         mockwebserver: '4.9.1', // This is different than a-c, but we're fine, it's only tests.
-        kotlin: '1.8.10',
-        robolectric: '4.9.2',
+        kotlin: '1.8.21',
+        robolectric: '4.10.1',
         rust_android_plugin: '0.9.3',
 
         // Android X dependencies
-        androidx_annotation: '1.5.0',
-        androidx_appcompat: '1.3.0',
-        androidx_browser: '1.3.0',
-        androidx_core: '1.9.0',
+        androidx_annotation: '1.6.0',
+        androidx_appcompat: '1.6.1',
+        androidx_browser: '1.5.0',
+        androidx_core: '1.10.0',
         androidx_espresso: '3.5.1',
         androidx_junit: '1.1.5',
-        androidx_lifecycle: '2.5.1',
+        androidx_lifecycle: '2.6.1',
         androidx_test: '1.5.0',
         androidx_work: '2.7.1',
         androidx_uiautomator: '2.2.0',
     ]
 
     ext.build = [
         ndkVersion: "25.2.9519653", // Keep it in sync in TC Dockerfile.
```

### Comparing `glean-sdk-52.6.0/deny.toml` & `glean-sdk-52.7.0/deny.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/README.md` & `glean-sdk-52.7.0/docs/dev/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/SUMMARY.md` & `glean-sdk-52.7.0/docs/dev/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/android/development-with-android-components.md` & `glean-sdk-52.7.0/docs/dev/android/development-with-android-components.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/android/glean-parser-substitution.md` & `glean-sdk-52.7.0/docs/dev/android/glean-parser-substitution.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/android/locally-published-components-in-fenix.md` & `glean-sdk-52.7.0/docs/dev/android/locally-published-components-in-fenix.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/android/sdk-ndk-versions.md` & `glean-sdk-52.7.0/docs/dev/android/sdk-ndk-versions.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/android/setup-android-build-environment.md` & `glean-sdk-52.7.0/docs/dev/android/setup-android-build-environment.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/book.toml` & `glean-sdk-52.7.0/docs/dev/book.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/ci.md` & `glean-sdk-52.7.0/docs/dev/ci.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/code_coverage.md` & `glean-sdk-52.7.0/docs/dev/code_coverage.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/contributing.md` & `glean-sdk-52.7.0/docs/dev/contributing.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/dependency-management.md` & `glean-sdk-52.7.0/docs/dev/core/dependency-management.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/dependency-vetting.md` & `glean-sdk-52.7.0/docs/dev/core/dependency-vetting.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/documentation-guidelines.md` & `glean-sdk-52.7.0/docs/dev/core/documentation-guidelines.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/clearing.md` & `glean-sdk-52.7.0/docs/dev/core/internal/clearing.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/database.md` & `glean-sdk-52.7.0/docs/dev/core/internal/database.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/debug-pings.md` & `glean-sdk-52.7.0/docs/dev/core/internal/debug-pings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/directory-structure.md` & `glean-sdk-52.7.0/docs/dev/core/internal/directory-structure.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/implementations.md` & `glean-sdk-52.7.0/docs/dev/core/internal/implementations.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/index.md` & `glean-sdk-52.7.0/docs/dev/core/internal/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/payload.md` & `glean-sdk-52.7.0/docs/dev/core/internal/payload.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/reserved-ping-names.md` & `glean-sdk-52.7.0/docs/dev/core/internal/reserved-ping-names.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/internal/upload.md` & `glean-sdk-52.7.0/docs/dev/core/internal/upload.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/logging-levels.md` & `glean-sdk-52.7.0/docs/dev/core/logging-levels.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type/kotlin.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type/kotlin.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type/platform.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type/platform.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type/python.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type/python.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type/rust.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type/rust.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type/swift.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type/swift.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/core/new-metric-type.md` & `glean-sdk-52.7.0/docs/dev/core/new-metric-type.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/cut-a-new-release.md` & `glean-sdk-52.7.0/docs/dev/cut-a-new-release.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/docs.md` & `glean-sdk-52.7.0/docs/dev/docs.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/glean.jpeg` & `glean-sdk-52.7.0/docs/dev/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/ios/debug-glean-on-ios.md` & `glean-sdk-52.7.0/docs/dev/ios/debug-glean-on-ios.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/ios/setup-ios-build-environment.md` & `glean-sdk-52.7.0/docs/dev/ios/setup-ios-build-environment.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/python/setting-up-python-build-environment.md` & `glean-sdk-52.7.0/docs/dev/python/setting-up-python-build-environment.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/testing.md` & `glean-sdk-52.7.0/docs/dev/testing.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/dev/upgrading-glean-parser.md` & `glean-sdk-52.7.0/docs/dev/upgrading-glean-parser.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/shared/glean.css` & `glean-sdk-52.7.0/docs/shared/glean.css`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/shared/mermaid.css` & `glean-sdk-52.7.0/docs/shared/mermaid.css`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/shared/mermaid.min.js` & `glean-sdk-52.7.0/docs/shared/mermaid.min.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/shared/tabs.js` & `glean-sdk-52.7.0/docs/shared/tabs.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/README.md` & `glean-sdk-52.7.0/docs/user/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/SUMMARY.md` & `glean-sdk-52.7.0/docs/user/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/_includes/labels-parameter.md` & `glean-sdk-52.7.0/docs/user/_includes/labels-parameter.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/_includes/lifetimes-parameters.md` & `glean-sdk-52.7.0/docs/user/_includes/lifetimes-parameters.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/appendix/contribution-guidelines.md` & `glean-sdk-52.7.0/docs/user/appendix/contribution-guidelines.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/appendix/glossary.md` & `glean-sdk-52.7.0/docs/user/appendix/glossary.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/appendix/twig.md` & `glean-sdk-52.7.0/docs/user/appendix/twig.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/book.toml` & `glean-sdk-52.7.0/docs/user/book.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/chart-distributions-ui.js` & `glean-sdk-52.7.0/docs/user/chart-distributions-ui.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/chart-distributions.js` & `glean-sdk-52.7.0/docs/user/chart-distributions.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/chart.min.js` & `glean-sdk-52.7.0/docs/user/chart.min.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/glean.jpeg` & `glean-sdk-52.7.0/docs/user/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/highlight.js` & `glean-sdk-52.7.0/docs/user/highlight.js`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/android/android-build-configuration-options.md` & `glean-sdk-52.7.0/docs/user/language-bindings/android/android-build-configuration-options.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/android/android-offline-builds.md` & `glean-sdk-52.7.0/docs/user/language-bindings/android/android-offline-builds.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/android/instrument-android-crashes-example.md` & `glean-sdk-52.7.0/docs/user/language-bindings/android/instrument-android-crashes-example.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/index.md` & `glean-sdk-52.7.0/docs/user/language-bindings/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/ios/ios-build-configuration-options.md` & `glean-sdk-52.7.0/docs/user/language-bindings/ios/ios-build-configuration-options.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/javascript/cli.md` & `glean-sdk-52.7.0/docs/user/language-bindings/javascript/cli.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/javascript/plugins/encryption.md` & `glean-sdk-52.7.0/docs/user/language-bindings/javascript/plugins/encryption.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/language-bindings/javascript/plugins/index.md` & `glean-sdk-52.7.0/docs/user/language-bindings/javascript/plugins/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/debugViewTag.md` & `glean-sdk-52.7.0/docs/user/reference/debug/debugViewTag.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/index.md` & `glean-sdk-52.7.0/docs/user/reference/debug/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/logPings.md` & `glean-sdk-52.7.0/docs/user/reference/debug/logPings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/screenshots/debug_view_tag_screenshot_swift.png` & `glean-sdk-52.7.0/docs/user/reference/debug/screenshots/debug_view_tag_screenshot_swift.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/screenshots/log_pings_screenshot_swift.png` & `glean-sdk-52.7.0/docs/user/reference/debug/screenshots/log_pings_screenshot_swift.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/screenshots/source_tags_screenshot_swift.png` & `glean-sdk-52.7.0/docs/user/reference/debug/screenshots/source_tags_screenshot_swift.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/debug/sourceTags.md` & `glean-sdk-52.7.0/docs/user/reference/debug/sourceTags.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/experiments-api.md` & `glean-sdk-52.7.0/docs/user/reference/general/experiments-api.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/index.md` & `glean-sdk-52.7.0/docs/user/reference/general/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/initializing.md` & `glean-sdk-52.7.0/docs/user/reference/general/initializing.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 - `appBuild`: A build identifier e.g. the build identifier generated by a CI system (e.g. "1234/A"). If not present, `app_build` will be reported as "Unknown" on all pings [`client_info`](../../user/pings/index.html#the-client_info-section) section.
 - `appDisplayVersion`: The user visible version string for the application running Glean. If not present, `app_display_version` will be reported as "Unknown" on all pings [`client_info`](../../user/pings/index.html#the-client_info-section) section.
 - `serverEndpoint`: The server pings are sent to. Defaults to `https://incoming.telemetry.mozilla.org`.
 - `maxEvents`: The maximum number of events the Glean storage will hold on to before submitting the 'events' ping. Defaults to 500. Refer to the [`events` ping documentation](../../user/pings/events.md) for more information on its scheduling.
 - `httpUploader`: A custom HTTP uploader instance, that will overwrite Glean's provided uploader. Useful
 for users that wish to use specific uploader implementations. See [Custom Uploaders](#custom-uploaders)
 for more information on how and when the use this feature.
+- `logLevel`: The level for how verbose the internal logging is. The level filter options in order from least to most verbose are: `Off`, `Error`, `Warn`, `Info`, `Debug`, `Trace`. See the [`log` crate docs](https://docs.rs/log/latest/log/) for more information.
 
 To learn about SDK specific configuration options available, refer to the [Reference](#reference) section.
 
 {{#include ../../../shared/blockquote-stop.html}}
 
 ##### Always initialize Glean with the correct upload preference
```

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/register-custom-pings.md` & `glean-sdk-52.7.0/docs/user/reference/general/register-custom-pings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/shutdown.md` & `glean-sdk-52.7.0/docs/user/reference/general/shutdown.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/general/toggling-upload-status.md` & `glean-sdk-52.7.0/docs/user/reference/general/toggling-upload-status.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/boolean.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/boolean.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/counter.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/counter.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/custom_distribution.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/custom_distribution.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/datetime.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/datetime.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/event.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/event.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/index.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/labeled_booleans.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/labeled_booleans.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/labeled_counters.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/labeled_counters.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/labeled_strings.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/labeled_strings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/memory_distribution.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/memory_distribution.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/quantity.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/quantity.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/rate.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/rate.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/string.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/string.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/string_list.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/string_list.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/text.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/text.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/timespan.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/timespan.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/timing_distribution.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/timing_distribution.md`

 * *Files 4% similar despite different names*

```diff
@@ -235,14 +235,109 @@
 Glean.pages.pageLoad.stopAndAccumulate(timerId);
 ```
 
 </div>
 
 {{#include ../../../shared/tab_footer.md}}
 
+### `accumulateSamples`
+
+Accumulates the provided signed samples in the metric.
+This is required so that the platform-specific code can provide us with
+64 bit signed integers if no `u64` comparable type is available. This
+will take care of filtering and reporting errors for any provided negative
+sample.
+
+Please note that this assumes that the provided samples are already in
+the "unit" declared by the instance of the metric type (e.g. if the
+instance this method was called on is using `TimeUnit::Second`, then
+`samples` are assumed to be in that unit).
+
+{{#include ../../../shared/tab_header.md}}
+
+<div data-lang="Kotlin" class="tab">
+
+```Kotlin
+import org.mozilla.yourApplication.GleanMetrics.Pages
+
+fun onPageLoaded(e: Event) {
+    Pages.pageLoad.accumulateSamples(samples)
+}
+```
+
+</div>
+<div data-lang="Java" class="tab">
+
+```Java
+import org.mozilla.yourApplication.GleanMetrics.Pages;
+
+void onPageLoaded(Event e) {
+    Pages.INSTANCE.pageLoad().accumulateSamples(samples);
+}
+```
+
+</div>
+<div data-lang="Swift" class="tab">
+
+```Swift
+import Glean
+
+func onPageLoaded() {
+    Pages.pageLoad.accumulateSamples(samples)
+}
+```
+
+</div>
+<div data-lang="Python" class="tab">
+
+```Python
+from glean import load_metrics
+metrics = load_metrics("metrics.yaml")
+
+class PageHandler:
+    def on_page_loaded(self, event):
+        metrics.pages.page_load.accumulate_samples(samples)
+```
+
+</div>
+<div data-lang="Rust" class="tab">
+
+This API is not currently exposed in Rust, see [Bug 1829745](https://bugzilla.mozilla.org/show_bug.cgi?id=1829745).
+
+</div>
+<div data-lang="JavaScript" class="tab">
+
+```Javascript
+import * as pages from "./path/to/generated/files/pages.js";
+
+function onPageLoaded() {
+    pages.pageLoad.accumulateSamples(samples);
+}
+```
+
+</div>
+<div data-lang="Firefox Desktop" class="tab">
+
+This API is not currently exposed in Firefox Desktop, see [Bug 1829745](https://bugzilla.mozilla.org/show_bug.cgi?id=1829745).
+
+</div>
+
+#### Limits
+
+- Samples are limited to the maximum value for the given time unit.
+- Only non-negative values may be recorded (`>= 0`).
+
+#### Recorded Errors
+
+- Negative values are discarded and an `ErrorType::InvalidValue` is generated for each instance.
+- Samples that are longer than maximum sample time for the given unit generate an `ErrorType::InvalidOverflow` error for each instance.
+
+{{#include ../../../shared/tab_footer.md}}
+
+
 #### Recorded errors
 
 * [`invalid_value`](../../user/metrics/error-reporting.md): If recording a negative timespan.
 * [`invalid_state`](../../user/metrics/error-reporting.md): If a non-existing/stopped timer is stopped again.
 * [`invalid_overflow`](../../user/metrics/error-reporting.md): If recording a time longer than the maximum for the given unit.
 
 ### `measure`
```

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/url.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/url.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/metrics/uuid.md` & `glean-sdk-52.7.0/docs/user/reference/metrics/uuid.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/pings/index.md` & `glean-sdk-52.7.0/docs/user/reference/pings/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/yaml/index.md` & `glean-sdk-52.7.0/docs/user/reference/yaml/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/yaml/metrics.md` & `glean-sdk-52.7.0/docs/user/reference/yaml/metrics.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/yaml/pings.md` & `glean-sdk-52.7.0/docs/user/reference/yaml/pings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/reference/yaml/tags.md` & `glean-sdk-52.7.0/docs/user/reference/yaml/tags.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/enable-data-ingestion.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/enable-data-ingestion.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/index.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/javascript.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/javascript.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/kotlin.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/kotlin.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/python.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/python.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/qt.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/qt.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/rust.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/rust.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/adding-glean-to-your-project/swift.md` & `glean-sdk-52.7.0/docs/user/user/adding-glean-to-your-project/swift.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/collected-metrics/metrics.md` & `glean-sdk-52.7.0/docs/user/user/collected-metrics/metrics.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/debugging/android.md` & `glean-sdk-52.7.0/docs/user/user/debugging/android.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/debugging/index.md` & `glean-sdk-52.7.0/docs/user/user/debugging/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/debugging/ios.md` & `glean-sdk-52.7.0/docs/user/user/debugging/ios.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/debugging/javascript.md` & `glean-sdk-52.7.0/docs/user/user/debugging/javascript.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/debugging/python.md` & `glean-sdk-52.7.0/docs/user/user/debugging/python.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/integrating-glean-for-product-managers.md` & `glean-sdk-52.7.0/docs/user/user/integrating-glean-for-product-managers.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metric-lifetime-timeline.svg` & `glean-sdk-52.7.0/docs/user/user/metric-lifetime-timeline.svg`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metrics/adding-new-metrics.md` & `glean-sdk-52.7.0/docs/user/user/metrics/adding-new-metrics.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metrics/error-reporting.md` & `glean-sdk-52.7.0/docs/user/user/metrics/error-reporting.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metrics/metrics-remote-settings.md` & `glean-sdk-52.7.0/docs/user/user/metrics/metrics-remote-settings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metrics/testing-metrics.md` & `glean-sdk-52.7.0/docs/user/user/metrics/testing-metrics.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/metrics/validation-checklist.md` & `glean-sdk-52.7.0/docs/user/user/metrics/validation-checklist.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/baseline.md` & `glean-sdk-52.7.0/docs/user/user/pings/baseline.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/custom.md` & `glean-sdk-52.7.0/docs/user/user/pings/custom.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/deletion-request.md` & `glean-sdk-52.7.0/docs/user/user/pings/deletion-request.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/events.md` & `glean-sdk-52.7.0/docs/user/user/pings/events.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/index.md` & `glean-sdk-52.7.0/docs/user/user/pings/index.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/metrics.md` & `glean-sdk-52.7.0/docs/user/user/pings/metrics.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/ping-schedules-and-timings.md` & `glean-sdk-52.7.0/docs/user/user/pings/ping-schedules-and-timings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/ping_timing.svg` & `glean-sdk-52.7.0/docs/user/user/pings/ping_timing.svg`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/sent-by-glean.md` & `glean-sdk-52.7.0/docs/user/user/pings/sent-by-glean.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/docs/user/user/pings/testing-custom-pings.md` & `glean-sdk-52.7.0/docs/user/user/pings/testing-custom-pings.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ARCHITECTURE.md` & `glean-sdk-52.7.0/glean-core/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/Cargo.toml` & `glean-sdk-52.7.0/glean-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "glean-core"
-version = "52.6.0"
+version = "52.7.0"
 authors = ["Jan-Erik Rediger <jrediger@mozilla.com>", "The Glean Team <glean-team@mozilla.com>"]
 description = "A modern Telemetry library"
 repository = "https://github.com/mozilla/glean"
 readme = "README.md"
 license = "MPL-2.0"
 edition = "2021"
 keywords = ["telemetry"]
```

### Comparing `glean-sdk-52.6.0/glean-core/LICENSE` & `glean-sdk-52.7.0/glean-core/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/README.md` & `glean-sdk-52.7.0/glean-core/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/build.gradle` & `glean-sdk-52.7.0/glean-core/android/build.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/dependency-licenses.xml` & `glean-sdk-52.7.0/glean-core/android/dependency-licenses.xml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/metrics.yaml` & `glean-sdk-52.7.0/glean-core/android/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/proguard-rules-consumer.pro` & `glean-sdk-52.7.0/glean-core/android/proguard-rules-consumer.pro`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/proguard-rules.pro` & `glean-sdk-52.7.0/glean-core/android/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/publish.gradle` & `glean-sdk-52.7.0/glean-core/android/publish.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Dispatchers.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Dispatchers.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Glean.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/Glean.kt`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,16 @@
                 applicationId = applicationContext.packageName,
                 languageBindingName = LANGUAGE_BINDING_NAME,
                 uploadEnabled = uploadEnabled,
                 maxEvents = null,
                 delayPingLifetimeIo = false,
                 appBuild = "none",
                 useCoreMps = false,
-                trimDataToRegisteredPings = false
+                trimDataToRegisteredPings = false,
+                logLevel = configuration.logLevel
             )
             val clientInfo = getClientInfo(configuration, buildInfo)
             val callbacks = OnGleanEventsImpl(this@GleanInternalAPI)
             gleanInitialize(cfg, clientInfo, callbacks)
         }
     }
 
@@ -417,15 +418,15 @@
      * If the tag is invalid it won't be set and this function will return `false`,
      * although if we are not initialized yet, there won't be any validation.
      *
      * This is only meant to be used internally by the `GleanDebugActivity`.
      *
      * @param value The value of the tag, which must be a valid HTTP header value.
      */
-    internal fun setDebugViewTag(value: String): Boolean {
+    fun setDebugViewTag(value: String): Boolean {
         return gleanSetDebugViewTag(value)
     }
 
     /**
      * Set the source tags to be applied as headers when uploading pings.
      *
      * If any of the tags is invalid nothing will be set and this function will
@@ -474,15 +475,15 @@
      * Set the logPing debug option, when this is `true`
      * the payload of assembled ping requests get logged.
      *
      * This is only meant to be used internally by the `GleanDebugActivity`.
      *
      * @param value The value of the option.
      */
-    internal fun setLogPings(value: Boolean) {
+    fun setLogPings(value: Boolean) {
         gleanSetLogPings(value)
     }
 
     /**
      * TEST ONLY FUNCTION.
      * This is called by the GleanTestRule, to enable test mode.
      *
```

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/Configuration.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/config/Configuration.kt`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 /* This Source Code Form is subject to the terms of the Mozilla Public
  * License, v. 2.0. If a copy of the MPL was not distributed with this
  * file, You can obtain one at http://mozilla.org/MPL/2.0/. */
 
 package mozilla.telemetry.glean.config
 
+import mozilla.telemetry.glean.internal.LevelFilter
 import mozilla.telemetry.glean.net.HttpURLConnectionUploader
 import mozilla.telemetry.glean.net.PingUploader
 
 /**
  * The Configuration class describes how to configure Glean.
  *
  * @property serverEndpoint the server pings are sent to. Please note that this is
  *           is only meant to be changed for tests.
  * @property maxEvents the number of events to store before the events ping is sent
  * @property httpClient The HTTP client implementation to use for uploading pings.
  * @property channel the release channel the application is on, if known. This will be
  *           sent along with all the pings, in the `client_info` section.
  * @property dataPath An optional [String] that specifies where to store data locally on the device.
  *           This should ONLY be used when setting up Glean on a non-main process.
+ * @property logLevel An optional [LevelFilter] that controls how verbose the internal logging is.
  */
 data class Configuration @JvmOverloads constructor(
     val serverEndpoint: String = DEFAULT_TELEMETRY_ENDPOINT,
     val channel: String? = null,
     val maxEvents: Int? = null,
     // NOTE: since only simple object or strings can be made `const val`s, if the
     // default values for the lines below are ever changed, they are required
     // to change in the public constructor below.
     val httpClient: PingUploader = HttpURLConnectionUploader(),
-    val dataPath: String? = null
+    val dataPath: String? = null,
+    val logLevel: LevelFilter? = null
 ) {
     companion object {
         /**
          * The default server pings are sent to.
          */
         const val DEFAULT_TELEMETRY_ENDPOINT = "https://incoming.telemetry.mozilla.org"
     }
```

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/GleanDebugActivity.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/debug/GleanDebugActivity.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/BaseUploader.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/BaseUploader.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/HttpURLConnectionUploader.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/HttpURLConnectionUploader.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/PingUploader.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/PingUploader.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/Upload.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/net/Upload.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/Aliases.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/Aliases.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/BooleanMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/BooleanMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CounterMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CounterMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CustomDistributionMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/CustomDistributionMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DatetimeMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DatetimeMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DenominatorMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/DenominatorMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/EventMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/EventMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/HistogramBase.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/HistogramBase.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/LabeledMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/LabeledMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/MemoryDistributionMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/MemoryDistributionMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/NumeratorMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/NumeratorMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/PingType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/PingType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/QuantityMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/QuantityMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/RateMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/RateMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringListMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringListMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/StringMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TextMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TextMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimespanMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimespanMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimingDistributionMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/TimingDistributionMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UrlMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UrlMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UuidMetricType.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/private/UuidMetricType.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/GleanLifecycleObserver.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/GleanLifecycleObserver.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/MetricsPingScheduler.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/MetricsPingScheduler.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/PingUploadWorker.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/scheduler/PingUploadWorker.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestLocalServer.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestLocalServer.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestRule.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/testing/GleanTestRule.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DataPathUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DataPathUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DateUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/DateUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/GzipUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/GzipUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/JsonUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/JsonUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/LocaleUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/LocaleUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/ThreadUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/ThreadUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/WorkManagerUtils.kt` & `glean-sdk-52.7.0/glean-core/android/src/main/java/mozilla/telemetry/glean/utils/WorkManagerUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/android/util/Log.java` & `glean-sdk-52.7.0/glean-core/android/src/test/java/android/util/Log.java`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanFromJavaTest.java` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanFromJavaTest.java`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/GleanTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/TestUtil.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/TestUtil.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/GleanDebugActivityTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/debug/GleanDebugActivityTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/BaseUploaderTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/BaseUploaderTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/HttpURLConnectionUploaderTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/net/HttpURLConnectionUploaderTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/CustomPingTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/CustomPingTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/DeletionPingTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/pings/DeletionPingTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/AccumulationsBeforeGleanInitTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/AccumulationsBeforeGleanInitTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/BooleanMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/BooleanMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CounterMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CounterMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CustomDistributionMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/CustomDistributionMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/DatetimeMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/DatetimeMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/EventMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/EventMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/LabeledMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/LabeledMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/MemoryDistributionMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/MemoryDistributionMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/PingTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/PingTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/QuantityMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/QuantityMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/RateMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/RateMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringListMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringListMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/StringMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimespanMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimespanMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimingDistributionMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/TimingDistributionMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UrlMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UrlMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UuidMetricTypeTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/private/UuidMetricTypeTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/MetricsPingSchedulerTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/MetricsPingSchedulerTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/PingUploadWorkerTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/scheduler/PingUploadWorkerTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/ShadowLog.java` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/shadows/ShadowLog.java`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DataPathUtilsTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DataPathUtilsTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DateUtilsTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/DateUtilsTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/GzipUtilsTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/GzipUtilsTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/JsonUtilsTest.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/JsonUtilsTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/KArgumentCaptor.kt` & `glean-sdk-52.7.0/glean-core/android/src/test/java/mozilla/telemetry/glean/utils/KArgumentCaptor.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android-native/build.gradle` & `glean-sdk-52.7.0/glean-core/android-native/build.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android-native/dependency-licenses.xml` & `glean-sdk-52.7.0/glean-core/android-native/dependency-licenses.xml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android-native/proguard-rules.pro` & `glean-sdk-52.7.0/glean-core/android-native/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/android-native/publish.gradle` & `glean-sdk-52.7.0/glean-core/android-native/publish.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/build/LICENSE` & `glean-sdk-52.7.0/glean-core/build/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/build/README.md` & `glean-sdk-52.7.0/glean-core/build/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/build/src/lib.rs` & `glean-sdk-52.7.0/glean-core/build/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/bundle/Cargo.toml` & `glean-sdk-52.7.0/glean-core/bundle/Cargo.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/bundle/src/lib.rs` & `glean-sdk-52.7.0/glean-core/bundle/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/bundle-android/Cargo.toml` & `glean-sdk-52.7.0/glean-core/bundle-android/Cargo.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Config/Configuration.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Config/Configuration.swift`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,37 @@
 /// The Configuration struct describes how to configure Glean as well as providing convenience
 /// property for calculating the `FfiConfiguration`
 public struct Configuration {
     let serverEndpoint: String
     let maxEvents: Int32?
     let channel: String?
     let dataPath: String?
+    let logLevel: LevelFilter?
 
     struct Constants {
         static let defaultTelemetryEndpoint = "https://incoming.telemetry.mozilla.org"
     }
 
     /// Create a new Glean `Configuration` object
     ///
     /// - parameters:
     ///   * maxEvents the number of events to store before the events ping is sent.
     ///   * channel the release channel the application is on, if known.
     ///   This will be sent along with all the pings, in the `client_info` section.
     ///   * serverEndpoint the server endpoint Glean should send data to
     ///   * dataPath an optional String that specifies where to store data locally on the device.
     ///   This should ONLY be used when setting up Glean on a non-main process.
+    ///   * logLevel an optional log level that controls how verbose the internal logging is.
     public init(
         maxEvents: Int32? = nil,
         channel: String? = nil,
         serverEndpoint: String? = nil,
-        dataPath: String? = nil
+        dataPath: String? = nil,
+        logLevel: LevelFilter? = nil
     ) {
         self.serverEndpoint = serverEndpoint ?? Constants.defaultTelemetryEndpoint
         self.maxEvents = maxEvents
         self.channel = channel
         self.dataPath = dataPath
+        self.logLevel = logLevel
     }
 }
```

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Debug/GleanDebugTools.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Debug/GleanDebugTools.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Dispatchers.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Dispatchers.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Glean.h` & `glean-sdk-52.7.0/glean-core/ios/Glean/Glean.h`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Glean.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Glean.swift`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,16 @@
             applicationId: AppInfo.name,
             languageBindingName: Constants.languageBindingName,
             uploadEnabled: uploadEnabled,
             maxEvents: configuration.maxEvents.map { UInt32($0) },
             delayPingLifetimeIo: false,
             appBuild: "0.0.0",
             useCoreMps: false,
-            trimDataToRegisteredPings: false
+            trimDataToRegisteredPings: false,
+            logLevel: configuration.logLevel
         )
         let clientInfo = getClientInfo(configuration, buildInfo: buildInfo)
         let callbacks = OnGleanEventsImpl(glean: self)
         gleanInitialize(cfg, clientInfo, callbacks)
     }
 
     /// Initialize the core metrics internally managed by Glean (e.g. client id).
```

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/GleanMetrics.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/GleanMetrics.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Info.plist` & `glean-sdk-52.7.0/glean-core/ios/Glean/Info.plist`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/BooleanMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/BooleanMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/CounterMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/CounterMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/DatetimeMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/DatetimeMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/EventMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/EventMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/LabeledMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/LabeledMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/MemoryDistributionMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/MemoryDistributionMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/Ping.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/Ping.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/QuantityMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/QuantityMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/RateMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/RateMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/StringListMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/StringListMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/StringMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/StringMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TextMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TextMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TimespanMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TimespanMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/TimingDistributionMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/TimingDistributionMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/UrlMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/UrlMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Metrics/UuidMetric.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Metrics/UuidMetric.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Net/HttpPingUploader.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Net/HttpPingUploader.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Scheduler/GleanLifecycleObserver.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Scheduler/GleanLifecycleObserver.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Scheduler/MetricsPingScheduler.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Scheduler/MetricsPingScheduler.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Logger.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Logger.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Sysctl.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Sysctl.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Unreachable.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Unreachable.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean/Utils/Utils.swift` & `glean-sdk-52.7.0/glean-core/ios/Glean/Utils/Utils.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.pbxproj` & `glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved` & `glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/Glean.xcscheme` & `glean-sdk-52.7.0/glean-core/ios/Glean.xcodeproj/xcshareddata/xcschemes/Glean.xcscheme`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Config/ConfigurationTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Config/ConfigurationTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Debug/GleanDebugUtilityTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Debug/GleanDebugUtilityTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/GleanTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/GleanTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Info.plist` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Info.plist`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/BooleanMetricTypeTest.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/BooleanMetricTypeTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/CounterMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/CounterMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/DatetimeMetricTypeTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/DatetimeMetricTypeTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/EventMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/EventMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/LabeledMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/LabeledMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/MemoryDistributionMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/MemoryDistributionMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/PingTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/PingTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/QuantityMetricTypeTest.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/QuantityMetricTypeTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/RateMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/RateMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/StringListMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/StringListMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/StringMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/StringMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/TimespanMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/TimespanMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/TimingDistributionMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/TimingDistributionMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/UrlMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/UrlMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Metrics/UuidMetricTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Metrics/UuidMetricTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/BaselinePingTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/BaselinePingTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/DeletionRequestPingTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/DeletionRequestPingTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Net/HttpPingUploaderTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Net/HttpPingUploaderTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Scheduler/MetricsPingSchedulerTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Scheduler/MetricsPingSchedulerTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/TestUtils.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/TestUtils.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/GleanTests/Utils/DataPathUtilsTests.swift` & `glean-sdk-52.7.0/glean-core/ios/GleanTests/Utils/DataPathUtilsTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/ios/sdk_generator.sh` & `glean-sdk-52.7.0/glean-core/ios/sdk_generator.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/metrics.yaml` & `glean-sdk-52.7.0/glean-core/metrics.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -740,14 +740,31 @@
     data_sensitivity:
       - technical
     notification_emails:
       - glean-team@mozilla.com
       - jrediger@mozilla.com
     expires: never
 
+  shutdown_dispatcher_wait:
+    type: timing_distribution
+    time_unit: millisecond
+    description: |
+      Time waited for the dispatcher to unblock during shutdown.
+      Most samples are expected to be below the 10s timeout used.
+    bugs:
+      - https://bugzilla.mozilla.org/show_bug.cgi?id=1828066
+    data_reviews:
+      - https://bugzilla.mozilla.org/show_bug.cgi?id=1828066#c7
+    data_sensitivity:
+      - technical
+    notification_emails:
+      - glean-team@mozilla.com
+      - jrediger@mozilla.com
+    expires: never
+
 glean:
   restarted:
     type: event
     description: |
       Recorded when the Glean SDK is restarted.
 
       Only included in custom pings that record events.
```

### Comparing `glean-sdk-52.6.0/glean-core/pings.yaml` & `glean-sdk-52.7.0/glean-core/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/__init__.py` & `glean-sdk-52.7.0/glean-core/python/glean/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_builtins.py` & `glean-sdk-52.7.0/glean-core/python/glean/_builtins.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_ffi.py` & `glean-sdk-52.7.0/glean-core/python/glean/_ffi.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_loader.py` & `glean-sdk-52.7.0/glean-core/python/glean/_loader.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_process_dispatcher.py` & `glean-sdk-52.7.0/glean-core/python/glean/_process_dispatcher.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py` & `glean-sdk-52.7.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/_util.py` & `glean-sdk-52.7.0/glean-core/python/glean/_util.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/config.py` & `glean-sdk-52.7.0/glean-core/python/glean/config.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/glean.py` & `glean-sdk-52.7.0/glean-core/python/glean/glean.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
             language_binding_name="Python",
             upload_enabled=upload_enabled,
             max_events=configuration.max_events,
             delay_ping_lifetime_io=False,
             use_core_mps=False,
             app_build=cls._application_build_id,
             trim_data_to_registered_pings=False,
+            log_level=None,
         )
 
         _uniffi.glean_initialize(cfg, client_info, callbacks)
         cls._initialized = True
 
     @classmethod
     def _initialize_with_tempdir_for_testing(
```

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/__init__.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/datetime.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/datetime.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/event.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/event.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/labeled.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/labeled.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/ping.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/ping.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/string.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/string.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/timespan.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/timespan.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/timing_distribution.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/timing_distribution.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/url.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/url.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/metrics/uuid.py` & `glean-sdk-52.7.0/glean-core/python/glean/metrics/uuid.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/net/__init__.py` & `glean-sdk-52.7.0/glean-core/python/glean/net/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/net/base_uploader.py` & `glean-sdk-52.7.0/glean-core/python/glean/net/base_uploader.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/net/http_client.py` & `glean-sdk-52.7.0/glean-core/python/glean/net/http_client.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/net/ping_upload_worker.py` & `glean-sdk-52.7.0/glean-core/python/glean/net/ping_upload_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             # or sending a deletion-request ping.
             upload_enabled=False,
             max_events=configuration.max_events,
             delay_ping_lifetime_io=False,
             use_core_mps=False,
             app_build="",
             trim_data_to_registered_pings=False,
+            log_level=None,
         )
         if not glean_initialize_for_subprocess(cfg):
             log.error("Couldn't initialize Glean in subprocess")
             sys.exit(1)
 
     # Limits are enforced by glean-core to avoid an inifinite loop here.
     # Whenever a limit is reached, this binding will receive `UploadTaskTag.DONE` and step out.
```

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/net/ping_uploader.py` & `glean-sdk-52.7.0/glean-core/python/glean/net/ping_uploader.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/glean/testing/__init__.py` & `glean-sdk-52.7.0/glean-core/python/glean/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/setup.py` & `glean-sdk-52.7.0/glean-core/python/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 with (SRC_ROOT / "README.md").open() as readme_file:
     readme = readme_file.read()
 
 with (SRC_ROOT / "CHANGELOG.md").open() as history_file:
     history = history_file.read()
 
 # glean version. Automatically updated by the bin/prepare_release.sh script
-version = "52.6.0"
+version = "52.7.0"
 
 requirements = [
     "semver>=2.13.0",
     "glean_parser~=7.1",
 ]
 
 # The environment variable `GLEAN_BUILD_VARIANT` can be set to `debug` or `release`
```

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/conftest.py` & `glean-sdk-52.7.0/glean-core/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/data/core.yaml` & `glean-sdk-52.7.0/glean-core/python/tests/data/core.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/data/events_with_types.yaml` & `glean-sdk-52.7.0/glean-core/python/tests/data/events_with_types.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/data/glinter.yaml` & `glean-sdk-52.7.0/glean-core/python/tests/data/glinter.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/data/pings.yaml` & `glean-sdk-52.7.0/glean-core/python/tests/data/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_boolean.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_boolean.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_counter.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_counter.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_datetime.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_datetime.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_event.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_event.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_labeled.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_labeled.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_memory_distribution.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_memory_distribution.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_quantity.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_quantity.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_string.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_string.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_string_list.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_string_list.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_timespan.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_timespan.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_timing_distribution.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_timing_distribution.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_url.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_url.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/metrics/test_uuid.py` & `glean-sdk-52.7.0/glean-core/python/tests/metrics/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/test_glean.py` & `glean-sdk-52.7.0/glean-core/python/tests/test_glean.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/test_loader.py` & `glean-sdk-52.7.0/glean-core/python/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/python/tests/test_network.py` & `glean-sdk-52.7.0/glean-core/python/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/Cargo.toml` & `glean-sdk-52.7.0/glean-core/rlb/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "glean"
-version = "52.6.0"
+version = "52.7.0"
 authors = ["Jan-Erik Rediger <jrediger@mozilla.com>", "The Glean Team <glean-team@mozilla.com>"]
 description = "Glean SDK Rust language bindings"
 repository = "https://github.com/mozilla/glean"
 readme = "README.md"
 license = "MPL-2.0"
 edition = "2021"
 keywords = ["telemetry", "glean"]
@@ -19,15 +19,15 @@
 
 [badges]
 circle-ci = { repository = "mozilla/glean", branch = "main" }
 maintenance = { status = "actively-developed" }
 
 [dependencies.glean-core]
 path = ".."
-version = "52.6.0"
+version = "52.7.0"
 
 [dependencies]
 crossbeam-channel = "0.5"
 inherent = "1"
 log = "0.4.8"
 once_cell = "1.2.0"
 thiserror = "1.0.4"
```

### Comparing `glean-sdk-52.6.0/glean-core/rlb/LICENSE` & `glean-sdk-52.7.0/glean-core/rlb/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/README.md` & `glean-sdk-52.7.0/glean-core/rlb/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/examples/long-running.rs` & `glean-sdk-52.7.0/glean-core/rlb/examples/long-running.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/examples/prototype.rs` & `glean-sdk-52.7.0/glean-core/rlb/examples/prototype.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/common_test.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/common_test.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/configuration.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/configuration.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
+use log::LevelFilter;
+
 use crate::net::PingUploader;
 
 use std::path::PathBuf;
 
 /// The default server pings are sent to.
 pub(crate) const DEFAULT_GLEAN_ENDPOINT: &str = "https://incoming.telemetry.mozilla.org";
 
@@ -30,14 +32,16 @@
     pub uploader: Option<Box<dyn PingUploader + 'static>>,
     /// Whether Glean should schedule "metrics" pings for you.
     pub use_core_mps: bool,
     /// Whether Glean should limit its storage to only that of registered pings.
     /// Unless you know that all your and your libraries' pings are appropriately registered
     /// _before_ init, you shouldn't use this.
     pub trim_data_to_registered_pings: bool,
+    /// The internal logging level.
+    pub log_level: Option<LevelFilter>,
 }
 
 /// Configuration builder.
 ///
 /// Let's you build a configuration from the required fields
 /// and let you set optional fields individually.
 #[derive(Debug)]
@@ -64,14 +68,17 @@
     /// Default: `false`
     pub use_core_mps: bool,
     /// Optional: Whether Glean should limit its storage to only that of registered pings.
     /// Unless you know that all your and your libraries' pings are appropriately registered
     /// _before_ init, you shouldn't use this.
     /// Default: `false`
     pub trim_data_to_registered_pings: bool,
+    /// Optional: The internal logging level.
+    /// Default: `None`
+    pub log_level: Option<LevelFilter>,
 }
 
 impl Builder {
     /// A new configuration builder.
     pub fn new<P: Into<PathBuf>, S: Into<String>>(
         upload_enabled: bool,
         data_path: P,
@@ -83,14 +90,15 @@
             application_id: application_id.into(),
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: None,
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         }
     }
 
     /// Generate the full configuration.
     pub fn build(self) -> Configuration {
         Configuration {
             upload_enabled: self.upload_enabled,
@@ -98,14 +106,15 @@
             application_id: self.application_id,
             max_events: self.max_events,
             delay_ping_lifetime_io: self.delay_ping_lifetime_io,
             server_endpoint: self.server_endpoint,
             uploader: self.uploader,
             use_core_mps: self.use_core_mps,
             trim_data_to_registered_pings: self.trim_data_to_registered_pings,
+            log_level: self.log_level,
         }
     }
 
     /// Set the maximum number of events to store before sending a ping containing events.
     pub fn with_max_events(mut self, max_events: usize) -> Self {
         self.max_events = Some(max_events);
         self
```

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/core_metrics.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/core_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/lib.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         application_id: cfg.application_id.clone(),
         language_binding_name: LANGUAGE_BINDING_NAME.into(),
         max_events: cfg.max_events.map(|m| m as u32),
         delay_ping_lifetime_io: cfg.delay_ping_lifetime_io,
         app_build: client_info.app_build.clone(),
         use_core_mps: cfg.use_core_mps,
         trim_data_to_registered_pings: cfg.trim_data_to_registered_pings,
+        log_level: cfg.log_level,
     };
 
     glean_core::glean_initialize(core_cfg, client_info.into(), callbacks);
     Some(())
 }
 
 /// Shuts down Glean in an orderly fashion.
```

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/net/http_uploader.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/net/http_uploader.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/net/mod.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/net/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/private/event.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/private/event.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/private/mod.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/private/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/private/ping.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/private/ping.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/system.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/system.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/src/test.rs` & `glean-sdk-52.7.0/glean-core/rlb/src/test.rs`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Define a new ping and submit it.
     const PING_NAME: &str = "test-ping";
     let custom_ping = private::PingType::new(PING_NAME, true, true, vec![]);
@@ -138,14 +139,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     assert!(test_is_experiment_active(
         "experiment_set_preinit".to_string()
@@ -198,14 +200,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Simulate becoming active.
     handle_client_active();
 
@@ -280,14 +283,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     // Wait for the ping to arrive.
     let url = r.recv().unwrap();
@@ -339,14 +343,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     // We don't expect a startup ping.
     assert_eq!(r.try_recv(), Err(crossbeam_channel::TryRecvError::Empty));
@@ -369,14 +374,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: None,
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     test_reset_glean(cfg, ClientInfoMetrics::unknown(), false);
 
     // We don't need to sleep here.
     // The `test_reset_glean` already waited on the initialize task.
 }
@@ -415,14 +421,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: None,
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
     let _t = new_glean(Some(cfg), false);
 
     // Verify that the callback was executed by testing for the correct value
     assert!(metric.test_get_value(None).is_some(), "Value must exist");
     assert_eq!(3, metric.test_get_value(None).unwrap(), "Value must match");
 }
@@ -441,14 +448,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         true,
     );
 
     // Glean was initialized and it waited for a full initialization to finish.
     // We now just want to try to initialize again.
@@ -461,14 +469,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
     );
 
     // We don't need to sleep here.
     // The `test_reset_glean` already waited on the initialize task,
     // and the 2nd initialize will bail out early.
@@ -489,14 +498,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         true,
     );
 
     // Ensure there's at least one event recorded,
     // otherwise the ping is not sent.
@@ -553,14 +563,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         client_info,
         true,
     );
     assert!(app_channel.test_get_value(None).is_none());
 
     // Custom app_channel reported.
@@ -575,14 +586,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         client_info,
         true,
     );
     assert_eq!("testing", app_channel.test_get_value(None).unwrap());
 }
 
@@ -638,14 +650,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         true,
     );
 
     let ping_name = "custom_ping_1";
     let ping = private::PingType::new(ping_name, true, false, vec![]);
@@ -719,14 +732,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         true,
     );
 
     // Internal metric, replicated here for testing.
     let os_version = StringMetric::new(CommonMetricData {
@@ -781,14 +795,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: None,
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Now reset Glean and disable upload: it should still send a deletion request
     // ping even though we're just starting.
     test_reset_glean(
@@ -798,14 +813,15 @@
             upload_enabled: false,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     // Wait for the ping to arrive.
     let url = r.recv().unwrap();
@@ -846,14 +862,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: None,
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Now reset Glean and keep upload enabled: no deletion-request
     // should be sent.
     test_reset_glean(
@@ -863,14 +880,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     assert_eq!(0, r.len());
 }
@@ -919,14 +937,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: None,
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         true,
     );
 
     // Reaching into the core.
     glean_core::glean_set_dirty_flag(true);
@@ -951,14 +970,15 @@
             upload_enabled: true,
             max_events: None,
             delay_ping_lifetime_io: false,
             server_endpoint: Some("invalid-test-host".into()),
             uploader: Some(Box::new(FakeUploader { sender: s })),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         },
         ClientInfoMetrics::unknown(),
         false,
     );
 
     let (url, body) = r.recv().unwrap();
     assert!(url.contains("/baseline/"));
@@ -1009,14 +1029,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Submit a baseline ping.
     submit_ping_by_name("baseline", Some("inactive"));
 
@@ -1067,14 +1088,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Submit a baseline ping.
     submit_ping_by_name("baseline", Some("inactive"));
 
@@ -1124,14 +1146,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Attempt to set source tags after `Glean.initialize` is called,
     // but before Glean is fully initialized.
     //assert!(was_initialize_called());
@@ -1195,14 +1218,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     // We create a ping and a metric before we initialize Glean
     let sample_ping = PingType::new("sample-ping-1", true, false, vec![]);
     let metric = private::StringMetric::new(CommonMetricData {
         name: "string_metric".into(),
         category: "telemetry".into(),
@@ -1263,14 +1287,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Submit a baseline ping.
     sample_ping.submit(None);
 
@@ -1313,14 +1338,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader { sender: s })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Create a custom ping and register it.
     let sample_ping = PingType::new("custom1", true, true, vec![]);
 
@@ -1441,14 +1467,15 @@
         server_endpoint: Some("invalid-test-host".into()),
         uploader: Some(Box::new(FakeUploader {
             barrier: Arc::clone(&barrier),
             counter: Arc::clone(&call_count),
         })),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let _t = new_glean(Some(cfg), true);
 
     // Define a new ping and submit it.
     const PING_NAME: &str = "test-ping";
     let custom_ping = private::PingType::new(PING_NAME, true, true, vec![]);
```

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/common/mod.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/init_fails.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/init_fails.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/never_init.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/never_init.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/no_time_to_init.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/no_time_to_init.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/overflowing_preinit.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/overflowing_preinit.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/persist_ping_lifetime.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/persist_ping_lifetime.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/persist_ping_lifetime_nopanic.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/persist_ping_lifetime_nopanic.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/schema.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/schema.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/simple.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/simple.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/test-shutdown-blocking.sh` & `glean-sdk-52.7.0/glean-core/rlb/tests/test-shutdown-blocking.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/rlb/tests/upload_timing.rs` & `glean-sdk-52.7.0/glean-core/rlb/tests/upload_timing.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/common_metric_data.rs` & `glean-sdk-52.7.0/glean-core/src/common_metric_data.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/core/mod.rs` & `glean-sdk-52.7.0/glean-core/src/core/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 ///     language_binding_name: "Rust".into(),
 ///     upload_enabled: true,
 ///     max_events: None,
 ///     delay_ping_lifetime_io: false,
 ///     app_build: "".into(),
 ///     use_core_mps: false,
 ///     trim_data_to_registered_pings: false,
+///     log_level: None,
 /// };
 /// let mut glean = Glean::new(cfg).unwrap();
 /// let ping = PingType::new("sample", true, false, vec![]);
 /// glean.register_ping_type(&ping);
 ///
 /// let call_counter: CounterMetric = CounterMetric::new(CommonMetricData {
 ///     name: "calls".into(),
@@ -289,14 +290,15 @@
             language_binding_name: "Rust".into(),
             upload_enabled,
             max_events: None,
             delay_ping_lifetime_io: false,
             app_build: "Unknown".into(),
             use_core_mps: false,
             trim_data_to_registered_pings: false,
+            log_level: None,
         };
 
         let mut glean = Self::new(cfg).unwrap();
 
         // Disable all upload manager policies for testing
         glean.upload_manager = PingUploadManager::no_policy(data_path);
```

### Comparing `glean-sdk-52.6.0/glean-core/src/core_metrics.rs` & `glean-sdk-52.7.0/glean-core/src/core_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/coverage.rs` & `glean-sdk-52.7.0/glean-core/src/coverage.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/database/mod.rs` & `glean-sdk-52.7.0/glean-core/src/database/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/debug.rs` & `glean-sdk-52.7.0/glean-core/src/debug.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/dispatcher/global.rs` & `glean-sdk-52.7.0/glean-core/src/dispatcher/global.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 use once_cell::sync::Lazy;
 use std::sync::atomic::{AtomicBool, Ordering};
 use std::sync::RwLock;
 use std::thread;
+use std::time::Duration;
 
 use super::{DispatchError, DispatchGuard, Dispatcher};
+use crossbeam_channel::RecvTimeoutError;
 
 #[cfg(feature = "preinit_million_queue")]
 pub const GLOBAL_DISPATCHER_LIMIT: usize = 1000000;
 #[cfg(not(feature = "preinit_million_queue"))]
 pub const GLOBAL_DISPATCHER_LIMIT: usize = 1000;
 
 static GLOBAL_DISPATCHER: Lazy<RwLock<Option<Dispatcher>>> =
@@ -72,14 +74,19 @@
 }
 
 /// Block until all tasks prior to this call are processed.
 pub fn block_on_queue() {
     guard().block_on_queue();
 }
 
+/// Block until all tasks prior to this call are processed, with a timeout.
+pub fn block_on_queue_timeout(timeout: Duration) -> Result<(), RecvTimeoutError> {
+    guard().block_on_queue_timeout(timeout)
+}
+
 /// Starts processing queued tasks in the global dispatch queue.
 ///
 /// This function blocks until queued tasks prior to this call are finished.
 /// Once the initial queue is empty the dispatcher will wait for new tasks to be launched.
 ///
 /// # Returns
 ///
```

### Comparing `glean-sdk-52.6.0/glean-core/src/dispatcher/mod.rs` & `glean-sdk-52.7.0/glean-core/src/dispatcher/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 use std::{
     mem,
     sync::{
         atomic::{AtomicBool, AtomicUsize, Ordering},
         Arc,
     },
     thread::{self, JoinHandle},
+    time::Duration,
 };
 
-use crossbeam_channel::{bounded, unbounded, SendError, Sender};
+use crossbeam_channel::{bounded, unbounded, RecvTimeoutError, SendError, Sender};
 use thiserror::Error;
 
 pub use global::*;
 
 pub(crate) mod global;
 
 /// Command received while blocked from further work.
@@ -157,14 +158,34 @@
             .send(task)
             .expect("Failed to launch the blocking task");
 
         rx.recv()
             .expect("Failed to receive message on single-use channel");
     }
 
+    /// Block on the task queue emptying, with a timeout.
+    fn block_on_queue_timeout(&self, timeout: Duration) -> Result<(), RecvTimeoutError> {
+        let (tx, rx) = crossbeam_channel::bounded(0);
+
+        // We explicitly don't use `self.launch` here.
+        // We always put this task on the unbounded queue.
+        // The pre-init queue might be full before its flushed, in which case this would panic.
+        // Blocking on the queue can only work if it is eventually flushed anyway.
+
+        let task = Command::Task(Box::new(move || {
+            tx.send(())
+                .expect("(worker) Can't send message on single-use channel");
+        }));
+        self.sender
+            .send(task)
+            .expect("Failed to launch the blocking task");
+
+        rx.recv_timeout(timeout)
+    }
+
     fn kill(&mut self) -> Result<(), DispatchError> {
         // We immediately stop queueing in the pre-init buffer.
         let old_val = self.queue_preinit.swap(false, Ordering::SeqCst);
         if !old_val {
             return Err(DispatchError::AlreadyFlushed);
         }
```

### Comparing `glean-sdk-52.6.0/glean-core/src/error.rs` & `glean-sdk-52.7.0/glean-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/error_recording.rs` & `glean-sdk-52.7.0/glean-core/src/error_recording.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/event_database/mod.rs` & `glean-sdk-52.7.0/glean-core/src/event_database/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                     }
                     continue;
                 }
                 let file = BufReader::new(File::open(entry.path())?);
                 db.insert(
                     store_name,
                     file.lines()
-                        .filter_map(|line| line.ok())
+                        .map_while(Result::ok)
                         .filter_map(|line| serde_json::from_str::<StoredEvent>(&line).ok())
                         .collect(),
                 );
             }
         }
         Ok(())
     }
```

### Comparing `glean-sdk-52.6.0/glean-core/src/fd_logger.rs` & `glean-sdk-52.7.0/glean-core/src/fd_logger.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/glean.udl` & `glean-sdk-52.7.0/glean-core/src/glean.udl`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,25 @@
     string language_binding_name;
     boolean upload_enabled;
     u32? max_events;
     boolean delay_ping_lifetime_io;
     string app_build;
     boolean use_core_mps;
     boolean trim_data_to_registered_pings;
+    LevelFilter? log_level;
+};
+
+// An enum representing the different logging levels for the `log` crate.
+enum LevelFilter {
+    "Off",
+    "Error",
+    "Warn",
+    "Info",
+    "Debug",
+    "Trace",
 };
 
 // Values for the `client_info` metrics.
 // The language SDK should collect them on `initialize` once.
 // They will be re-used, e.g. when upload is toggled from off to on, to re-set them.
 //
 // See https://mozilla.github.io/glean/book/user/pings/index.html#the-client_info-section for details.
```

### Comparing `glean-sdk-52.6.0/glean-core/src/glean_metrics.rs` & `glean-sdk-52.7.0/glean-core/src/glean_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/histogram/exponential.rs` & `glean-sdk-52.7.0/glean-core/src/histogram/exponential.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/histogram/functional.rs` & `glean-sdk-52.7.0/glean-core/src/histogram/functional.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/histogram/linear.rs` & `glean-sdk-52.7.0/glean-core/src/histogram/linear.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/histogram/mod.rs` & `glean-sdk-52.7.0/glean-core/src/histogram/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/internal_metrics.rs` & `glean-sdk-52.7.0/glean-core/src/internal_metrics.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     pub io_errors: CounterMetric,
 
     /// A count of the pings submitted, by ping type.
     pub pings_submitted: LabeledMetric<CounterMetric>,
 
     /// Time waited for the uploader at shutdown.
     pub shutdown_wait: TimingDistributionMetric,
+
+    /// Time waited for the dispatcher to unblock during shutdown.
+    pub shutdown_dispatcher_wait: TimingDistributionMetric,
 }
 
 impl CoreMetrics {
     pub fn new() -> CoreMetrics {
         CoreMetrics {
             client_id: UuidMetric::new(CommonMetricData {
                 name: "client_id".into(),
@@ -92,14 +95,26 @@
                     category: "glean.validation".into(),
                     send_in_pings: vec!["metrics".into()],
                     lifetime: Lifetime::Ping,
                     disabled: false,
                     dynamic_label: None,
                 },
                 TimeUnit::Millisecond,
+            ),
+
+            shutdown_dispatcher_wait: TimingDistributionMetric::new(
+                CommonMetricData {
+                    name: "shutdown_dispatcher_wait".into(),
+                    category: "glean.validation".into(),
+                    send_in_pings: vec!["metrics".into()],
+                    lifetime: Lifetime::Ping,
+                    disabled: false,
+                    dynamic_label: None,
+                },
+                TimeUnit::Millisecond,
             ),
         }
     }
 }
 
 #[derive(Debug)]
 pub struct UploadMetrics {
```

### Comparing `glean-sdk-52.6.0/glean-core/src/internal_pings.rs` & `glean-sdk-52.7.0/glean-core/src/internal_pings.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/lib.rs` & `glean-sdk-52.7.0/glean-core/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 use std::fmt;
 use std::sync::atomic::{AtomicBool, Ordering};
 use std::sync::{Arc, Mutex};
 use std::thread;
 use std::time::Duration;
 
 use crossbeam_channel::unbounded;
+use log::{self, LevelFilter};
 use once_cell::sync::{Lazy, OnceCell};
 use uuid::Uuid;
 
 use metrics::MetricsEnabledConfig;
 
 mod common_metric_data;
 mod core;
@@ -121,14 +122,16 @@
     /// The application's build identifier. If this is different from the one provided for a previous init,
     /// and use_core_mps is `true`, we will trigger a "metrics" ping.
     pub app_build: String,
     /// Whether Glean should schedule "metrics" pings.
     pub use_core_mps: bool,
     /// Whether Glean should, on init, trim its event storage to only the registered pings.
     pub trim_data_to_registered_pings: bool,
+    /// The internal logging level.
+    pub log_level: Option<LevelFilter>,
 }
 
 /// Launches a new task on the global dispatch queue with a reference to the Glean singleton.
 fn launch_with_glean(callback: impl FnOnce(&Glean) + Send + 'static) {
     dispatcher::launch(|| core::with_glean(callback));
 }
 
@@ -302,14 +305,19 @@
 
     let init_handle = std::thread::Builder::new()
         .name("glean.init".into())
         .spawn(move || {
             let upload_enabled = cfg.upload_enabled;
             let trim_data_to_registered_pings = cfg.trim_data_to_registered_pings;
 
+            // Set the internal logging level.
+            if let Some(level) = cfg.log_level {
+                log::set_max_level(level)
+            }
+
             let glean = match Glean::new(cfg) {
                 Ok(glean) => glean,
                 Err(err) => {
                     log::error!("Failed to initialize Glean: {}", err);
                     return;
                 }
             };
@@ -553,16 +561,39 @@
     }
 
     crate::launch_with_glean_mut(|glean| {
         glean.cancel_metrics_ping_scheduler();
         glean.set_dirty_flag(false);
     });
 
-    // We need to wait for above task to finish.
-    dispatcher::block_on_queue();
+    // We need to wait for above task to finish,
+    // but we also don't wait around forever.
+    //
+    // TODO: Make the timeout configurable?
+    // The default hang watchdog on Firefox waits 60s,
+    // Glean's `uploader_shutdown` further below waits up to 30s.
+    let timer_id = core::with_glean(|glean| {
+        glean
+            .additional_metrics
+            .shutdown_dispatcher_wait
+            .start_sync()
+    });
+    if dispatcher::block_on_queue_timeout(Duration::from_secs(10)).is_err() {
+        log::error!(
+            "Timeout while blocking on the dispatcher. No further shutdown cleanup will happen."
+        );
+        return;
+    }
+    let stop_time = time::precise_time_ns();
+    core::with_glean(|glean| {
+        glean
+            .additional_metrics
+            .shutdown_dispatcher_wait
+            .set_stop_and_accumulate(glean, timer_id, stop_time);
+    });
 
     if let Err(e) = dispatcher::shutdown() {
         log::error!("Can't shutdown dispatcher thread: {:?}", e);
     }
 
     uploader_shutdown();
```

### Comparing `glean-sdk-52.6.0/glean-core/src/lib_unit_tests.rs` & `glean-sdk-52.7.0/glean-core/src/lib_unit_tests.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/boolean.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/counter.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/counter.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/custom_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/datetime.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/denominator.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/denominator.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/event.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/event.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/experiment.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/experiment.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/labeled.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/memory_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/memory_unit.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/memory_unit.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/metrics_enabled_config.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/metrics_enabled_config.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/mod.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/numerator.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/ping.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/ping.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/quantity.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/rate.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/rate.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/recorded_experiment.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/recorded_experiment.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/string.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/string.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/string_list.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/text.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/text.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/time_unit.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/time_unit.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/timespan.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/timing_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/url.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/url.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/metrics/uuid.rs` & `glean-sdk-52.7.0/glean-core/src/metrics/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/ping/mod.rs` & `glean-sdk-52.7.0/glean-core/src/ping/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/scheduler.rs` & `glean-sdk-52.7.0/glean-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/storage/mod.rs` & `glean-sdk-52.7.0/glean-core/src/storage/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/system.rs` & `glean-sdk-52.7.0/glean-core/src/system.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/boolean.rs` & `glean-sdk-52.7.0/glean-core/src/traits/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/counter.rs` & `glean-sdk-52.7.0/glean-core/src/traits/counter.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/custom_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/traits/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/datetime.rs` & `glean-sdk-52.7.0/glean-core/src/traits/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/event.rs` & `glean-sdk-52.7.0/glean-core/src/traits/event.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/labeled.rs` & `glean-sdk-52.7.0/glean-core/src/traits/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/memory_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/traits/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/mod.rs` & `glean-sdk-52.7.0/glean-core/src/traits/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/numerator.rs` & `glean-sdk-52.7.0/glean-core/src/traits/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/ping.rs` & `glean-sdk-52.7.0/glean-core/src/traits/ping.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/quantity.rs` & `glean-sdk-52.7.0/glean-core/src/traits/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/rate.rs` & `glean-sdk-52.7.0/glean-core/src/traits/rate.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/string.rs` & `glean-sdk-52.7.0/glean-core/src/traits/string.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/string_list.rs` & `glean-sdk-52.7.0/glean-core/src/traits/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/text.rs` & `glean-sdk-52.7.0/glean-core/src/traits/text.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/timespan.rs` & `glean-sdk-52.7.0/glean-core/src/traits/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/timing_distribution.rs` & `glean-sdk-52.7.0/glean-core/src/traits/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/url.rs` & `glean-sdk-52.7.0/glean-core/src/traits/url.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/traits/uuid.rs` & `glean-sdk-52.7.0/glean-core/src/traits/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/upload/directory.rs` & `glean-sdk-52.7.0/glean-core/src/upload/directory.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/upload/mod.rs` & `glean-sdk-52.7.0/glean-core/src/upload/mod.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/upload/policy.rs` & `glean-sdk-52.7.0/glean-core/src/upload/policy.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/upload/request.rs` & `glean-sdk-52.7.0/glean-core/src/upload/request.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/upload/result.rs` & `glean-sdk-52.7.0/glean-core/src/upload/result.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/src/util.rs` & `glean-sdk-52.7.0/glean-core/src/util.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/boolean.rs` & `glean-sdk-52.7.0/glean-core/tests/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/common/mod.rs` & `glean-sdk-52.7.0/glean-core/tests/common/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         language_binding_name: "Rust".into(),
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         app_build: "Unknown".into(),
         use_core_mps: false,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
     let glean = Glean::new(cfg).unwrap();
 
     (glean, dir)
 }
 
 /// Converts an iso8601::DateTime to a chrono::DateTime<FixedOffset>
```

### Comparing `glean-sdk-52.6.0/glean-core/tests/counter.rs` & `glean-sdk-52.7.0/glean-core/tests/counter.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/custom_distribution.rs` & `glean-sdk-52.7.0/glean-core/tests/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/datetime.rs` & `glean-sdk-52.7.0/glean-core/tests/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/event.rs` & `glean-sdk-52.7.0/glean-core/tests/event.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/labeled.rs` & `glean-sdk-52.7.0/glean-core/tests/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/memory_distribution.rs` & `glean-sdk-52.7.0/glean-core/tests/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/ping.rs` & `glean-sdk-52.7.0/glean-core/tests/ping.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/ping_maker.rs` & `glean-sdk-52.7.0/glean-core/tests/ping_maker.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/quantity.rs` & `glean-sdk-52.7.0/glean-core/tests/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/rate.rs` & `glean-sdk-52.7.0/glean-core/tests/rate.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/storage.rs` & `glean-sdk-52.7.0/glean-core/tests/storage.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/string.rs` & `glean-sdk-52.7.0/glean-core/tests/string.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/string_list.rs` & `glean-sdk-52.7.0/glean-core/tests/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/text.rs` & `glean-sdk-52.7.0/glean-core/tests/text.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/timespan.rs` & `glean-sdk-52.7.0/glean-core/tests/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/timing_distribution.rs` & `glean-sdk-52.7.0/glean-core/tests/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean-core/tests/uuid.rs` & `glean-sdk-52.7.0/glean-core/tests/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean.1.schema.json` & `glean-sdk-52.7.0/glean.1.schema.json`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/glean_sdk.egg-info/PKG-INFO` & `glean-sdk-52.7.0/glean_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-sdk
-Version: 52.6.0
+Version: 52.7.0
 Summary: Mozilla's Glean Telemetry SDK: The Machine that Goes 'Ping!'
 Home-page: https://github.com/mozilla/glean
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -85,15 +85,27 @@
 [devbook]: https://mozilla.github.io/glean/dev/
 [rustdoc]: https://mozilla.github.io/glean/docs/index.html
 [ktdoc]: https://mozilla.github.io/glean/javadoc/glean/index.html
 
 
 # Unreleased changes
 
-[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...main)
+[Full changelog](https://github.com/mozilla/glean/compare/v52.7.0...main)
+
+# v52.7.0 (2023-05-10)
+
+[Full changelog](https://github.com/mozilla/glean/compare/v52.6.0...v52.7.0)
+
+* General
+  * Allow user to configure how verbose the internal logging is ([#2459](https://github.com/mozilla/glean/pull/2459))
+  * Added a timeout waiting for the dispatcher at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+  * Added a new Glean metric `glean.validation.shutdown_dispatcher_wait` measuring the wait time at shutdown ([#2461](https://github.com/mozilla/glean/pull/2461))
+* Kotlin
+  * Update Kotlin to version 1.8.21 ([#2462](https://github.com/mozilla/glean/pull/2462))
+  * Make debugging APIs available on Android ([Bug 1830937](https://bugzilla.mozilla.org/show_bug.cgi?id=1830937))
 
 # v52.6.0 (2023-04-20)
 
 [Full changelog](https://github.com/mozilla/glean/compare/v52.5.0...v52.6.0)
 
 * Rust
   * The Text metric type is now available in the Rust language bindings ([#2451](https://github.com/mozilla/glean/pull/2451))
```

### Comparing `glean-sdk-52.6.0/glean_sdk.egg-info/SOURCES.txt` & `glean-sdk-52.7.0/glean_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/gradle/wrapper/gradle-wrapper.jar` & `glean-sdk-52.7.0/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/gradle-plugin/build.gradle` & `glean-sdk-52.7.0/gradle-plugin/build.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/GleanGradlePlugin.groovy` & `glean-sdk-52.7.0/gradle-plugin/src/main/groovy/mozilla/telemetry/glean-gradle-plugin/GleanGradlePlugin.groovy`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
             return GLEAN_PARSER_VERSION
         }
     }
 
     void apply(Project project) {
         isOffline = project.gradle.startParameter.offline
 
-        project.ext.glean_version = "52.6.0"
+        project.ext.glean_version = "52.7.0"
         def parserVersion = gleanParserVersion(project)
 
         // Print the required glean_parser version to the console. This is
         // offline builds, and is mentioned in the documentation for offline
         // builds.
         println("Requires ${parserVersion}")
```

### Comparing `glean-sdk-52.6.0/gradle.properties` & `glean-sdk-52.7.0/gradle.properties`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/gradlew` & `glean-sdk-52.7.0/gradlew`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/gradlew.bat` & `glean-sdk-52.7.0/gradlew.bat`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/README.md` & `glean-sdk-52.7.0/samples/android/app/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/build.gradle` & `glean-sdk-52.7.0/samples/android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/metrics.yaml` & `glean-sdk-52.7.0/samples/android/app/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/pings.yaml` & `glean-sdk-52.7.0/samples/android/app/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/proguard-rules.pro` & `glean-sdk-52.7.0/samples/android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/MainActivityTest.kt` & `glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/MainActivityTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/BaselinePingTest.kt` & `glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/BaselinePingTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/DeletionRequestPingTest.kt` & `glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/DeletionRequestPingTest.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/SharedTestUtils.kt` & `glean-sdk-52.7.0/samples/android/app/src/androidTest/java/org/mozilla/samples/gleancore/pings/SharedTestUtils.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/AndroidManifest.xml` & `glean-sdk-52.7.0/samples/android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/glean/GleanApplication.kt` & `glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/glean/GleanApplication.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/java/org/mozilla/samples/glean/MainActivity.kt` & `glean-sdk-52.7.0/samples/android/app/src/main/java/org/mozilla/samples/glean/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/layout/activity_main.xml` & `glean-sdk-52.7.0/samples/android/app/src/main/res/layout/activity_main.xml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-hdpi/ic_launcher.png` & `glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-hdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-mdpi/ic_launcher.png` & `glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-mdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png` & `glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png` & `glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png` & `glean-sdk-52.7.0/samples/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/android/app/src/main/res/values/strings.xml` & `glean-sdk-52.7.0/samples/android/app/src/main/res/values/strings.xml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/README.md` & `glean-sdk-52.7.0/samples/ios/app/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/AppDelegate.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/AppDelegate.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/Contents.json` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Base.lproj/LaunchScreen.storyboard` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Base.lproj/Main.storyboard` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/Info.plist` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/Info.plist`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app/ViewController.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app/ViewController.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.pbxproj` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/glean-sample-app.xcscheme` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-app.xcodeproj/xcshareddata/xcschemes/glean-sample-app.xcscheme`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appTests/Info.plist` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appTests/Info.plist`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appTests/glean_sample_appTests.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appTests/glean_sample_appTests.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/BaselinePingTest.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/BaselinePingTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/DeletionRequestPingTest.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/DeletionRequestPingTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/EventPingTest.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/EventPingTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/Info.plist` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/Info.plist`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/MockServer.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/MockServer.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/glean-sample-appUITests/ViewControllerTest.swift` & `glean-sdk-52.7.0/samples/ios/app/glean-sample-appUITests/ViewControllerTest.swift`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/metrics.yaml` & `glean-sdk-52.7.0/samples/ios/app/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/pings.yaml` & `glean-sdk-52.7.0/samples/ios/app/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/ios/app/sdk_generator.sh` & `glean-sdk-52.7.0/samples/ios/app/sdk_generator.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/rust/metrics.yaml` & `glean-sdk-52.7.0/samples/rust/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/rust/pings.yaml` & `glean-sdk-52.7.0/samples/rust/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/samples/rust/src/main.rs` & `glean-sdk-52.7.0/samples/rust/src/main.rs`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         upload_enabled: true,
         max_events: None,
         delay_ping_lifetime_io: false,
         server_endpoint: Some("invalid-test-host".into()),
         uploader: None,
         use_core_mps: true,
         trim_data_to_registered_pings: false,
+        log_level: None,
     };
 
     let client_info = ClientInfoMetrics {
         app_build: env!("CARGO_PKG_VERSION").to_string(),
         app_display_version: env!("CARGO_PKG_VERSION").to_string(),
         channel: None,
     };
```

### Comparing `glean-sdk-52.6.0/settings.gradle` & `glean-sdk-52.7.0/settings.gradle`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/setup.py` & `glean-sdk-52.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/supply-chain/config.toml` & `glean-sdk-52.7.0/supply-chain/config.toml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/supply-chain/imports.lock` & `glean-sdk-52.7.0/supply-chain/imports.lock`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/android-build/kind.yml` & `glean-sdk-52.7.0/taskcluster/ci/android-build/kind.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/beetmover/kind.yml` & `glean-sdk-52.7.0/taskcluster/ci/beetmover/kind.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/config.yml` & `glean-sdk-52.7.0/taskcluster/ci/config.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/module-build/kind.yml` & `glean-sdk-52.7.0/taskcluster/ci/module-build/kind.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/rust/kind.yml` & `glean-sdk-52.7.0/taskcluster/ci/rust/kind.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/ci/signing/kind.yml` & `glean-sdk-52.7.0/taskcluster/ci/signing/kind.yml`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/docker/linux/Dockerfile` & `glean-sdk-52.7.0/taskcluster/docker/linux/Dockerfile`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/docker/linux/runlocally.sh` & `glean-sdk-52.7.0/taskcluster/docker/linux/runlocally.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/__init__.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/build_config.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/build_config.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/job.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/job.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/__init__.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/build_config.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/build_config.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/loader/multi_dep.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/loader/multi_dep.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/target_tasks.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/__init__.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/beetmover.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/beetmover.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/module_build.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/module_build.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/multi_dep.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/multi_dep.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/transforms/signing.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/transforms/signing.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/glean_taskgraph/worker_types.py` & `glean-sdk-52.7.0/taskcluster/glean_taskgraph/worker_types.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/requirements.txt` & `glean-sdk-52.7.0/taskcluster/requirements.txt`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/scripts/cross-compile-setup.sh` & `glean-sdk-52.7.0/taskcluster/scripts/cross-compile-setup.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/scripts/macos.manifest` & `glean-sdk-52.7.0/taskcluster/scripts/macos.manifest`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/taskcluster/scripts/rustup-setup.sh` & `glean-sdk-52.7.0/taskcluster/scripts/rustup-setup.sh`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/tools/analysis/ping-patterns/README.md` & `glean-sdk-52.7.0/tools/analysis/ping-patterns/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/tools/analysis/ping-patterns/config.py` & `glean-sdk-52.7.0/tools/analysis/ping-patterns/config.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/tools/analysis/ping-patterns/ping-patterns.py` & `glean-sdk-52.7.0/tools/analysis/ping-patterns/ping-patterns.py`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/README.md` & `glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/README.md`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/tools/embedded-uniffi-bindgen/src/main.rs` & `glean-sdk-52.7.0/tools/embedded-uniffi-bindgen/src/main.rs`

 * *Files identical despite different names*

### Comparing `glean-sdk-52.6.0/xcconfig/common.xcconfig` & `glean-sdk-52.7.0/xcconfig/common.xcconfig`

 * *Files identical despite different names*

