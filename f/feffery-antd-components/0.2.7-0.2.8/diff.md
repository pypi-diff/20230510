# Comparing `tmp/feffery_antd_components-0.2.7.tar.gz` & `tmp/feffery_antd_components-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_components-0.2.7.tar", last modified: Wed May 10 07:00:54 2023, max compression
+gzip compressed data, was "feffery_antd_components-0.2.8.tar", last modified: Wed May 10 08:23:38 2023, max compression
```

## Comparing `feffery_antd_components-0.2.7.tar` & `feffery_antd_components-0.2.8.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:00:54.990317 feffery_antd_components-0.2.7/
--rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-05-10 07:00:54.990317 feffery_antd_components-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2301 2023-05-04 07:03:17.000000 feffery_antd_components-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 07:00:54.981222 feffery_antd_components-0.2.7/feffery_antd_components/
--rw-rw-rw-   0        0        0     3328 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAccordion.py
--rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAccordionItem.py
--rw-rw-rw-   0        0        0     2006 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAffix.py
--rw-rw-rw-   0        0        0     2627 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAlert.py
--rw-rw-rw-   0        0        0     2314 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAnchor.py
--rw-rw-rw-   0        0        0     2586 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAvatar.py
--rw-rw-rw-   0        0        0     2611 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdAvatarGroup.py
--rw-rw-rw-   0        0        0     1892 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdBackTop.py
--rw-rw-rw-   0        0        0     2730 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdBadge.py
--rw-rw-rw-   0        0        0     2313 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdBreadcrumb.py
--rw-rw-rw-   0        0        0     3218 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdButton.py
--rw-rw-rw-   0        0        0     3356 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCalendar.py
--rw-rw-rw-   0        0        0     2991 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCard.py
--rw-rw-rw-   0        0        0     1924 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCardGrid.py
--rw-rw-rw-   0        0        0     2490 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCarousel.py
--rw-rw-rw-   0        0        0     5312 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCascader.py
--rw-rw-rw-   0        0        0     3615 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckCard.py
--rw-rw-rw-   0        0        0     3694 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckCardGroup.py
--rw-rw-rw-   0        0        0     3303 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckbox.py
--rw-rw-rw-   0        0        0     3388 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckboxGroup.py
--rw-rw-rw-   0        0        0     3890 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCol.py
--rw-rw-rw-   0        0        0     3763 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCollapse.py
--rw-rw-rw-   0        0        0     3987 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdComment.py
--rw-rw-rw-   0        0        0     2044 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCompact.py
--rw-rw-rw-   0        0        0     2076 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdConfigProvider.py
--rw-rw-rw-   0        0        0     1824 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdContent.py
--rw-rw-rw-   0        0        0     2109 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCopyText.py
--rw-rw-rw-   0        0        0     2497 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCountdown.py
--rw-rw-rw-   0        0        0     2530 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdCustomSkeleton.py
--rw-rw-rw-   0        0        0     5475 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDatePicker.py
--rw-rw-rw-   0        0        0     5549 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDateRangePicker.py
--rw-rw-rw-   0        0        0     2263 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDescriptionItem.py
--rw-rw-rw-   0        0        0     2745 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDescriptions.py
--rw-rw-rw-   0        0        0     2676 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDivider.py
--rw-rw-rw-   0        0        0     6311 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDraggerUpload.py
--rw-rw-rw-   0        0        0     3109 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDrawer.py
--rw-rw-rw-   0        0        0     4183 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdDropdown.py
--rw-rw-rw-   0        0        0     2250 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdEmpty.py
--rw-rw-rw-   0        0        0     1820 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdFooter.py
--rw-rw-rw-   0        0        0     2552 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdForm.py
--rw-rw-rw-   0        0        0     3344 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdFormItem.py
--rw-rw-rw-   0        0        0     1820 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdHeader.py
--rw-rw-rw-   0        0        0     1829 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdIcon.py
--rw-rw-rw-   0        0        0     5562 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdImage.py
--rw-rw-rw-   0        0        0     5779 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdInput.py
--rw-rw-rw-   0        0        0     5082 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdInputNumber.py
--rw-rw-rw-   0        0        0     1820 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdLayout.py
--rw-rw-rw-   0        0        0     3094 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdMentions.py
--rw-rw-rw-   0        0        0     4059 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdMenu.py
--rw-rw-rw-   0        0        0     2110 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdMessage.py
--rw-rw-rw-   0        0        0     5365 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdModal.py
--rw-rw-rw-   0        0        0     2417 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdNotification.py
--rw-rw-rw-   0        0        0     2555 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPageHeader.py
--rw-rw-rw-   0        0        0     4592 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPagination.py
--rw-rw-rw-   0        0        0     2752 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdParagraph.py
--rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPasteImage.py
--rw-rw-rw-   0        0        0     6418 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPictureUpload.py
--rw-rw-rw-   0        0        0     4807 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPopconfirm.py
--rw-rw-rw-   0        0        0     3562 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPopover.py
--rw-rw-rw-   0        0        0     2869 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdPopupCard.py
--rw-rw-rw-   0        0        0     3352 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdProgress.py
--rw-rw-rw-   0        0        0     4008 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdRadioGroup.py
--rw-rw-rw-   0        0        0     3488 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdRate.py
--rw-rw-rw-   0        0        0     2181 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdResult.py
--rw-rw-rw-   0        0        0     2068 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdRibbon.py
--rw-rw-rw-   0        0        0     2489 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdRow.py
--rw-rw-rw-   0        0        0     3715 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSegmented.py
--rw-rw-rw-   0        0        0     3598 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSegmentedColoring.py
--rw-rw-rw-   0        0        0     7197 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSelect.py
--rw-rw-rw-   0        0        0     2846 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSider.py
--rw-rw-rw-   0        0        0     3193 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeleton.py
--rw-rw-rw-   0        0        0     1934 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonAvatar.py
--rw-rw-rw-   0        0        0     2017 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonButton.py
--rw-rw-rw-   0        0        0     1604 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonImage.py
--rw-rw-rw-   0        0        0     1808 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonInput.py
--rw-rw-rw-   0        0        0     4230 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSlider.py
--rw-rw-rw-   0        0        0     2566 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSpace.py
--rw-rw-rw-   0        0        0     2931 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSpin.py
--rw-rw-rw-   0        0        0     2853 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSpoiler.py
--rw-rw-rw-   0        0        0     2607 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdStatistic.py
--rw-rw-rw-   0        0        0     3223 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSteps.py
--rw-rw-rw-   0        0        0     3651 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdSwitch.py
--rw-rw-rw-   0        0        0     2314 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTabPane.py
--rw-rw-rw-   0        0        0    19336 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTable.py
--rw-rw-rw-   0        0        0     5266 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTabs.py
--rw-rw-rw-   0        0        0     1950 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTag.py
--rw-rw-rw-   0        0        0     2820 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdText.py
--rw-rw-rw-   0        0        0     4722 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTimePicker.py
--rw-rw-rw-   0        0        0     4787 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTimeRangePicker.py
--rw-rw-rw-   0        0        0     2750 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTimeline.py
--rw-rw-rw-   0        0        0     2900 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTitle.py
--rw-rw-rw-   0        0        0     3445 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTooltip.py
--rw-rw-rw-   0        0        0     4586 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTransfer.py
--rw-rw-rw-   0        0        0     5585 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTree.py
--rw-rw-rw-   0        0        0     6685 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdTreeSelect.py
--rw-rw-rw-   0        0        0     6123 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdUpload.py
--rw-rw-rw-   0        0        0     2397 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/AntdWatermark.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.7/feffery_antd_components/__init__.py
--rw-rw-rw-   0        0        0     5810 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/_imports_.py
--rw-rw-rw-   0        0        0  3776761 2023-05-10 07:00:47.000000 feffery_antd_components-0.2.7/feffery_antd_components/feffery_antd_components.min.js
--rw-rw-rw-   0        0        0   632608 2023-05-10 07:00:53.000000 feffery_antd_components-0.2.7/feffery_antd_components/metadata.json
--rw-rw-rw-   0        0        0     3034 2023-05-10 07:00:49.000000 feffery_antd_components-0.2.7/feffery_antd_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-05-10 07:00:54.988306 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/
--rw-rw-rw-   0        0        0      346 2023-05-10 07:00:54.000000 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4380 2023-05-10 07:00:54.000000 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:00:54.000000 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 07:00:54.000000 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-10 07:00:54.000000 feffery_antd_components-0.2.7/feffery_antd_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3034 2023-05-10 06:59:21.000000 feffery_antd_components-0.2.7/package.json
--rw-rw-rw-   0        0        0       42 2023-05-10 07:00:54.990317 feffery_antd_components-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:23:38.767040 feffery_antd_components-0.2.8/
+-rw-rw-rw-   0        0        0     1087 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-05-10 08:23:38.766042 feffery_antd_components-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2301 2023-05-10 08:20:42.000000 feffery_antd_components-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:23:38.755522 feffery_antd_components-0.2.8/feffery_antd_components/
+-rw-rw-rw-   0        0        0     3328 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAccordion.py
+-rw-rw-rw-   0        0        0     2539 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAccordionItem.py
+-rw-rw-rw-   0        0        0     2006 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAffix.py
+-rw-rw-rw-   0        0        0     2627 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAlert.py
+-rw-rw-rw-   0        0        0     2314 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAnchor.py
+-rw-rw-rw-   0        0        0     2586 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAvatar.py
+-rw-rw-rw-   0        0        0     2611 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdAvatarGroup.py
+-rw-rw-rw-   0        0        0     1892 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdBackTop.py
+-rw-rw-rw-   0        0        0     2730 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdBadge.py
+-rw-rw-rw-   0        0        0     2313 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdBreadcrumb.py
+-rw-rw-rw-   0        0        0     3218 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdButton.py
+-rw-rw-rw-   0        0        0     3356 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCalendar.py
+-rw-rw-rw-   0        0        0     2991 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCard.py
+-rw-rw-rw-   0        0        0     1924 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCardGrid.py
+-rw-rw-rw-   0        0        0     2490 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCarousel.py
+-rw-rw-rw-   0        0        0     5312 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCascader.py
+-rw-rw-rw-   0        0        0     3615 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckCard.py
+-rw-rw-rw-   0        0        0     3694 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckCardGroup.py
+-rw-rw-rw-   0        0        0     3303 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckbox.py
+-rw-rw-rw-   0        0        0     3388 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckboxGroup.py
+-rw-rw-rw-   0        0        0     3890 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCol.py
+-rw-rw-rw-   0        0        0     3763 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCollapse.py
+-rw-rw-rw-   0        0        0     3987 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdComment.py
+-rw-rw-rw-   0        0        0     2044 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCompact.py
+-rw-rw-rw-   0        0        0     2076 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdConfigProvider.py
+-rw-rw-rw-   0        0        0     1824 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdContent.py
+-rw-rw-rw-   0        0        0     2109 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCopyText.py
+-rw-rw-rw-   0        0        0     2497 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCountdown.py
+-rw-rw-rw-   0        0        0     2530 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdCustomSkeleton.py
+-rw-rw-rw-   0        0        0     5475 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDatePicker.py
+-rw-rw-rw-   0        0        0     5549 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDateRangePicker.py
+-rw-rw-rw-   0        0        0     2263 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDescriptionItem.py
+-rw-rw-rw-   0        0        0     2745 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDescriptions.py
+-rw-rw-rw-   0        0        0     2676 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDivider.py
+-rw-rw-rw-   0        0        0     6311 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDraggerUpload.py
+-rw-rw-rw-   0        0        0     3109 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDrawer.py
+-rw-rw-rw-   0        0        0     4183 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdDropdown.py
+-rw-rw-rw-   0        0        0     2250 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdEmpty.py
+-rw-rw-rw-   0        0        0     1820 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdFooter.py
+-rw-rw-rw-   0        0        0     2552 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdForm.py
+-rw-rw-rw-   0        0        0     3344 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdFormItem.py
+-rw-rw-rw-   0        0        0     1820 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdHeader.py
+-rw-rw-rw-   0        0        0     1829 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdIcon.py
+-rw-rw-rw-   0        0        0     5562 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdImage.py
+-rw-rw-rw-   0        0        0     5779 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdInput.py
+-rw-rw-rw-   0        0        0     5082 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdInputNumber.py
+-rw-rw-rw-   0        0        0     1820 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdLayout.py
+-rw-rw-rw-   0        0        0     3094 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdMentions.py
+-rw-rw-rw-   0        0        0     4059 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdMenu.py
+-rw-rw-rw-   0        0        0     2110 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdMessage.py
+-rw-rw-rw-   0        0        0     5365 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdModal.py
+-rw-rw-rw-   0        0        0     2417 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdNotification.py
+-rw-rw-rw-   0        0        0     2555 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPageHeader.py
+-rw-rw-rw-   0        0        0     4592 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPagination.py
+-rw-rw-rw-   0        0        0     2752 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdParagraph.py
+-rw-rw-rw-   0        0        0     2002 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPasteImage.py
+-rw-rw-rw-   0        0        0     6418 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPictureUpload.py
+-rw-rw-rw-   0        0        0     4807 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPopconfirm.py
+-rw-rw-rw-   0        0        0     3562 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPopover.py
+-rw-rw-rw-   0        0        0     2869 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdPopupCard.py
+-rw-rw-rw-   0        0        0     3352 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdProgress.py
+-rw-rw-rw-   0        0        0     4008 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdRadioGroup.py
+-rw-rw-rw-   0        0        0     3488 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdRate.py
+-rw-rw-rw-   0        0        0     2181 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdResult.py
+-rw-rw-rw-   0        0        0     2068 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdRibbon.py
+-rw-rw-rw-   0        0        0     2489 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdRow.py
+-rw-rw-rw-   0        0        0     3715 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSegmented.py
+-rw-rw-rw-   0        0        0     3598 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSegmentedColoring.py
+-rw-rw-rw-   0        0        0     7197 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSelect.py
+-rw-rw-rw-   0        0        0     2846 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSider.py
+-rw-rw-rw-   0        0        0     3193 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeleton.py
+-rw-rw-rw-   0        0        0     1934 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonAvatar.py
+-rw-rw-rw-   0        0        0     2017 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonButton.py
+-rw-rw-rw-   0        0        0     1604 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonImage.py
+-rw-rw-rw-   0        0        0     1808 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonInput.py
+-rw-rw-rw-   0        0        0     4230 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSlider.py
+-rw-rw-rw-   0        0        0     2566 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSpace.py
+-rw-rw-rw-   0        0        0     2931 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSpin.py
+-rw-rw-rw-   0        0        0     2853 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSpoiler.py
+-rw-rw-rw-   0        0        0     2607 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdStatistic.py
+-rw-rw-rw-   0        0        0     3223 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSteps.py
+-rw-rw-rw-   0        0        0     3651 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdSwitch.py
+-rw-rw-rw-   0        0        0     2314 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTabPane.py
+-rw-rw-rw-   0        0        0    19336 2023-05-10 08:18:41.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTable.py
+-rw-rw-rw-   0        0        0     5266 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTabs.py
+-rw-rw-rw-   0        0        0     1950 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTag.py
+-rw-rw-rw-   0        0        0     2820 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdText.py
+-rw-rw-rw-   0        0        0     4722 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTimePicker.py
+-rw-rw-rw-   0        0        0     4787 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTimeRangePicker.py
+-rw-rw-rw-   0        0        0     2750 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTimeline.py
+-rw-rw-rw-   0        0        0     2900 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTitle.py
+-rw-rw-rw-   0        0        0     3445 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTooltip.py
+-rw-rw-rw-   0        0        0     4586 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTransfer.py
+-rw-rw-rw-   0        0        0     5585 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTree.py
+-rw-rw-rw-   0        0        0     6685 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdTreeSelect.py
+-rw-rw-rw-   0        0        0     6123 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdUpload.py
+-rw-rw-rw-   0        0        0     2397 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/AntdWatermark.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 07:50:35.000000 feffery_antd_components-0.2.8/feffery_antd_components/__init__.py
+-rw-rw-rw-   0        0        0     5810 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/_imports_.py
+-rw-rw-rw-   0        0        0  3776761 2023-05-10 08:18:36.000000 feffery_antd_components-0.2.8/feffery_antd_components/feffery_antd_components.min.js
+-rw-rw-rw-   0        0        0   632608 2023-05-10 08:18:42.000000 feffery_antd_components-0.2.8/feffery_antd_components/metadata.json
+-rw-rw-rw-   0        0        0     3032 2023-05-10 08:18:37.000000 feffery_antd_components-0.2.8/feffery_antd_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-05-10 08:23:38.764529 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-05-10 08:23:38.000000 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4380 2023-05-10 08:23:38.000000 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:23:38.000000 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 08:23:38.000000 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 08:23:38.000000 feffery_antd_components-0.2.8/feffery_antd_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3032 2023-05-10 08:23:29.000000 feffery_antd_components-0.2.8/package.json
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:23:38.767040 feffery_antd_components-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-25 07:15:34.000000 feffery_antd_components-0.2.8/setup.py
```

### Comparing `feffery_antd_components-0.2.7/LICENSE` & `feffery_antd_components-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/README.md` & `feffery_antd_components-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-components "Percentage of issues still open")
 
 </div>
 
 简体中文 | [English](./README-en_US.md)
 
