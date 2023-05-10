# Comparing `tmp/jmcomic-1.9.1.tar.gz` & `tmp/jmcomic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-dzo_jz90/jmcomic-1.9.1.tar", last modified: Sat Apr 29 05:41:16 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-h6zzdcfs/jmcomic-2.0.0.tar", last modified: Wed May 10 14:07:59 2023, max compression
```

## Comparing `jmcomic-1.9.1.tar` & `jmcomic-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 05:41:07.000000 jmcomic-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-29 05:41:16.000000 jmcomic-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-29 05:41:07.000000 jmcomic-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:41:16.000000 jmcomic-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-29 05:41:07.000000 jmcomic-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-29 05:41:07.000000 jmcomic-1.9.1/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 05:41:16.000000 jmcomic-1.9.1/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 14:07:44.000000 jmcomic-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-10 14:07:59.000000 jmcomic-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-10 14:07:44.000000 jmcomic-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:07:59.000000 jmcomic-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 14:07:44.000000 jmcomic-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.9.1/LICENSE` & `jmcomic-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.1/PKG-INFO` & `jmcomic-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.9.1
+Version: 2.0.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-1.9.1/README.md` & `jmcomic-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.1/setup.py` & `jmcomic-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.9.1/src/jmcomic/api.py` & `jmcomic-2.0.0/src/jmcomic/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,46 +9,43 @@
     @param option: 下载选项，为空默认是 JmOption.default()
     """
 
     if not isinstance(jm_album_id, (str, int)):
         return download_album_batch(jm_album_id, option)
 
     option, jm_client = build_client(option)
-    album_detail: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
+    album: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
 
-    jm_debug('download_album',
-             f'获得album_detail成功，准备下载。'
-             f'本子作者是【{album_detail.author}】，一共有{len(album_detail)}集本子')
-
-    def download_photo(index: int,
-                       photo_detail: JmPhotoDetail,
-                       debug_topic='download_album_photo',
+    jm_debug('album',
+             f'本子获取成功: [{album.id}], '
+             f'标题: [{album.title}], '
+             f'作者: [{album.author}], '
+             f'章节数: [{len(album)}]')
+
+    def download_photo(photo: JmPhotoDetail,
+                       debug_topic='photo',
                        ):
-        jm_client.ensure_photo_can_use(photo_detail)
+        jm_client.ensure_photo_can_use(photo)
 
         jm_debug(debug_topic,
-                 f"下载第[{index + 1}]集: "
-                 f"图片数为[{len(photo_detail)}]，"
-                 f"标题为：({photo_detail.title}) "
-                 f"-- photo {photo_detail.photo_id}")
-
-        download_by_photo_detail(
-            photo_detail,
-            option,
-        )
+                 f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}]), '
+                 f'标题: [{photo.title}], '
+                 f'图片数为[{len(photo)}]')
 
-        jm_debug(debug_topic,
-                 f"下载完成：({photo_detail.title}) "
-                 f"-- photo {photo_detail.photo_id}")
+        download_by_photo_detail(photo, option)
+
+        jm_debug(debug_topic, f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}])')
 
     thread_pool_executor(
-        iter_objs=enumerate(album_detail),
+        iter_objs=album,
         apply_each_obj_func=download_photo,
     )
 
+    jm_debug('album', f'本子下载完成: [{album.id}]')
+
 
 def download_album_batch(jm_album_id_iter: Union[Iterable, Generator],
                          option=None,
                          wait_finish=True,
                          ) -> List[Thread]:
     """
     批量下载album，每个album一个线程，使用的是同一个option。
