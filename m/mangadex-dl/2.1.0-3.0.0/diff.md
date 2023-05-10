# Comparing `tmp/mangadex_dl-2.1.0-py3-none-any.whl.zip` & `tmp/mangadex_dl-3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13527 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-03 06:42 mangadex_dl/__init__.py
--rw-rw-rw-  2.0 fat     3822 b- defN 23-Apr-05 05:47 mangadex_dl/chapter.py
--rw-rw-rw-  2.0 fat     6946 b- defN 23-Apr-05 05:39 mangadex_dl/cli.py
--rw-rw-rw-  2.0 fat      974 b- defN 23-Apr-05 05:53 mangadex_dl/constants.py
--rw-rw-rw-  2.0 fat     8999 b- defN 23-Apr-04 04:22 mangadex_dl/helper.py
--rw-rw-rw-  2.0 fat     1801 b- defN 23-Apr-04 03:47 mangadex_dl/manga.py
--rw-rw-rw-  2.0 fat     4731 b- defN 23-Apr-04 04:19 mangadex_dl/organiser.py
--rw-rw-rw-  2.0 fat     1073 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7192 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1052 b- defN 23-Apr-05 05:59 mangadex_dl-2.1.0.dist-info/RECORD
-13 files, 36747 bytes uncompressed, 11767 bytes compressed:  68.0%
+Zip file size: 11356 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-05 10:57 mangadex_dl/__init__.py
+-rw-rw-rw-  2.0 fat     3083 b- defN 23-May-09 16:13 mangadex_dl/chapter.py
+-rw-rw-rw-  2.0 fat     6281 b- defN 23-May-09 16:13 mangadex_dl/cli.py
+-rw-rw-rw-  2.0 fat      974 b- defN 23-May-09 16:18 mangadex_dl/constants.py
+-rw-rw-rw-  2.0 fat      789 b- defN 23-May-09 16:13 mangadex_dl/helper.py
+-rw-rw-rw-  2.0 fat     1011 b- defN 23-May-09 16:13 mangadex_dl/manga.py
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-May-09 16:13 mangadex_dl/organiser.py
+-rw-rw-rw-  2.0 fat     1073 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7192 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1052 b- defN 23-May-09 16:28 mangadex_dl-3.0.0.dist-info/RECORD
+13 files, 26445 bytes uncompressed, 9596 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mangadex_dl/manga.py
 Comment: 
 
 Filename: mangadex_dl/organiser.py
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/LICENSE
+Filename: mangadex_dl-3.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/METADATA
+Filename: mangadex_dl-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/WHEEL
+Filename: mangadex_dl-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/entry_points.txt
+Filename: mangadex_dl-3.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/top_level.txt
+Filename: mangadex_dl-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mangadex_dl-2.1.0.dist-info/RECORD
+Filename: mangadex_dl-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mangadex_dl/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6e61 6d65 3d22 6d61 6e67 6164 6578 5f64  name="mangadex_d
+00000010: 6c22                                     l"
```

## mangadex_dl/chapter.py

```diff
@@ -1,106 +1,88 @@
-from mangadex_dl.helper import name_gen
-import time
-import requests
-from shutil import copyfileobj
-import os
-import mangadex
-from mangadex_dl.organiser import Organiser
-api = mangadex.Api()
-
-
-class MangaChapter(Organiser):
-
-    def __init__(self, ch_url) -> None:
-        self.id = ch_url.split('/')[-1]
-        self.chapter_number = str(api.get_chapter(self.id).chapter)
-        self.chapter_name = api.get_chapter(self.id).title
-
-    def download_chapter(self, data_saver):
-        ch_number = str(self.chapter_number)
-        print('\ndownloading images for chapter {}..'.format(ch_number))
-        os.mkdir(ch_number)
-        all_ch_image_path = []
-        try:
-            r = requests.get(
-                url='https://api.mangadex.org/at-home/server/' + self.id)
-            data = r.json()
-            baseurl = data['baseUrl']
-            hash = data['chapter']['hash']
-            time.sleep(0.75)
-        except:
-            time.sleep(6.0)
-            try:
-                r = requests.get(
-                    url='https://api.mangadex.org/at-home/server/' + self.id)
-                data = r.json()
-                baseurl = data['baseUrl']
-                hash = data['chapter']['hash']
-            except:
-                print(
-                    'ERROR: server is too crowded please wait a bit and re-run the program')
-                return 0
-
-        image_list = []
-
-        if data_saver:
-            url = baseurl + '/data-saver/' + hash + '/'
-            for j in data['chapter']['dataSaver']:
-                image_list.append(url + j)
-        else:
-            url = baseurl + '/data/' + hash + '/'
-            for j in data['chapter']['data']:
-                image_list.append(url + j)
-
-        overlay = name_gen(len(image_list))
-        unable_to_download = []
-        for j in image_list:
-            try:
-                r = requests.get(j, stream=True)
-            except:
-                n = 1
-                while n < 10:
-                    try:
-                        r = requests.get(j, stream=True)
-                        break
-                    except:
-                        n += 1
-                        pass
-                else:
-                    unable_to_download.append(image_list.index(j) + 1)
-                    continue
-
-            with open(ch_number + '/' + overlay[image_list.index(j)] + '-' + str(image_list.index(j) + 1) + j[-4:], 'wb') as f:
-                r.raw.decode_content = True
-                copyfileobj(r.raw, f)
-
-            all_ch_image_path.append(
-                ch_number + '/' + overlay[image_list.index(j)] + '-' + str(image_list.index(j) + 1) + j[-4:])
-
-        if unable_to_download:
-            print('unable to download page(s) {}. skipping page(s)..'.format(
-                str(unable_to_download)))
-
-        if os.path.exists('all_images_paths.txt'):
-
-            with open('all_images_paths.txt', 'r') as f:
-                all_images_paths_list = eval(f.read())
-            with open('all_images_paths.txt', 'w') as f:
-                all_images_paths_list.extend(all_ch_image_path)
-                f.write(str(all_images_paths_list))
-
-        else:
-
-            with open('all_images_paths.txt', 'w') as f:
-                f.write(str(all_ch_image_path))
-
-        if os.path.exists('all_images_paths_ch_dict.txt'):
-            ch_dict = {ch_number: all_ch_image_path}
-            with open('all_images_paths_ch_dict.txt', 'r') as f:
-                all_images_paths_ch_dict = eval(f.read())
-            with open('all_images_paths_ch_dict.txt', 'w') as f:
-                all_images_paths_ch_dict.update(ch_dict)
-                f.write(str(all_images_paths_ch_dict))
-        else:
-            with open('all_images_paths_ch_dict.txt', 'w') as f:
-                f.write(str({ch_number: all_ch_image_path}))
-        return 1
+from mangadex_dl.helper import name_gen, update_file
+import time
+import requests
+from shutil import copyfileobj
+import os
+import mangadex
+import sys
+api = mangadex.Api()
+
+
+class MangaChapter:
+
+    def __init__(self, ch_url) -> None:
+        self.id = ch_url.split(
+            '/')[-1] if ch_url[-1] != '/' else ch_url.split('/')[-2]
+        self.__get_ch = api.get_chapter(self.id)
+        self.chapter_number = str(self.__get_ch.chapter)
+        self.chapter_name = self.__get_ch.title
+
+    def __connect_to_server(self, _id: str):
+        r = requests.get(
+            url='https://api.mangadex.org/at-home/server/' + _id, timeout=10)
+        data = r.json()
+
+        baseurl = data['baseUrl']
+        _hash = data['chapter']['hash']
+        return data, baseurl, _hash
+
+    def download_chapter(self, data_saver):
+        ch_number = float(self.chapter_number)
+        print('\ndownloading images for chapter {}..'.format(ch_number))
+        os.mkdir(str(ch_number))
+        all_ch_image_path = []
+        try:
+            data, baseurl, _hash = self.__connect_to_server(self.id)
+            time.sleep(0.75)
+        except:
+            time.sleep(6.0)
+            try:
+                data, baseurl, _hash = self.__connect_to_server(self.id)
+            except:
+                print(
+                    'ERROR: server is too crowded please wait a bit and re-run the program')
+                sys.exit()
+
+        image_url_list = []
+
+        url = baseurl + '/data/' + _hash + \
+            '/' if data_saver else '/data-saver/' + _hash + '/'
+        for i in data['chapter']['data' if data_saver else 'dataSaver']:
+            image_url_list.append(url + i)
+
+        overlay = name_gen(len(image_url_list))
+        unable_to_download = []
+
+        for j in image_url_list:
+            image_index = image_url_list.index(j)
+            try:
+                r = requests.get(j, stream=True)
+            except:
+                for i in range(6):
+                    try:
+                        r = requests.get(j, stream=True)
+                        break
+                    except:
+                        time.sleep(5)
+                        continue
+                else:
+                    unable_to_download.append(image_index + 1)
+                    continue
+
+            image_file_path = str(ch_number) + '/' + \
+                overlay[image_index] + '-' + str(image_index + 1) + j[-4:]
+            with open(image_file_path, 'wb') as f:
+                r.raw.decode_content = True
+                copyfileobj(r.raw, f)
+
+            all_ch_image_path.append(
+                image_file_path)
+
+        if unable_to_download:
+            print('unable to download page(s) {}. skipping page(s)..'.format(
+                str(unable_to_download)))
+
+        update_file('all_images_paths.txt', all_ch_image_path, 'list')
+        update_file('all_images_paths_ch_dict.txt', {
+                    ch_number: all_ch_image_path}, 'dict')
+        return {ch_number: all_ch_image_path}
```

## mangadex_dl/cli.py

```diff
@@ -16,155 +16,133 @@
 - it names files in the format aaa-1.jpg, aab-2.jpg...ect.
   if not, the file order will be quite messed up
 
 This software is completely open source.
 Feel free to use it as you like!
 
 '''
-
-from sys import argv
-from mangadex_dl.helper import *
 from mangadex_dl.organiser import Organiser
 from mangadex_dl.manga import Manga
 from mangadex_dl.chapter import MangaChapter
+from mangadex_dl.constants import VERSION
 import os
 from shutil import rmtree
 from random import randint
 from time import sleep
-
-args = argv
-arg_dict = get_arguments(args)
+import argparse
+import sys
+parser = argparse.ArgumentParser(prog='mangadex-dl',
+                                 formatter_class=argparse.RawDescriptionHelpFormatter,
+                                 description='Python CLI that downloads manga from mangadex.org as PDF or images', epilog='in case of suggestions or bugs, please open an issue on the project github :\nhttps://github.com/john-erinjery/mangadex-dl')
+
+parser.add_argument('-v', '--version', action="version",
+                    version=f'mangadex-dl {VERSION}')
+parser.add_argument('-t', '--manga-url', action='store',
+                    help='the manga homepage url', type=str, dest='manga_url', metavar='')
+parser.add_argument('-c', '--chapter-url',
+                    help='the chapter url', dest='chapter_url', metavar='')
+parser.add_argument('-pdf', help='organise manga into chapterwise PDFs',
+                    dest='pdf', action='store_true', default=False)
+parser.add_argument('-m', '--merge', help="merge chapter PDFs into single PDF (-pdf must be provided)",
+                    dest='merge', action='store_true', default=False)
+parser.add_argument('-img', help="organise manga into chapterwise image folders",
+                    dest='img', action='store_true', default=False)
+parser.add_argument('-s', '--single-folder', help="organise manga into chapterwise image folders (-img must be provided)",
+                    dest='single_folder', action='store_true', default=False)
+parser.add_argument('--data', help='enable data saver (default)',
+                    action='store_true', dest='data_saver', default=True)
+parser.add_argument('-r', '--range', action='extend', nargs=2,
+                    help='range of chapters to download, eg: -r 1 5 (download chapters 1 - 4)', dest='range', metavar='', type=int)
+parser.add_argument('-tl', '--translated-language', action='store', default='en',
+                    help='language code of translation (default : en, others availiable on github homepage)', metavar='', dest='tl')
+arg_dict = dict(parser.parse_args()._get_kwargs())
 
 
 def main():
     '''
     Main Entry Point of the CLI
     '''
-    if arg_dict != None:
-        pass
-    else:
-        return
-
     organiser = Organiser(args_dict=arg_dict)
 
-    if organiser.args_evaluvator():
-        folder_name = 'manga' + str(randint(10000, 99999))
-        os.mkdir(folder_name)
-        os.chdir(folder_name)
+    if not organiser.args_evaluvator():
+        sys.exit()
 
-        if organiser.pdf:
-
-            if organiser.chapter_url != None:
-                chapter = MangaChapter(organiser.chapter_url)
-                print(
-                    f'\nStarting download of Chapter {chapter.chapter_number} : {chapter.chapter_name}')
-                print(
-                    f'initialising download in folder : {os.getcwd()}')
-
-                ret = chapter.download_chapter(organiser.data_saver)
-                if ret == 1:
-                    ch_img_path_dict = eval(
-                        open('all_images_paths_ch_dict.txt').read())
-                    organiser.convert_chapter_images_to_pdf(ch_img_path_dict)
-                    os.rename(f'pdf/{chapter.chapter_number}.pdf',
-                              f'../Chapter {chapter.chapter_number}.pdf')
-                    print('deleting cache and temp folder..')
-                    os.chdir('..')
-                    rmtree(folder_name)
-                    print('done!')
-
-                else:
-                    sleep(5.0)
-                    ret = chapter.download_chapter(organiser.data_saver)
-                    if ret != 1:
-                        print(
-                            'ERROR: Could not download chapter. Check your network connection and try again later.')
-
-            else:
-                manga = Manga(organiser.manga_url, translation=organiser.tl)
-                if manga.title != '':
-                    print('\nStarting download of {}..'.format(manga.title))
-
-                print('initialising download in folder : {}'.format(os.getcwd()))
-                print('getting chapters and volumes..')
-                ch_dict = manga.get_chapter_dict(organiser.range_)
-                for i in ch_dict:
-                    chapter = MangaChapter(
-                        'https://mangadex.org/chapter/{}'.format(ch_dict[i]))
-                    status = chapter.download_chapter(organiser.data_saver)
-                    if status != 0:
-                        ch_images = None
-                        with open('all_images_paths_ch_dict.txt') as f:
-                            all_images_paths_ch_dict = eval(f.read())
-                        for j in all_images_paths_ch_dict:
-                            if str(i) == str(j):
-                                ch_images = {
-                                    str(i): all_images_paths_ch_dict[str(i)]}
-                                organiser.convert_chapter_images_to_pdf(
-                                    ch_images)
-                    else:
-                        print('\nconverting downloaded chapters to pdf..')
-                        rmtree(i)
-                        break
-                if organiser.merge:
-                    organiser.pdf_merger()
-                else:
-                    os.rename(
-                        'pdf', f'../Chapter {organiser.range_[0]}-{organiser.range_[1]}')
-                print('\ndeleting cache and temp folder..')
-                os.chdir('..')
-                rmtree(folder_name)
-                print('done!')
+    folder_name = 'manga' + str(randint(10000, 99999))
+    os.mkdir(folder_name)
+    os.chdir(folder_name)
+
+    if organiser.chapter_url != None:
+        chp = MangaChapter(organiser.chapter_url)
+        if chp.chapter_name != None:
+            print(
+                f'\nStarting download of Chapter {chp.chapter_number} : {chp.chapter_name}')
+        print(
+            f'initialising download in folder : {os.getcwd()}')
 
+        chp.download_chapter(organiser.data_saver)
+        if organiser.pdf:
+            ch_img_dict = eval(open('all_images_paths_ch_dict.txt').read())
+            organiser.convert_chapter_images_to_pdf(ch_img_dict)
+            os.rename(f'pdf/{chp.chapter_number}.pdf',
+                      f'../Chapter {chp.chapter_number}.pdf')
         else:
-
-            if organiser.chapter_url != None:
-                chapter = MangaChapter(organiser.chapter_url)
-                print(
-                    f'\nStarting download of Chapter {chapter.chapter_number} : {chapter.chapter_name}')
-                print(
-                    f'initialising download in folder : {os.path.join(os.getcwd(), folder_name)}')
-                chapter.download_chapter(organiser.data_saver)
-                for i in os.listdir('.'):
-                    if os.path.isdir(i):
-                        print('Organising image folder..')
-                        os.rename(i, f'../Chapter {i}')
-                print('deleting cache and temp folders..')
-                os.chdir('..')
-                rmtree(folder_name)
-                print('done!')
-
+            os.rename(str(chp.chapter_number),
+                      f'../Chapter {chp.chapter_number}')
+        print('deleting cache and temp folder..')
+        os.chdir('..')
+        rmtree(folder_name)
+        print('done!')
+        sys.exit()
+
+    manga = Manga(organiser.manga_url, translation=organiser.tl)
+    if manga.title:
+        print('\nStarting download of {}..'.format(manga.title))
+    print('initialising download in folder : {}'.format(os.getcwd()))
+    print('getting chapters and volumes..')
+    ch_dict = manga.get_chapter_dict(organiser.range_)
+
+    for i in ch_dict:
+        chapter = MangaChapter(
+            'https://mangadex.org/chapter/{}'.format(ch_dict[i]))
+
+        try:
+            all_ch_imgs_dict = chapter.download_chapter(organiser.data_saver)
+        except:
+            if organiser.pdf:
+                print('\nconverting downloaded chapters to pdf..')
             else:
+                organiser.range_[1] = float(i) - 1.0
+                print('organising downloaded image folders..')
+            rmtree(i)
+            break
 
-                manga = Manga(organiser.manga_url, translation=organiser.tl)
-                print('\nStarting download of {}..'.format(manga.title))
-                print('initialising download in folder : {}'.format(os.getcwd()))
-                print('getting chapters and volumes..')
-                ch_dict = manga.get_chapter_dict(organiser.range_)
-                for i in ch_dict:
-                    chapter = MangaChapter(
-                        'https://mangadex.org/chapter/{}'.format(ch_dict[i]))
-                    status = chapter.download_chapter(organiser.data_saver)
-                    if status != 0:
-                        pass
-                    else:
-                        organiser.range_[1] = float(i) - 1.0
-                        print('organising downloaded image folders..')
-                        break
-
-                print('Organising Image folders..')
-                if organiser.single_folder:
-                    organiser.single_folder_images()
-                    os.rename(
-                        'imgs', f'../Chapter {organiser.range_[0]}-{organiser.range_[1]}')
-                else:
-                    for i in os.listdir('.'):
-                        if os.path.isfile(i):
-                            os.remove(i)
-                    os.chdir('..')
-                    os.rename(
-                        folder_name, f'Chapter {organiser.range_[0]}-{organiser.range_[1]}')
-                print('done!')
+        if organiser.pdf:
+            organiser.convert_chapter_images_to_pdf(all_ch_imgs_dict)
+    if organiser.pdf:
+        if organiser.merge:
+            organiser.pdf_merger()
+        else:
+            os.rename(
+                'pdf', f'../chapter {organiser.range_[0]}-{organiser.range_[1]}')
+    if organiser.img:
+        if organiser.single_folder:
+            organiser.single_folder_images()
+            os.rename(
+                'imgs', f'../chapter {organiser.range_[0]}-{organiser.range_[1]}')
+        else:
+            print('organising image folders..')
+            for i in os.listdir('.'):
+                if os.path.isfile(i):
+                    os.remove(i)
+            os.chdir('..')
+            os.rename(
+                folder_name, f'Chapter {organiser.range_[0]}-{organiser.range_[1]}')
+            print('done!')
+            sys.exit()
+    print('deleting cache and temp folders..')
+    os.chdir('..')
+    rmtree(folder_name)
+    print('done!')
 
 
 if __name__ == '__main__':
     main()
```

## mangadex_dl/constants.py

```diff
@@ -1,4 +1,4 @@
-VERSION = '2.1.0'
+VERSION = '3.0.0'
 LANGUAGE_CODES = {'sa': 'Arabic', 'bd': 'Bengali', 'bg': 'Bulgarian', 'mm': 'Burmese', 'ct': 'Catalan', 'cz': 'Czech', 'dk': 'Danish', 'nl': 'Dutch', 'en': 'English', 'ph': 'Filipino', 'fi': 'Finnish', 'fr': 'French', 'de': 'German', 'gr': 'Greek', 'il': 'Hebrew', 'in': 'Hindi', 'hu': 'Hungarian', 'id': 'Indonesian', 'it': 'Italian',
                   'ja': 'Japanese', 'kr': 'Korean', 'lt': 'Lithuanian', 'my': 'Malay', 'mn': 'Mongolian', 'ir': 'Persian', 'pl': 'Polish', 'br': 'Portuguese (Br)', 'pt': 'Portuguese (Pt)', 'ro': 'Romanian', 'ru': 'Russian', 'rs': 'Serbo-Croatian', 'es': 'Spanish (Es)', 'mx': 'Spanish (LATAM)', 'se': 'Swedish', 'th': 'Thai', 'tr': 'Turkish',
                   'ua': 'Ukrainian', 'vn': 'Vietnames', 'zh': 'Simplified Chinese', 'zh-hk': 'Traditional Chinese', 'pt-br': 'Brazilian Portugese', 'es-la': 'Latin American Spanish', 'ja-ro': 'Romanized Japanese', 'ko-ro': 'Romanized Korean', 'zh-ro': 'Romanized Chinese'}
```

## mangadex_dl/helper.py

```diff
@@ -1,226 +1,28 @@
-#!env python
-'''
-MangaDex-dl CLI
-
-This Command Line Client uses the ManagDex API to download manga
-and store it in image or PDF format.
-
-You can choose whether to have the software merge all the chapters
-downloaded into a single PDF, or have it in Chapterwise PDFs
-
-If you choose to download manga in image format, you can choose
-whether to save it in chapterwise folders or as a single large folder.
-- this option is made to make it more convinient for readers to scroll
-  through and read manga
-- another feature is that if the files are named in a format that
-  Andriod phones and PC's will be able to sort easily.
-- it names files in the format aaa-1.jpg, aab-2.jpg...ect.
-  if not, the file order will be quite messed up
-
-This software is completely open source.
-Feel free to use it as you like!
-
-'''
-from mangadex_dl.constants import VERSION
-abc = 'abcdefghijklmnopqrstuvwxyz'
-
-
-def make_sortable(stack):
-    lenght = len(stack)
-    prefixes = name_gen(lenght)
-    result_stack = []
-    for i in range(lenght):
-        result_stack.append(prefixes[i] + '-' + str(stack[i]))
-    return result_stack
+import itertools
+from string import ascii_lowercase as abc
+import os
 
 
 def name_gen(lenght):
-    n1 = 0
-    n2 = 0
-    n3 = 0
-    name_list = []
-    while n1 < 26:
-        while n2 < 26:
-            while (n3 < 26) and (len(name_list) < lenght):
-                name_list.append(abc[n1] + abc[n2] + abc[n3])
-                n3 += 1
-            n2 += 1
-            n3 = 0
-        n1 += 1
-        n2 = 0
-        n3 = 0
-    return name_list
-
-
-def ret_float_or_int(num):
-    if '.' in num:
-        if (num.split('.')[1] != '0') and (num.split('.')[1] != '00'):
-            return float(num)
-        else:
-            return int(num.split('.')[0])
-    else:
-        try:
-            return int(num)
-        except:
-            return False
-
-
-def path_prettify(path: str):
-    new_path = path.replace('/', '\\')
-    return new_path
-
-
-help_dict = {
-    'general,': '''
-MangaDex-dl CLI, a manga download software powered by MangaDex API
-Usage : mangadex_dl [OPTION]
-
-Startup:
-    -h, --help              print this help message and exit
-    -V, --version           display the version of MangaDex-dl
-
-Download:
-    -t, --manga-url                 the mangadex manga url (url is title page url)
-    -c, --chapter-url               the mangadex chapter url (url is chapter url) (currently unavailiable)
-    -r, --range                     the range of chapters to download. (if manga url provided)
-    -pdf                            download manga as chapterwise pdfs (default)
-    -img                            download manga as chapterwise images
-    --data                          download manga in high quality
-    -tl, --translated-language      the language code for managdex translations, run mangadex_dl --help -tl for more info
-
-Post-Download-Processing:
-    -m, --merge-pdf         merges all chapter pdfs into one file
-    -s, --single-folder     collect all images into a single folder
-
-for more information about an option,
-Run mangadex_dl --help <option>
-
-in case of bugs/issues/discussions please open an issue at
-https://github.com/john-erinjery/mangadex-dl
-''',
-    '-h,--help': '''
-MangaDex-dl CLI, a manga download software powered by MangaDex API
-Usage : mangadex_dl [OPTION]
-
-Startup:
-    -h, --help              print this help message and exit
-    -V, --version           display the version of MangaDex-dl
-
-Download:
-    -t, --manga-url                 the mangadex manga url (url is title page url)
-    -c, --chapter-url               the mangadex chapter url (url is chapter url)
-    -r, --range                     the range of chapters to download. (if manga url provided)
-    -pdf                            download manga as chapterwise pdfs (default)
-    -img                            download manga as chapterwise images
-    --data                          download manga in high quality
-    -tl, --translated-language      the language code for managdex translations, run mangadex_dl --help -tl for more info (default en)
-
-Post-Download-Processing:
-    -m, --merge-pdf         merges all chapter pdfs into one file
-    -s, --single-folder     collect all images into a single folder
-
-for more information about an option,
-Run mangadex_dl --help <option>
-
-in case of bugs/issues/discussions please open an issue at
-https://github.com/john-erinjery/mangadex-dl
-''',
-    '-V,--version': f'current version of MangaDex-dl is {VERSION}',
-    '-t,--manga-url': '\nThe MangaDex manga homepage url.\nNote that this is different from the chapter url. Manga URLs are of the form:\n\nhttps://mangadex.org/title/<manga-id>/<manga-name>\n\nfor eg: https://mangadex.org/title/9417ab7d-b231-4481-8279-34a873cc820f/chicchai-senpai-ga-kawaisugiru',
-    '-c,--chapter-url': '\nThe MangaDex chapter url\nNote that this is different from the manga url. Chapter URLs are of the form:\n\nhttps://mangadex.org/chapter/<chapter-id>\n\nfor eg: https://mangadex.org/chapter/23deab8b-8866-401a-925d-115788a0027c',
-    '-r,--range': 'The chapter range to be downloaded. Use only when providing Manga URLs.\n\nFormat : -r/--range <chapter-start> <chapter-end>\n\nTo download a single chapter pass the same value twice eg: --range 100 100',
-    '-pdf': 'Downloads manga as chapter-wise pdfs. Output will be a folder "pdf" containing pdf files of the chapters.',
-    '-img': 'Downloads mangs as chapter-wise image folders. Output will be an "imgs" folder containing image chapter folders',
-    '-s,--single-folder': 'Option only availiable when downloading as image files. All images will be sorted and stored in a single folder.',
-    '-m,--merge-pdf': 'Option only availiable when downloading as pdf files. All pdfs will be merged into a single pdf.',
-    '--data': 'downloads manga in higher quality. note that the program might become slower with this option.',
-    '-tl,--translated-language': 'the language code for managdex translations.\nall codes availiable here : https://github.com/john-erinjery/mangadex-dl#codes'
-}
-
-
-def help_(func='general'):
-    help_dict_ops = []
-    help_dict_all_ops = []
-    for i in help_dict.keys():
-        help_dict_ops.append(i.split(','))
-        for j in i.split(','):
-            if j != '':
-                help_dict_all_ops.append(j)
-    if func not in help_dict_all_ops:
-        print('ERROR : Invalid Option')
-    else:
-        for i in help_dict_ops:
-            if func in i:
-                print(help_dict[list(help_dict.keys())
-                                [help_dict_ops.index(i)]])
+    return [w for w in (''.join(word) for word in itertools.product(abc, repeat=3))][:lenght]
 
 
 def obj_at_next_index(obj, stack, steps=1):
-    index = stack.index(obj) + 1
-    if steps == 1:
-        return stack[index]
-    else:
-        return stack[index: index + steps]
+    index = stack.index(obj) + steps
+    return stack[index]
 
 
-def get_arguments(args):
-    manga_url = None
-    chapter_url = None
-    range_ = []
-    range_1 = []
-    pdf = True
-    img = False
-    merge = False
-    single_folder = False
-    data_saver = True
-    tl = 'en'
-    if len(args) == 1:
-        help_()
-        return None
-    elif len(args) == 2:
-        if args[-1] == '-V' or args[-1] == '--version':
-            help_('-V')
-            return None
-        elif args[-1] == '-h' or args[-1] == '--help':
-            help_()
-            return None
-        else:
-            print('ERROR: Invalid Syntax')
-            return None
-    elif len(args) == 3 and (('--help' in args) or ('-h' in args)):
-        help_(args[-1])
-        return None
+def update_file(file_path, obj, _type):
+    if os.path.exists(file_path):
+        with open(file_path) as f:
+            data = eval(f.read())
+        with open(file_path, 'w') as f:
+            if _type == 'dict':
+                data.update(obj)
+                f.write(str(data))
+            elif _type == 'list':
+                data.extend(obj)
+                f.write(str(data))
     else:
-        for i in args[1:]:
-            if i == '-t' or i == '--manga-url':
-                manga_url = obj_at_next_index(i, args)
-            elif i == '-c' or i == '--chapter-url':
-                chapter_url = obj_at_next_index(i, args)
-            elif i == '-tl' or i == '--translated-launguage':
-                tl = obj_at_next_index(i, args)
-            elif i == tl:
-                continue
-            elif i == '-r' or i == '--range':
-                range_1 = obj_at_next_index(i, args, 2)
-                for i in range_1:
-                    range_.append(ret_float_or_int(i))
-                range_.sort()
-            elif i == '-pdf':
-                continue
-            elif i == '-img':
-                pdf = False
-                img = True
-            elif i == '-m' or i == '--merge-pdf':
-                merge = True
-            elif i == '--data':
-                data_saver = False
-            elif i == '-s' or i == '--single-folder':
-                single_folder = True
-            elif i in range_1:
-                continue
-            elif i == manga_url or i == chapter_url:
-                continue
-            else:
-                print('ERROR: Invalid Option', i)
-                return None
-    return {'manga_url': manga_url, 'chapter_url': chapter_url, 'range': range_, 'pdf': pdf, 'img': img, 'merge': merge, 'single_folder': single_folder, 'data_saver': data_saver, 'tl': tl}
+        with open(file_path, 'w') as f:
+            f.write(str(obj))
```

## mangadex_dl/manga.py

```diff
@@ -1,53 +1,30 @@
-from mangadex_dl.helper import ret_float_or_int
-import mangadex
-api = mangadex.Api()
-
-
-class Manga:
-    def __init__(self, _url, translation) -> None:
-        self.url = _url
-        self.tl = translation
-        self.id = self.url.split('/')[-2]
-        self.title = self.name_of_manga()
-        self.chapters = self.number_of_chaps_vols()[0]()
-        self.volumes = self.number_of_chaps_vols()[1]
-
-    def name_of_manga(self):
-        try:
-            return api.view_manga_by_id(manga_id=self.id).title[self.tl]
-        except:
-            return ''
-
-    def number_of_chaps_vols(self):
-        manga_dict = api.get_manga_volumes_and_chapters(
-            manga_id=self.id, translatedLanguage=[self.tl])
-        last_volume = list(manga_dict.keys())
-
-        def chapters():
-            ch_dict = self.get_chapter_dict([])
-            output = []
-            for i in ch_dict:
-                output.append(i)
-            return output
-        return chapters, last_volume
-
-    def get_chapter_dict(self, range_=[]):
-        manga_dict = api.get_manga_volumes_and_chapters(
-            manga_id=self.id, translatedLanguage=[self.tl])
-        chapters_dict_ = {}
-        for i in dict(manga_dict).keys():
-            chapters_dict_.update(manga_dict[i]['chapters'])
-        all_chapter_dict = {}
-        for i in chapters_dict_:
-            all_chapter_dict[i] = chapters_dict_[i]['id']
-        if range_ == []:
-            return all_chapter_dict
-        all_ch_keys = list(float(x)
-                           for x in all_chapter_dict.keys())
-        all_ch_keys.sort()
-        ch_dict = {}
-        for i in all_ch_keys:
-            if i >= range_[0] and i < range_[1]:
-                ch_dict[str(i)] = all_chapter_dict[str(
-                    ret_float_or_int(str(i)))]
-        return ch_dict
+import mangadex
+api = mangadex.Api()
+
+
+class Manga:
+    def __init__(self, _url, translation) -> None:
+        self.url = _url
+        self.tl = translation
+        self.id = self.url.split('/')[-2]
+        self.title = self.name_of_manga()
+
+    def name_of_manga(self):
+        try:
+            return api.view_manga_by_id(manga_id=self.id).title[self.tl]
+        except:
+            return ''
+
+    def get_chapter_dict(self, range_) -> dict:
+        manga_dict = api.get_manga_volumes_and_chapters(
+            manga_id=self.id, translatedLanguage=[self.tl])
+        chapters_dict_ = {}
+        for i in manga_dict.keys():
+            chaps = manga_dict[i]['chapters']
+            for j in chaps:
+                floated_j = float(j)
+                if (range_[0] <= floated_j < range_[1]):
+                    chapters_dict_.update(
+                        {floated_j: chaps[j]['id']})
+        chapters_dict_ = dict(sorted(chapters_dict_.items()))
+        return chapters_dict_
```

## mangadex_dl/organiser.py

```diff
@@ -24,18 +24,18 @@
 
         if self.manga_url == self.chapter_url == None:
             print('ERROR: manga or chapter url must be provided')
             return False
         elif self.manga_url != None and self.chapter_url != None:
             print('ERROR: both manga and chapter urls should not be provided')
             return False
-        elif self.manga_url != None and self.range_ == []:
+        elif self.manga_url != None and self.range_ == None:
             print('ERROR: Range must be provided for manga urls')
             return False
-        elif self.chapter_url != None and self.range_ != []:
+        elif self.chapter_url != None and self.range_ != None:
             print('ERROR: Range should not be provided for chapter urls')
             return False
         elif self.pdf and self.img:
             print('ERROR: Manga cannot be stored as both image and pdf')
             return False
         elif self.merge and self.single_folder:
             print('ERROR: Cannot merge and single folder')
@@ -45,48 +45,48 @@
             return False
         elif self.img and self.merge:
             print('ERROR: Cannot be both img and merge')
             return False
         else:
             if self.tl not in list(lang_c.keys()):
                 print('ERROR: Invalid language code. Availiable language codes here : https://github.com/john-erinjery/mangadex-dl#codes')
+                return False
             else:
                 if self.manga_url != None:
                     if not api.get_manga_volumes_and_chapters(manga_id=self.manga_url.split('/')[-2], translatedLanguage=[self.tl]):
                         print(
                             'managdex does not have any availiable translations of this manga in', lang_c[self.tl])
+                        return False
                     else:
                         return True
+                else:
+                    return True
 
     def convert_chapter_images_to_pdf(self, ch_image_path_: dict):
         '''
         Converts the given images into pdfs and saves it in a folder 'pdf'
 
         - the argument is a single element dictionary whose key is the chapter number and value is a list contaning
           paths to the chapter images
         '''
-
-        ch_image_path = ch_image_path_
-        image_list = list(ch_image_path.values())[0]
-        image_objs = []
+        print('converting chapter to PDF..\n')
         if not os.path.exists('pdf'):
             os.mkdir('pdf')
+        image_list = list(ch_image_path_.values())[0]
+        image_objs = []
         for i in image_list:
             try:
                 image_objs.append(Image.open(str(i)).convert('RGB'))
             except:
                 print('truncination error in image {}. skipping page..'.format(
                     image_list.index(i)))
                 continue
-        print('converting chapter to PDF..\n')
-
         try:
-            image_objs[0].save('pdf/' + str(list(ch_image_path.keys())[0]) +
+            image_objs[0].save('pdf/' + str(list(ch_image_path_.keys())[0]) +
                                '.pdf', save_all=True, append_images=image_objs[1:])
-
         except UnidentifiedImageError:
             print('unidentified image detected, skipping..')
 
     def pdf_merger(self):
         '''
         Mergers all PDFs in the folder 'pdf'
```

## Comparing `mangadex_dl-2.1.0.dist-info/LICENSE` & `mangadex_dl-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mangadex_dl-2.1.0.dist-info/METADATA` & `mangadex_dl-3.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadex-dl
-Version: 2.1.0
+Version: 3.0.0
 Summary: A Python CLI that downloads manga from mangadex.org as image or PDF
 Home-page: https://github.com/john-erinjery/mangadex-dl/
 Author: John Erinjery
 Author-email: jancyvinod415@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