-`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.6`
+`feffery-components`计划子项目，`Plotly Dash`第三方组件库，基于`Antd`，将超多具有丰富功能的通用网页常用交互组件引入`Dash`的生态中 🥳，最新稳定版本：`0.2.8`
 
 ## 1 最新版本安装方式
 
 ```bash
 pip install feffery-antd-components -U
 ```
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
  components "Average time to resolve an issue") [![Percentage of issues still
       open](http://isitmaintained.com/badge/open/CNFeffery/feffery-antd-
   components.svg)](http://isitmaintained.com/project/CNFeffery/feffery-antd-
                  components "Percentage of issues still open")
 ç®ä½ä¸­æ | [English](./README-en_US.md) `feffery-
 components`è®¡åå­é¡¹ç®ï¼`Plotly
 Dash`ç¬¬ä¸æ¹ç»ä»¶åºï¼åºäº`Antd`ï¼å°è¶å¤å·æä¸°å¯åè½çéç¨ç½é¡µå¸¸ç¨äº¤äºç»ä»¶å¼å¥`Dash`ççæä¸­
-ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.6` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
+ð¥³ï¼ææ°ç¨³å®çæ¬ï¼`0.2.8` ## 1 ææ°çæ¬å®è£æ¹å¼ ```bash pip
 install feffery-antd-components -U ``` ## 2 ææ°é¢åå¸çæ¬å®è£æ¹å¼
 ```bash pip install feffery-antd-components --pre -U ``` ## 3 éæèµæº CDN
 å éæ¹æ³ ```Python # édebugæ¨¡å¼ä¸å¯¹Dash
 ()ä¼ å¥åæ°serve_locally=Falseä¼å¼ºå¶æµè§å¨ç«¯ä»unpkg
 cdnå è½½åä¸ªä¾èµç #
 xxx.min.jsç­éæèµæºï¼ä»èé¿åå ç¨æå¡å¨å¸¦å®½ï¼éåä¸­å°åç«ç¹å éè®¿é®
 app = dash.Dash(serve_locally=False) ``` ## 4 å¨çº¿ææ¡£ ææ¡£å°å ## 5
```

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAccordion.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAccordion.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAccordionItem.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAccordionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAffix.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAffix.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAlert.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAlert.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAnchor.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAnchor.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAvatar.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdAvatarGroup.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdAvatarGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdBackTop.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdBackTop.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdBadge.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdBadge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdBreadcrumb.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdBreadcrumb.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdButton.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCalendar.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCalendar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCard.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCardGrid.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCardGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCarousel.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCarousel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCascader.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCascader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckCard.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckCardGroup.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckCardGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckbox.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckbox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCheckboxGroup.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCol.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCol.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCollapse.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCollapse.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdComment.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdComment.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCompact.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCompact.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdConfigProvider.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdConfigProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdContent.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdContent.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCopyText.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCopyText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCountdown.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCountdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdCustomSkeleton.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdCustomSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDatePicker.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDatePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDateRangePicker.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDescriptionItem.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDescriptionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDescriptions.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDescriptions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDivider.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDivider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDraggerUpload.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDraggerUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDrawer.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDrawer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdDropdown.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdDropdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdEmpty.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdEmpty.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdFooter.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdFooter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdForm.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdForm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdFormItem.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdFormItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdHeader.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdIcon.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdIcon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdImage.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdInput.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdInputNumber.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdInputNumber.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdLayout.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdLayout.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdMentions.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdMentions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdMenu.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdMenu.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdMessage.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdModal.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdModal.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdNotification.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPageHeader.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPageHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPagination.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPagination.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdParagraph.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdParagraph.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPasteImage.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPasteImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPictureUpload.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPictureUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPopconfirm.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPopconfirm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPopover.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPopover.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdPopupCard.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdPopupCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdProgress.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdRadioGroup.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdRadioGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdRate.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdRate.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdResult.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdResult.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdRibbon.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdRibbon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdRow.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdRow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSegmented.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSegmented.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSegmentedColoring.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSegmentedColoring.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSelect.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSider.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeleton.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonAvatar.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonButton.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonImage.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSkeletonInput.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSkeletonInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSlider.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSpace.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSpace.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSpin.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSpin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSpoiler.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSpoiler.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdStatistic.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdStatistic.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSteps.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSteps.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdSwitch.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdSwitch.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTabPane.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTabPane.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTable.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTable.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTabs.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTabs.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTag.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTag.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdText.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTimePicker.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTimePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTimeRangePicker.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTimeRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTimeline.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTimeline.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTitle.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTooltip.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTransfer.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTransfer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTree.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTree.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdTreeSelect.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdTreeSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdUpload.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/AntdWatermark.py` & `feffery_antd_components-0.2.8/feffery_antd_components/AntdWatermark.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/__init__.py` & `feffery_antd_components-0.2.8/feffery_antd_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/_imports_.py` & `feffery_antd_components-0.2.8/feffery_antd_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/feffery_antd_components.min.js` & `feffery_antd_components-0.2.8/feffery_antd_components/feffery_antd_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
     return Object.defineProperty(r, "p", {
         get: (t = o().src.split("/").slice(0, -1).join("/") + "/", function() {
             return t
         })
     }), "undefined" != typeof jsonpScriptSrc && (i = jsonpScriptSrc, jsonpScriptSrc = function(t) {
         var e, n = /\/_dash-component-suites\//.test(o().src),
             t = i(t);
-        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_7m1683702006"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
+        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_8m1683706677"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
     }), r(r.s = 688)
 }([function(t, e) {
     t.exports = window.React
 }, function(t, e) {
     t.exports = window.PropTypes
 }, function(R, t, e) {
     "use strict";
```

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/metadata.json` & `feffery_antd_components-0.2.8/feffery_antd_components/metadata.json`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components/package-info.json` & `feffery_antd_components-0.2.8/feffery_antd_components/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.8'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.7"
+    "version": "0.2.8"
 }
```

### Comparing `feffery_antd_components-0.2.7/feffery_antd_components.egg-info/SOURCES.txt` & `feffery_antd_components-0.2.8/feffery_antd_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.7/package.json` & `feffery_antd_components-0.2.8/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.8'"}*

```diff
@@ -84,9 +84,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.7"
+    "version": "0.2.8"
 }
```

### Comparing `feffery_antd_components-0.2.7/setup.py` & `feffery_antd_components-0.2.8/setup.py`

 * *Files identical despite different names*