@@ -84,54 +81,53 @@
     下载一个本子的一章，根据 photo_detail
     @param photo_detail: 本子章节信息
     @param option: 选项
     """
     option, jm_client = build_client(option)
 
     # 下载准备
-    use_cache = option.download_use_disk_cache
-    decode_image = option.download_image_then_decode
+    use_cache = option.download_cache
+    decode_image = option.download_image_decode
     jm_client.ensure_photo_can_use(photo_detail)
 
     # 下载每个图片的函数
-    def download_image(index, img_detail, debug_topic='download_images_of_photo'):
+    def download_image(index, image: JmImageDetail, debug_topic='image'):
         img_save_path = option.decide_image_filepath(photo_detail, index)
 
         # 已下载过，缓存命中
         if use_cache is True and file_exists(img_save_path):
-            jm_debug(debug_topic, f'photo-{img_detail.aid}: '
-                                  f'图片{img_detail.filename}已下载过，'
-                                  f'命中磁盘缓存（{img_save_path}）')
+            jm_debug(debug_topic,
+                     f'图片已存在: {image.aid}[{image.filename}] → {img_save_path}')
             return
 
         # 开始下载
         jm_client.download_by_image_detail(
-            img_detail,
+            image,
             img_save_path,
             decode_image=decode_image,
         )
 
-        jm_debug(debug_topic, f'photo-{img_detail.aid}: '
-                              f'图片{img_detail.filename}下载完成：'
-                              f'[{img_detail.img_url}] → [{img_save_path}]')
+        jm_debug(debug_topic,
+                 f'图片下载完成: {image.aid}/{image.filename}, '
+                 f'[{image.img_url}] → [{img_save_path}]')
 
     length = len(photo_detail)
     # 根据图片数，决定下载策略
-    if length <= option.download_multi_thread_photo_len_limit:
+    if length <= option.download_threading_batch_count:
         # 如果图片数小的话，直接使用多线程下载，一张图一个线程。
         multi_thread_launcher(
             iter_objs=enumerate(photo_detail),
             apply_each_obj_func=download_image,
         )
     else:
         # 如果图片数多的话，还是分批下载。
         multi_task_launcher_batch(
             iter_objs=enumerate(photo_detail),
             apply_each_obj_func=download_image,
-            batch_size=option.download_multi_thread_photo_batch_count
+            batch_size=option.download_threading_batch_count
         )
 
 
 def build_client(option: Optional[JmOption]) -> Tuple[JmOption, JmcomicClient]:
     """
     处理option的判空，并且创建jm_client
     """
@@ -139,9 +135,9 @@
         option = JmOption.default()
 
     jm_client = option.build_jm_client()
     return option, jm_client
 
 
 def create_option(filepath: str) -> JmOption:
-    option = JmOption.create_from_file(filepath)
+    option = JmOption.from_file(filepath)
     return option
```

### Comparing `jmcomic-1.9.1/src/jmcomic/jm_client.py` & `jmcomic-2.0.0/src/jmcomic/jm_client_impl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,128 @@
-from .jm_toolkit import *
+from .jm_client_interface import *
 
 
-class JmcomicClient(PostmanProxy):
-    retry_postman_type = RetryPostman
+class AbstractJmClient(
+    JmcomicClient,
+    PostmanProxy,
+):
+
+    def __init__(self,
+                 postman: Postman,
+                 retry_times: int,
+                 domain=None,
+                 fallback_domain_list=None,
+                 ):
+        super().__init__(postman)
+        self.retry_times = retry_times
+
+        if fallback_domain_list is None:
+            fallback_domain_list = []
+
+        if domain is not None:
+            fallback_domain_list.insert(0, domain)
+
+        self.domain_list = fallback_domain_list
+
+    def get(self, url, **kwargs):
+        return self.request_with_retry(self.postman.get, url, **kwargs)
+
+    def post(self, url, **kwargs):
+        return self.request_with_retry(self.postman.post, url, **kwargs)
+
+    def of_api_url(self, api_path, domain):
+        return f'{JmModuleConfig.PROT}{domain}{api_path}'
+
+    def request_with_retry(self,
+                           request,
+                           url,
+                           domain_index=0,
+                           retry_count=0,
+                           **kwargs,
+                           ):
+        if domain_index >= len(self.domain_list):
+            raise AssertionError("All domains failed.")
+
+        domain = self.domain_list[domain_index]
+
+        if not url.startswith(JmModuleConfig.PROT):
+            url = self.of_api_url(url, domain)
+            jm_debug('api', url)
+
+        if domain_index != 0 and retry_count != 0:
+            jm_debug(
+                f'请求重试',
+                ', '.join([
+                    f'次数: [{retry_count + 1}/{self.retry_times}]',
+                    f'域名: [{domain} ({domain_index}/{len(self.domain_list)})]',
+                    f'路径: [{url}]',
+                    f'参数: [{kwargs if "login" not in url else "#login_form#"}]'
+                ])
+            )
 
-    def __init__(self, postman: Postman, domain, retry_times=None):
-        super().__init__(postman.with_retry(retry_times or 5, self.retry_postman_type))
-        self.domain = domain
-
-    def download_image(self,
-                       data_original: str,
-                       img_save_path: str,
-                       scramble_id: str,
-                       photo_id: str = None,
-                       decode_image=True,
-                       ):
-        """
-        下载JM的图片
-        @param data_original: 图片url
-        @param img_save_path: 图片保存位置
-        @param scramble_id: 图片所在photo的scramble_id
-        @param photo_id: 图片所在photo的photo_id，可为空
-        @param decode_image: 要保存的是解密后的图还是原图
-        """
-        # 请求图片
-        resp = self.jm_get(data_original, is_api=False)
+        try:
+            return request(url, **kwargs)
+        except Exception as e:
+            self.before_retry(e, kwargs, retry_count, url)
+
+            if retry_count < self.retry_times:
+                return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
+            else:
+                return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
+
+    # noinspection PyMethodMayBeStatic, PyUnusedLocal
+    def before_retry(self, e, kwargs, retry_count, url):
+        jm_debug('error', str(e))
 
-        if self.is_empty_image(resp):
-            raise AssertionError(f'接收到的图片数据为空: {resp.url}')
+    def enable_cache(self, debug=False):
+        def wrap_func_cache(func_name, cache_dict_name):
+            if hasattr(self, cache_dict_name):
+                return
 
-        # gif图无需加解密，需要最先判断
-        if self.img_is_not_need_to_decode(data_original, resp):
-            JmImageSupport.save_resp_img(resp, img_save_path, False)
-            return
+            cache_dict = {}
+            setattr(self, cache_dict_name, cache_dict)
 
-        # 不解密图片，直接返回
-        if decode_image is False:
-            # 保存图片
-            JmImageSupport.save_resp_img(
-                resp,
-                img_save_path,
-                need_convert=suffix_not_equal(data_original, img_save_path),
-            )
+            # 重载本对象的方法
+            func = getattr(self, func_name)
 
-        JmImageSupport.save_resp_decoded_img(
-            resp=resp,
-            img_detail=JmImageDetail.of(
-                photo_id or JmcomicText.parse_to_photo_id(data_original),
-                scramble_id,
-                data_original,
-            ),
-            filepath=img_save_path
-        )
+            cache_hit_msg = f'【缓存命中】{cache_dict_name} ' + '→ [{}]' if debug is True else None
+            cache_miss_msg = f'【缓存缺失】{cache_dict_name} ' + '← [{}]' if debug is True else None
 
-    def download_by_image_detail(self,
-                                 img_detail: JmImageDetail,
-                                 img_save_path,
-                                 decode_image=True,
-                                 ):
-        self.download_image(
-            img_detail.img_url,
-            img_save_path,
-            img_detail.scramble_id,
-            photo_id=img_detail.aid,
-            decode_image=decode_image,
-        )
+            wrap_func = enable_cache(
+                cache_dict=cache_dict,
+                cache_hit_msg=cache_hit_msg,
+                cache_miss_msg=cache_miss_msg,
+            )(func)
+
+            setattr(self, func_name, wrap_func)
+
+        wrap_func_cache('get_photo_detail', 'album_cache_dict')
+        wrap_func_cache('get_album_detail', 'photo_cache_dict')
+        wrap_func_cache('search_album', 'search_album_cache_dict')
 
-    # -- get detail（返回值是实体类） --
+
+# 基于网页实现的JmClient
+class JmHtmlClient(AbstractJmClient):
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         # 参数校验
         album_id = JmcomicText.parse_to_photo_id(album_id)
 
         # 请求
-        resp = self.jm_get(f"/album/{album_id}")
+        resp = self.get_jm_html(f"/album/{album_id}")
 
         # 用 JmcomicText 解析 html，返回实体类
         return JmcomicText.analyse_jm_album_html(resp.text)
 
     def get_photo_detail(self, photo_id: str, album=True) -> JmPhotoDetail:
         # 参数校验
         photo_id = JmcomicText.parse_to_photo_id(photo_id)
 
         # 请求
-        resp = self.jm_get(f"/photo/{photo_id}")
+        resp = self.get_jm_html(f"/photo/{photo_id}")
 
         # 用 JmcomicText 解析 html，返回实体类
         photo_detail = JmcomicText.analyse_jm_photo_html(resp.text)
 
         # 一并获取该章节的所处本子
         if album is True:
             photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
@@ -101,100 +136,30 @@
 
         # 检查 page_arr 和 data_original_domain
         if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
             new = self.get_photo_detail(photo_detail.photo_id, False)
             new.from_album = photo_detail.from_album
             photo_detail.__dict__.update(new.__dict__)
 
-    # -- search --
-
-    def search_album(self, search_query, main_tag=0) -> JmSearchPage:
+    def search_album(self, search_query, main_tag=0):
         params = {
             'main_tag': main_tag,
             'search_query': search_query,
         }
 
-        resp = self.jm_get('/search/photos', params=params)
-
-        return JmSearchSupport.analyse_jm_search_html(resp.text)
-
-    # -- 对象方法 --
-
-    def of_api_url(self, api_path):
-        return f"{JmModuleConfig.PROT}{self.domain}{api_path}"
-
-    def jm_get(self, url, is_api=True, require_200=True, **kwargs):
-        """
-        向禁漫发请求的统一入口
-        """
-        url = self.of_api_url(url) if is_api is True else url
-        if is_api is True:
-            jm_debug("api", url)
-
-        resp = self.get(url, **kwargs)
-
-        if require_200 is True and resp.status_code != 200:
-            write_text('./resp.html', resp.text)
-            raise AssertionError(f"请求失败，"
-                                 f"响应状态码为{resp.status_code}，"
-                                 f"URL=[{resp.url}]，"
-                                 +
-                                 (f"响应文本=[{resp.text}]" if len(resp.text) < 50 else
-                                  f'响应文本过长(len={len(resp.text)})，不打印')
-                                 )
-        # 图片请求，直接返回
-        if is_api is False:
-            return resp
-
-        # 检查请求是否成功
-        self.require_resp_success_else_raise(resp, url)
-
-        return resp
-
-    # -- 类方法 --
-
-    @classmethod
-    def is_empty_image(cls, resp):
-        return resp.status_code != 200 or len(resp.content) == 0
-
-    @classmethod
-    def img_is_not_need_to_decode(cls, data_original: str, _resp):
-        return data_original.endswith('.gif')
-
-    # noinspection PyAttributeOutsideInit
-    def enable_cache(self, debug=False):
-        def wrap_func_cache(func_name, cache_dict_name):
-            if hasattr(self, cache_dict_name):
-                return
-
-            cache_dict = {}
-            setattr(self, cache_dict_name, cache_dict)
-
-            # 重载本对象的方法
-            func = getattr(self, func_name)
-
-            cache_hit_msg = f'【缓存命中】{cache_dict_name} ' + '→ [{}]' if debug is True else None
-            cache_miss_msg = f'【缓存缺失】{cache_dict_name} ' + '← [{}]' if debug is True else None
-
-            wrap_func = enable_cache(
-                cache_dict=cache_dict,
-                cache_hit_msg=cache_hit_msg,
-                cache_miss_msg=cache_miss_msg,
-            )(func)
-
-            setattr(self, func_name, wrap_func)
+        resp = self.get_jm_html('/search/photos', params=params, allow_redirects=True)
 
-        wrap_func_cache('get_photo_detail', 'album_cache_dict')
-        wrap_func_cache('get_album_detail', 'photo_cache_dict')
+        # 检查是否发生了重定向
+        # 因为如果搜索的是禁漫车号，会直接跳转到本子详情页面
+        if resp.redirect_count != 0 and '/album/' in resp.url:
+            return JmcomicText.analyse_jm_album_html(resp.text)
+        else:
+            return JmSearchSupport.analyse_jm_search_html(resp.text)
 
-    def get_jmcomic_url(self, postman=None):
-        return JmModuleConfig.get_jmcomic_url(postman or self)
-
-    def get_jmcomic_url_all(self, postman=None):
-        return JmModuleConfig.get_jmcomic_url_all(postman or self)
+    # -- 帐号管理 --
 
     def login(self,
               username,
               password,
               refresh_client_cookies=True,
               id_remember='on',
               login_remember='on',
@@ -204,42 +169,118 @@
             'username': username,
             'password': password,
             'id_remember': id_remember,
             'login_remember': login_remember,
             'submit_login': '',
         }
 
-        resp = self \
-            .get_root_postman() \
-            .post(self.of_api_url('/login'),
-                  data=data,
-                  allow_redirects=False,
-                  )
+        resp = self.post('/login',
+                         data=data,
+                         allow_redirects=False,
+                         )
 
         if resp.status_code != 301:
             raise AssertionError(f'登录失败，状态码为{resp.status_code}')
 
         if refresh_client_cookies is True:
             self['cookies'] = resp.cookies
 
         return resp
 
+    def get_jm_html(self, url, require_200=True, **kwargs):
+        """
+        请求禁漫网页的入口
+        """
+        resp = self.get(url, **kwargs)
+
+        if require_200 is True and resp.status_code != 200:
+            write_text('./resp.html', resp.text)
+            self.check_special_http_code(resp.status_code, url)
+            raise AssertionError(f"请求失败，"
+                                 f"响应状态码为{resp.status_code}，"
+                                 f"URL=[{resp.url}]，"
+                                 + (f"响应文本=[{resp.text}]" if len(resp.text) < 50 else
+                                    f'响应文本过长(len={len(resp.text)})，不打印')
+                                 )
+        # 检查请求是否成功
+        self.require_resp_success_else_raise(resp)
+
+        return resp
+
+    def get_jm_image(self, img_url) -> JmImageResp:
+        return JmImageResp(self.get(img_url))
+
     @classmethod
-    def require_resp_success_else_raise(cls, resp, url):
+    def require_resp_success_else_raise(cls, resp):
         # 1. 是否 album_missing
-        if resp.url.endswith('/error/album_missing'):
-            raise AssertionError(f'请求的本子不存在！({url})\n'
+        resp_url = resp.url
+        if resp_url.endswith('/error/album_missing'):
+            raise AssertionError(f'请求的本子不存在！({resp_url})\n'
                                  '原因可能为:\n'
                                  '1. id有误，检查你的本子/章节id\n'
                                  '2. 该漫画只对登录用户可见，请配置你的cookies\n')
 
-        # 2. 是否是特殊html页
-        cls.check_special_html(resp.text.strip(), url)
+        # 2. 是否是错误html页
+        cls.check_error_html(resp.text.strip(), resp_url)
 
     @classmethod
-    def check_special_html(cls, html: str, url=None):
+    def check_error_html(cls, html: str, url=None):
         html = html.strip()
         error_msg = JmModuleConfig.JM_ERROR_RESPONSE_HTML.get(html, None)
         if error_msg is None:
             return
 
-        raise AssertionError(f'{error_msg}' + f': {url}' if url is not None else '')
+        write_text('./resp.html', html)
+        raise AssertionError(f'{error_msg}'
+                             + (f': {url}' if url is not None else ''))
+
+    @classmethod
+    def check_special_http_code(cls, code, url=None):
+        error_msg = JmModuleConfig.JM_ERROR_STATUS_CODE.get(int(code), None)
+        if error_msg is None:
+            return
+
+        raise AssertionError(f"请求失败，"
+                             f"响应状态码为{code}，"
+                             f'原因为: [{error_msg}], '
+                             + (f'URL=[{url}]' if url is not None else '')
+                             )
+
+
+class JmApiClient(AbstractJmClient):
+    API_SEARCH = '/search'
+
+    def __init__(self,
+                 base_url,
+                 postman: Postman,
+                 retry_times=5,
+                 ):
+        super().__init__(postman, retry_times)
+        self.base_url: str = base_url
+
+    def search_album(self, search_query: str, main_tag=0) -> JmApiResp:
+        return self.get(
+            self.API_SEARCH,
+            params={
+                'search_query': search_query,
+            }
+        )
+
+    def get(self, url, **kwargs) -> JmApiResp:
+        # set headers
+        headers, key_ts = self.headers_key_ts
+        kwargs.setdefault('headers', headers)
+
+        resp = super().get(url, **kwargs)
+        return JmApiResp.wrap(resp, key_ts)
+
+    @property
+    def headers_key_ts(self):
+        key_ts = time_stamp()
+        import hashlib
+        token = hashlib.md5(f"{key_ts}{JmModuleConfig.MAGIC_18COMICAPPCONTENT}".encode()).hexdigest()
+        return {
+            "token": token,
+            "tokenparam": f"{key_ts},1.5.2",
+            "user-agent": "okhttp/3.12.1",
+            "accept-encoding": "gzip",
+        }, key_ts
```

### Comparing `jmcomic-1.9.1/src/jmcomic/jm_config.py` & `jmcomic-2.0.0/src/jmcomic/jm_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+def default_jm_debug(topic: str, msg: str):
+    from common import format_ts
+    print(f'{format_ts()}:【{topic}】{msg}')
+
+
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
     _DOMAIN = None
     JM_REDIRECT_URL = f'{PROT}jm365.xyz/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
     JM_PUB_URL = f'{PROT}jmcomic1.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
@@ -9,30 +14,35 @@
 
     # 访问JM可能会遇到的异常网页
     JM_ERROR_RESPONSE_HTML = {
         "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
         "Restricted Access!": "禁漫拒绝你所在ip地区的访问，你可以选择: 换域名/换代理",
     }
 
+    JM_ERROR_STATUS_CODE = {
+        520: '520: Web server is returning an unknown error (禁漫服务器内部报错)',
+        524: '524: The origin web server timed out responding to this request. (禁漫服务器处理超时)',
+    }
+
     # 图片分隔相关
     SCRAMBLE_0 = 220980
     SCRAMBLE_10 = 268850
     SCRAMBLE_NUM_8 = 421926  # 2023-02-08后改了图片切割算法
 
+    # API的相关配置
+    MAGIC_18COMICAPPCONTENT = '18comicAPPContent'
+
     # 下载时的一些默认值
     default_author = 'default-author'
     default_photo_title = 'default-photo-title'
     default_photo_id = 'default-photo-id'
 
     # debug
     enable_jm_debug = True
-    debug_printer = print
-
-    # 缓存
-    jm_client_caches = {}
+    debug_executor = default_jm_debug
 
     @classmethod
     def domain(cls, postman=None):
         """
         由于禁漫的域名经常变化，调用此方法可以获取一个当前可用的最新的域名 domain，
         并且设置把 domain 设置为禁漫模块的默认域名。
         这样一来，配置文件也不用配置域名了，一切都在运行时动态获取。
