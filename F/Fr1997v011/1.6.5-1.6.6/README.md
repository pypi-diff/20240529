# Comparing `tmp/Fr1997v011-1.6.5.tar.gz` & `tmp/Fr1997v011-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.6.5.tar", last modified: Tue May 28 06:01:18 2024, max compression
+gzip compressed data, was "Fr1997v011-1.6.6.tar", last modified: Wed May 29 06:20:17 2024, max compression
```

## Comparing `Fr1997v011-1.6.5.tar` & `Fr1997v011-1.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.353311 Fr1997v011-1.6.5/
-drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.345308 Fr1997v011-1.6.5/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.5/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-28 06:01:18.352311 Fr1997v011-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-28 04:18:40.000000 Fr1997v011-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.346309 Fr1997v011-1.6.5/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.5/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.349311 Fr1997v011-1.6.5/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.5/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   171518 2024-05-28 06:01:16.000000 Fr1997v011-1.6.5/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.351309 Fr1997v011-1.6.5/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.5/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-28 06:01:18.353311 Fr1997v011-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-28 06:01:16.000000 Fr1997v011-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:20:17.882517 Fr1997v011-1.6.6/
+drwxrwxrwx   0        0        0        0 2024-05-29 06:20:17.853516 Fr1997v011-1.6.6/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-29 06:20:17.000000 Fr1997v011-1.6.6/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-29 06:20:17.000000 Fr1997v011-1.6.6/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 06:20:17.000000 Fr1997v011-1.6.6/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 06:20:17.000000 Fr1997v011-1.6.6/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-29 06:20:17.000000 Fr1997v011-1.6.6/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-29 06:20:17.872521 Fr1997v011-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-28 13:15:16.000000 Fr1997v011-1.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 06:20:17.864516 Fr1997v011-1.6.6/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.6/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:20:17.868521 Fr1997v011-1.6.6/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.6/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   167247 2024-05-29 02:54:03.000000 Fr1997v011-1.6.6/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-29 06:20:17.870522 Fr1997v011-1.6.6/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.6/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 06:20:17.882517 Fr1997v011-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-28 13:15:13.000000 Fr1997v011-1.6.6/setup.py
```

### Comparing `Fr1997v011-1.6.5/LICENSE` & `Fr1997v011-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.6.5/README.md` & `Fr1997v011-1.6.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.6.4.tar.gz
+pip install dist/Fr1997v011-1.6.6.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.6.5/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.6.6/fr1997_mode/mode_func/all_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
     pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.6.1
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.6.5
 """
 
 """
     pip3 install --upgrade Fr1997v011
     pip3 install redis
     pip3 install pymysql
     pip3 install elasticsearch
@@ -1953,48 +1953,14 @@
         if response.status_code == 200:
             data_data = response.json
             user_detail = data_data.get('user')
 
             data_json = self.analysis_douyin_user(user_detail)  # 数据获取
             return data_json
 
-    # 【api】 视频详情
-    def api_douyin_video_old(self, video_id, use_proxies=1, res_tp='video_info'):
-        cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
-        headers = {
-            "authority": "www.douyin.com",
-            "pragma": "no-cache",
-            "cache-control": "no-cache",
-            "accept": "application/json, text/plain, */*",
-            "user-agent": config_dict['base_ua'],
-            "referer": "https://www.douy" + "in.com/user/MS4wLjABAAAAM5BxLLRhN2jrzttuOUI3LEmFClP8t6dp0bf67Oi3deE",
-            "accept-language": "zh-CN,zh;q=0.9",
-            'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;{random.choice(cookies)}'
-        }
-
-        url = f'https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0'
-        url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
-        try:
-            if use_proxies:
-                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
-            else:
-                response = HttpJike.get(url=url, headers=headers)
-            if response.status_code == 200:
-                data_data = response.json
-
-                # 是否存在
-                if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
-                    return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
-
-                video_detail = data_data['aweme_detail']
-                data_json = mode_spider.douyin_video_response(video_detail, tp=res_tp)  # 数据获取
-                return data_json
-        except Exception as E:
-            return {'aweme_type': 1, 'is_alive': 0, 'err': E}
-
     # 【api】 视频详情 2024-05-28
     def api_douyin_video(self, video_id, use_proxies=1, res_tp='video_info'):
         headers = {
             "user-agent": config_dict['base_ua'],
         }
         url = f'https://aweme.snssdk.com/aweme/v1/multi/aweme/detail/?aweme_ids=[{video_id}]'
         try:
@@ -2006,55 +1972,16 @@
                 data_data = response.json
                 aweme_details = data_data['aweme_details']
                 if aweme_details:
                     video_detail = aweme_details[0]
                     data_json = mode_spider.douyin_video_response2(video_detail, tp=res_tp)  # 数据获取
                     return data_json
                 else:
-                    print("没有数据")
-
-        except Exception as E:
-            return {'aweme_type': 1, 'is_alive': 0, 'err': E}
-
-    # 【api】 视频详情
-    def api_douyin_video_cookie(self, video_id, use_proxies=1, res_tp='video_info', nc=None):
-        cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
-
-        print(random.choice(cookies))
-        headers = {
-            "authority": "www.douyin.com",
-            "pragma": "no-cache",
-            "cache-control": "no-cache",
-            "accept": "application/json, text/plain, */*",
-            "user-agent": config_dict['base_ua'],
-            "referer": "https://www.douy" + "in.com/user/MS4wLjABAAAAM5BxLLRhN2jrzttuOUI3LEmFClP8t6dp0bf67Oi3deE",
-            "accept-language": "zh-CN,zh;q=0.9",
-            # 'cookie':f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;__ac_nonce=066555a45000c53ec2bfd; __ac_signature=_02B4Z6wo00f018lQJLAAAIDDFidCqT5aCBfJcCAAAJQKaI0pMYyKNFyZl3yW2m1RRFENvDzftFrOz8CPtglGy14SoXj9SUTLrpuAX8h6P9Z-ERHDzPFm8BMUKNBbhdqW34Wfm1aEewD8aUd7bc;'
-            # 'cookie': 'ttwid=1%7CARl_GZTLCKZHJ57UtJTQd4d2gvGRa6im27p4kVMquO8%7C1713580624%7C33cbf11ff924db7aa2566de888817f3729d15736a8f76f49b27ee77fa5b23ea9;'
-            'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;__ac_nonce=0658c0c6200a36d7cfa0a; __ac_signature=_02B4Z6wo00001ztv5IAAAIDBuvhKN7Rrq887b-AAAKtic9;ttwid={nc}; __ac_referer=__ac_blank'
-        }
-        print(headers)
-
-        url = f'https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0'
-        url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
-        try:
-            if use_proxies:
-                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
-            else:
-                response = HttpJike.get(url=url, headers=headers)
-            if response.status_code == 200:
-                data_data = response.json
+                    return {'aweme_type': 1, 'is_alive': 0, 'err': '没有数据'}
 
-                # 是否存在
-                if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
-                    return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
-
-                video_detail = data_data['aweme_detail']
-                data_json = mode_spider.douyin_video_response(video_detail, tp=res_tp)  # 数据获取
-                return data_json
         except Exception as E:
             return {'aweme_type': 1, 'is_alive': 0, 'err': E}
 
     # 【api】 抖音合集列表
     def api_douyin_mix_list(self, cursor=0, limit=6, use_proxies=1):
         cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
         headers = {
```