@@ -42,15 +52,15 @@
             cls._DOMAIN = JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
 
         return cls._DOMAIN  # jmcomic默认域名
 
     @classmethod
     def headers(cls, authority=None):
         return {
-            'authority': authority or cls.domain(),
+            'authority': authority or '18comic.vip',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,'
                       'application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'zh-CN,zh;q=0.9',
             'sec-ch-ua': '"Google Chrome";v="111", "Not(A:Brand";v="8", "Chromium";v="111"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
@@ -60,17 +70,17 @@
             'upgrade-insecure-requests': '1',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 '
                           'Safari/537.36',
         }
 
     # noinspection PyUnusedLocal
     @classmethod
-    def jm_debug(cls, topic: str, msg: str, from_class=None):
+    def jm_debug(cls, topic: str, msg: str):
         if cls.enable_jm_debug is True:
-            cls.debug_printer(f'【{topic}】{msg}')
+            cls.debug_executor(topic, msg)
 
     @classmethod
     def disable_jm_debug(cls):
         cls.enable_jm_debug = False
 
     @classmethod
     def get_jmcomic_url(cls, postman=None):
@@ -84,15 +94,15 @@
 
         resp = postman.get(cls.JM_REDIRECT_URL)
         url = resp.url
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
         return url
 
     @classmethod
-    def get_jmcomic_url_all(cls, postman=None):
+    def get_jmcomic_domain_all(cls, postman=None):
         """
         访问禁漫发布页，得到所有禁漫的域名
         @return：['18comic.vip', ..., 'jm365.xyz/ZNPJam'], 最后一个是【APP軟件下載】
         """
         if postman is None:
             from common import Postmans
             postman = Postmans.get_impl_clazz('cffi').create()
```

### Comparing `jmcomic-1.9.1/src/jmcomic/jm_entity.py` & `jmcomic-2.0.0/src/jmcomic/jm_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 
     def save_file_name(self) -> str:
         def jm_type():
             # "JmAlbumDetail" -> "album"
             cls_name = self.__class__.__name__
             return cls_name[cls_name.index("m") + 1: cls_name.rfind("Detail")].lower()
 
-        return '[{}]{}{}'.format(jm_type(), self.get_id(), self.detail_save_file_suffix)
+        return '[{}]{}{}'.format(jm_type(), self.id, self.detail_save_file_suffix)
 
-    def get_id(self) -> str:
+    @property
+    def id(self) -> str:
         raise NotImplementedError
 
     def __len__(self):
         raise NotImplementedError
 
     def __getitem__(self, item) -> Union['JmAlbumDetail', 'JmPhotoDetail']:
         raise NotImplementedError
@@ -116,14 +117,15 @@
             import json
             page_arr = json.loads(page_arr)
 
         # 该photo的所有图片名 img_name
         self.page_arr: List[str] = page_arr
         # 图片域名
         self.data_original_domain: StrNone = data_original_domain
+        self.index = self.album_index
 
     @property
     def is_single_album(self) -> bool:
         return self._series_id == 0
 
     @property
     def keywords(self) -> List[str]:
@@ -187,15 +189,16 @@
             raise AssertionError(f'图片域名为空: {self.__dict__}')
 
         return f'https://{data_original_domain}/media/photos/{self.photo_id}/{img_name}'
 
     def __getitem__(self, item) -> JmImageDetail:
         return self.create_image_detail(item)
 
-    def get_id(self):
+    @property
+    def id(self):
         return self.photo_id
 
     def __len__(self):
         return len(self.page_arr)
 
 
 class JmAlbumDetail(WorkEntity):
@@ -259,15 +262,16 @@
             return self._author_list[0]
         return JmModuleConfig.default_author
 
     @property
     def keywords(self) -> List[str]:
         return self._keywords_list
 
-    def get_id(self):
+    @property
+    def id(self):
         return self.album_id
 
     def __len__(self):
         return len(self.episode_list)
 
     def __getitem__(self, item) -> JmPhotoDetail:
         return self.create_photo_detail(item)[0]
@@ -288,54 +292,16 @@
                 ret.append(episode)
 
         return ret
 
 
 class JmSearchPage(IterableEntity):
 
-    def __init__(self, album_info_list) -> None:
+    def __init__(self, album_info_list):
         # (album_id, title, category_none, label_sub_none, tag_list)
-        self.data: List[Tuple[str, str, StrNone, StrNone, List[str]]] = album_info_list
-
-    def album_id_iter(self):
-        for album_info in self.data:
-            yield album_info[0]
+        self.album_info_list: List[Tuple[str, str, StrNone, StrNone, List[str]]] = album_info_list
 
     def __len__(self):
-        return len(self.data)
+        return len(self.album_info_list)
 
     def __getitem__(self, item):
-        return self.data[item]
-
-
-# cdn爬取请求
-class CdnRequest:
-    SavePathProvider = Callable[[str, str, int, bool], str]
-
-    def __init__(self,
-                 photo_id,
-                 scramble_id,
-                 from_index: int,
-                 photo_len: Optional[int],
-                 save_path_provider: SavePathProvider,
-                 ):
-        self.photo_id = photo_id
-        self.scramble_id = scramble_id
-        self.from_index = from_index
-        self.photo_len = photo_len
-        self.save_path_provider = save_path_provider
-
-    @classmethod
-    def create(cls,
-               photo_id,
-               save_path_provider: SavePathProvider,
-               scramble_id,
-               from_index=1,
-               photo_len=None,
-               ):
-        return CdnRequest(
-            photo_id,
-            scramble_id,
-            from_index,
-            photo_len,
-            save_path_provider,
-        )
+        return self.album_info_list[item][0:2]
```

### Comparing `jmcomic-1.9.1/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.0/src/jmcomic/jm_toolkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -203,27 +203,27 @@
     @classmethod
     def save_resp_decoded_img(cls,
                               resp: Any,
                               img_detail: JmImageDetail,
                               filepath: str
                               ) -> None:
         cls.decode_and_save(
-            cls.calculate_segmentation_num(img_detail),
+            cls.get_num_by_detail(img_detail),
             cls.open_Image(resp.content),
             filepath
         )
 
     @classmethod
     def decode_disk_img(cls,
                         img_detail: JmImageDetail,
                         img_filepath: str,
                         decoded_save_path: str
                         ) -> None:
         cls.decode_and_save(
-            cls.calculate_segmentation_num(img_detail),
+            cls.get_num_by_detail(img_detail),
             cls.open_Image(img_filepath),
             decoded_save_path
         )
 
     @classmethod
     def decode_and_save(cls,
                         num: int,
@@ -271,28 +271,47 @@
     def open_Image(cls, fp: Union[str, bytes]):
         from PIL import Image
         from io import BytesIO
         fp = fp if isinstance(fp, str) else BytesIO(fp)
         return Image.open(fp)
 
     @classmethod
-    def calculate_segmentation_num(cls, detail: JmImageDetail) -> int:
+    def get_num(cls, scramble_id, aid, filename: str) -> int:
         """
         获得图片分割数
         """
-        scramble_id = int(detail.scramble_id)
-        aid = int(detail.aid)
+
+        scramble_id = int(scramble_id)
+        aid = int(aid)
 
         if aid < scramble_id:
             return 0
         elif aid < JmModuleConfig.SCRAMBLE_10:
             return 10
         else:
             import hashlib
             x = 10 if aid < JmModuleConfig.SCRAMBLE_NUM_8 else 8
-            s = f"{aid}{detail.img_file_name}"  # 拼接
+            s = f"{aid}{filename}"  # 拼接
             s = s.encode()
             s = hashlib.md5(s).hexdigest()
             num = ord(s[-1])
             num %= x
             num = num * 2 + 2
             return num
+
+    @classmethod
+    def get_num_by_url(cls, scramble_id, url) -> int:
+        """
+        获得图片分割数
+        """
+        return cls.get_num(
+            scramble_id,
+            aid=JmcomicText.parse_to_photo_id(url),
+            filename=of_file_name(url, True),
+        )
+
+    @classmethod
+    def get_num_by_detail(cls, detail: JmImageDetail) -> int:
+        """
+        获得图片分割数
+        """
+        return cls.get_num(detail.scramble_id, detail.aid, detail.img_file_name)
```

### Comparing `jmcomic-1.9.1/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.0/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.9.1
+Version: 2.0.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

