# Comparing `tmp/blockmango-1.4.4.tar.gz` & `tmp/blockmango-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.4.tar", last modified: Thu May 23 13:02:11 2024, max compression
+gzip compressed data, was "blockmango-1.4.5.tar", last modified: Tue May 28 20:22:04 2024, max compression
```

## Comparing `blockmango-1.4.4.tar` & `blockmango-1.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.175326 blockmango-1.4.4/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.4/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      425 2024-05-23 13:02:11.171326 blockmango-1.4.4/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.4/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.151326 blockmango-1.4.4/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.4/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4628 2024-05-17 15:51:44.000000 blockmango-1.4.4/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1477 2024-05-23 12:59:50.000000 blockmango-1.4.4/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2505 2024-05-17 15:53:00.000000 blockmango-1.4.4/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-17 15:53:21.000000 blockmango-1.4.4/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3674 2024-05-17 15:53:39.000000 blockmango-1.4.4/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2437 2024-05-23 12:58:39.000000 blockmango-1.4.4/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.167326 blockmango-1.4.4/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      425 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      349 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-23 13:02:11.175326 blockmango-1.4.4/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      498 2024-05-23 13:01:12.000000 blockmango-1.4.4/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.902259 blockmango-1.4.5/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.5/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)     1716 2024-05-28 20:22:04.902259 blockmango-1.4.5/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.5/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.882259 blockmango-1.4.5/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.5/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4177 2024-05-28 20:15:07.000000 blockmango-1.4.5/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     1336 2024-05-28 20:16:13.000000 blockmango-1.4.5/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2231 2024-05-28 20:15:48.000000 blockmango-1.4.5/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.5/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.5/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2105 2024-05-28 20:19:37.000000 blockmango-1.4.5/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-28 20:22:04.898259 blockmango-1.4.5/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)     1716 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      349 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-28 20:22:04.000000 blockmango-1.4.5/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-28 20:22:04.902259 blockmango-1.4.5/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)     1091 2024-05-28 20:14:26.000000 blockmango-1.4.5/setup.py
```

### Comparing `blockmango-1.4.4/LICENSE.md` & `blockmango-1.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.4/README.md` & `blockmango-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.4/blockmango/clan.py` & `blockmango-1.4.5/blockmango/clan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,81 @@
 from .http import HTTPMixin
 
-
 BASE_URL = "http://modsgs.sandboxol.com/clan/api/v1/clan"
 BASE_URL_V2 = "http://modsgs.sandboxol.com/clan/api/v2/clan"
 BASE_URL_V3 = "http://modsgs.sandboxol.com/clan/api/v3/clan"
 
-
 class Clan(HTTPMixin):
-  __slots__ = ("headers",)
-
   def __init__(self, user_id, access_token):
-    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
   def user_clan(self):
     return self._get(f"{BASE_URL}/tribe/base", headers=self.headers)
 
   def join(self, clan_id):
-    return self._post(f"{BASE_URL}/tribe/member", headers=self.headers, json_data={ "clanId": clan_id, "msg": "" })
+    return self._post(f"{BASE_URL}/tribe/member", headers=self.headers, json={"clanId": clan_id, "msg": ""})
 
   def leave(self, clan_id):
-    return self._delete(f"{BASE_URL}/tribe/member", headers=self.headers, params={ "clanId": clan_id })
+    return self._delete(f"{BASE_URL}/tribe/member", headers=self.headers, params={"clanId": clan_id})
 
-  def search(self, clan_name, page_no = 0, page_size = 20):
-    params = {"clanName": clan_name, "pageNo": page_no, "pageSize": page_size}
-    return self._get(f"{BASE_URL}/tribe/blurry/info", headers=self.headers, params=params)
+  def search(self, clan_name, page_no=0, page_size=20):
+    return self._get(f"{BASE_URL}/tribe/blurry/info", headers=self.headers, params={"clanName": clan_name, "pageNo": page_no, "pageSize": page_size})
 
   def info(self, clan_id):
-    return self._get(f"{BASE_URL_V2}/tribe", headers=self.headers, params={ "clanId": clan_id })
+    return self._get(f"{BASE_URL_V2}/tribe", headers=self.headers, params={"clanId": clan_id})
 
-  def invite(self, friend_ids, message = ""):
-    json_data = { "friendIds": friend_ids, "msg": message }
-    return self._post(f"{BASE_URL}/tribe/member/invite", headers=self.headers, json_data=json_data)
+  def invite(self, friend_ids, message=""):
+    return self._post(f"{BASE_URL}/tribe/member/invite", headers=self.headers, json={"friendIds": friend_ids, "msg": message})
 
   def agreement_user(self, other_id):
-    return self._put(f"{BASE_URL}/tribe/member/agreement", headers=self.headers, params={ "otherId": other_id })
+    return self._put(f"{BASE_URL}/tribe/member/agreement", headers=self.headers, params={"otherId": other_id})
 
   def reject_user(self, other_id):
-    return self._put(f"{BASE_URL}/tribe/member/rejection", headers=self.headers, params={ "otherId": other_id })
+    return self._put(f"{BASE_URL}/tribe/member/rejection", headers=self.headers, params={"otherId": other_id})
 
   def mute_member(self, member_id, minutes):
-    params = { "memberId": member_id, "minute": minutes }
-    return self._post(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params=params)
+    return self._post(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params={"memberId": member_id, "minute": minutes})
 
   def unmute_member(self, member_id):
-    return self._delete(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params={ "memberId": member_id })
+    return self._delete(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params={"memberId": member_id})
 
   def mute_all(self):
-    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={ "muteStatus": 1 })
+    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={"muteStatus": 1})
 
   def unmute_all(self):
-    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={ "muteStatus": 0 })
+    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={"muteStatus": 0})
 
   def remove_member(self, member_ids):
-    return self._delete(f"{BASE_URL}/tribe/member/remove/batch", headers=self.headers, json_data=member_ids)
+    return self._delete(f"{BASE_URL}/tribe/member/remove/batch", headers=self.headers, json=member_ids)
 
-  def edit(self, clan_id, currency = 0, details = "", head_pic = "", name = "", tags = None):
-    json_data = {
-      "clanId": clan_id,
-      "currency": currency,
-      "details": details,
-      "headPic": head_pic,
-      "name": name,
-      "tags": tags or []
-    }
-    return self._put(f"{BASE_URL}/tribe", headers=self.headers, json_data=json_data)
+  def edit(self, clan_id, currency=0, details="", head_pic="", name="", tags=None):
+    return self._put(f"{BASE_URL}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
 
   def edit_elders(self, type_, elder_ids):
-    params = { "type": type_, "otherIds": elder_ids }
-    return self._put(f"{BASE_URL}/tribe/members", headers=self.headers, params=params)
+    return self._put(f"{BASE_URL}/tribe/members", headers=self.headers, params={"type": type_, "otherIds": elder_ids})
 
   def authentication(self, type_):
-    params = { "freeVerify": 1 if type_ == "on" else 0 }
-    return self._put(f"{BASE_URL}/free/verification", headers=self.headers, params=params)
+    return self._put(f"{BASE_URL}/free/verification", headers=self.headers, params={"freeVerify": 1 if type_ == "on" else 0})
 
   def buy_decoration(self, decoration_id):
-    return self._put(f"{BASE_URL}/decorations/purchase", headers=self.headers, params={ "decorationId": decoration_id })
+    return self._put(f"{BASE_URL}/decorations/purchase", headers=self.headers, params={"decorationId": decoration_id})
 
   def task_accept(self, task_id, is_team_task):
-    params = { "id": task_id, "type": 0 if is_team_task == True else 1 }
-    return self._put("{BASE_URL}/tasks/accept", headers=self.headers, params=params)
+    return self._put(f"{BASE_URL}/tasks/accept", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
 
   def self_task_refresh(self):
-    return self._get(f"{BASE_URL_V3}/personal/tasks", headers=self.headers, params={ "type": 1 })
+    return self._get(f"{BASE_URL_V3}/personal/tasks", headers=self.headers, params={"type": 1})
 
   def task_claim(self, task_id, is_team_task):
-    params = { "id": task_id, "type": 0 if is_team_task == True else 1 }
-    return self._put(f"{BASE_URL}/tasks", headers=self.headers, params=params)
+    return self._put(f"{BASE_URL}/tasks", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
 
   def notice(self, content):
-    json_data = { "content": content }
-    return self._post(f"{BASE_URL}/tribe/bulletin", headers=self.headers, json_data=json_data)
+    return self._post(f"{BASE_URL}/tribe/bulletin", headers=self.headers, json={"content": content})
 
   def transfer_chief(self, new_chief_id):
-    return self._put(f"{BASE_URL}/tribe/member", headers=self.headers, params={ "otherId": new_chief_id, "type": 3 })
+    return self._put(f"{BASE_URL}/tribe/member", headers=self.headers, params={"otherId": new_chief_id, "type": 3})
 
-  def create(self, clan_id = 0, currency = 2, details = "", head_pic = "", name = "", tags = None):
-    json_data = {
-      "clanId": clan_id,
-      "currency": currency,
-      "details": details,
-      "headPic": head_pic,
-      "name": name,
-      "tags": tags or []
-    }
-    return self._post(f"{BASE_URL_V3}/tribe", headers=self.headers, json_data=json_data)
+  def create(self, clan_id=0, currency=2, details="", head_pic="", name="", tags=None):
+    return self._post(f"{BASE_URL_V3}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
 
   def dissolve(self, clan_id):
-    return self._delete(f"{BASE_URL}/tribe", headers=self.headers, params={ "clanId": clan_id })
+    return self._delete(f"{BASE_URL}/tribe", headers=self.headers, params={"clanId": clan_id})
```

### Comparing `blockmango-1.4.4/blockmango/decoration.py` & `blockmango-1.4.5/blockmango/decoration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 from .http import HTTPMixin
 
-
 BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
 BASE_URL_SHOP = "http://modsgs.sandboxol.com/shop/api/v1"
 BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
 
-
 class Decoration(HTTPMixin):
-  __slots__ = ("headers",)
-
   def __init__(self, user_id, access_token):
-    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
   def skins(self, uid):
-    endpoint = f"{BASE_URL_DECORATION}/new/decorations/users/{uid}/classify/all"
-    params = { "engineVersion": "10105", "os": "android", "showVip": 1 }
-    return self._get(endpoint, headers=self.headers, params=params)
+    params = {"engineVersion": "10105", "os": "android", "showVip": 1}
+    return self._get(f"{BASE_URL_DECORATION}/new/decorations/users/{uid}/classify/all", headers=self.headers, params=params)
 
   def current_price(self, skin_id, is_suit):
-    endpoint = f"{BASE_URL_DECORATION}/decoration/current/price"
-    payload = [{ "id": skin_id, "isSuit": is_suit }]
-    return self._post(endpoint, headers=self.headers, json_data=payload)
+    payload = [{"id": skin_id, "isSuit": is_suit}]
+    return self._post(f"{BASE_URL_DECORATION}/decoration/current/price", headers=self.headers, json=payload)
 
   def buy(self, diamond, cloth_voucher, paytype):
-    endpoint = f"{BASE_URL_SHOP}/new/shop/decorations/buy"
-    params = { "diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype }
-    return self._post(endpoint, headers=self.headers, params=params)
+    params = {"diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype}
+    return self._post(f"{BASE_URL_SHOP}/new/shop/decorations/buy", headers=self.headers, params=params)
 
   def shop_info(self):
     return self._get(f"{BASE_URL_USER}/user/shop/info", headers=self.headers)
 
   def equip(self, skin_id):
-    endpoint = f"{BASE_URL_DECORATION}/decorations/using/new"
-    params = { "ids": skin_id }
-    return self._post(endpoint, headers=self.headers, params=params)
+    params = {"ids": skin_id}
+    return self._post(f"{BASE_URL_DECORATION}/decorations/using/new", headers=self.headers, params=params)
```

### Comparing `blockmango-1.4.4/blockmango/friends.py` & `blockmango-1.4.5/blockmango/friends.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,48 @@
 from .http import HTTPMixin
 
-
 BASE_URL_FRIEND = "http://modsgs.sandboxol.com/friend/api/v1"
 BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
 
-
 class Friends(HTTPMixin):
-  __slots__ = ("headers",)
-
   def __init__(self, user_id, access_token):
-    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
   def delete_friend(self, friend_id):
-    endpoint = f"{BASE_URL_FRIEND}/friends"
-    params = { "friendId": friend_id }
-    return self._delete(endpoint, headers=self.headers, params=params)
+    return self._delete(f"{BASE_URL_FRIEND}/friends", headers=self.headers, params={"friendId": friend_id})
 
   def request(self, friend_id, msg):
-    endpoint = f"{BASE_URL_FRIEND}/friends"
-    payload = { "friendId": friend_id, "msg": msg, "type": 1 }
-    headers = { **self.headers, "Content-Type": "application/json" }
-    return self._post(endpoint, headers=headers, json_data=payload)
+    payload = {"friendId": friend_id, "msg": msg, "type": 1}
+    headers = {"Content-Type": "application/json", **self.headers}
+    return self._post(f"{BASE_URL_FRIEND}/friends", headers=headers, json=payload)
 
   def popularity(self, friend_id):
     return self._get(f"{BASE_URL_FRIEND}/popularity/{friend_id}", headers=self.headers)
 
   def info(self, friend_id):
     return self._get(f"{BASE_URL_FRIEND}/friends/{friend_id}", headers=self.headers)
 
   def decoration(self, friend_id):
     return self._get(f"{BASE_URL_DECORATION}/decorations-v2/{friend_id}/using", headers=self.headers)
 
   def add_popularity(self, friend_id):
-    endpoint = f"{BASE_URL_FRIEND}/popularity"
-    params = { "friendId": friend_id }
-    return self._post(endpoint, headers=self.headers, params=params)
+    return self._post(f"{BASE_URL_FRIEND}/popularity", headers=self.headers, params={"friendId": friend_id})
 
   def friend_list(self):
-    endpoint = f"{BASE_URL_FRIEND}/friends/status"
-    headers ={ **self.headers, "language": "en_US" }
-    return self._get(endpoint, headers=headers)
+    headers = {"language": "en_US", **self.headers}
+    return self._get(f"{BASE_URL_FRIEND}/friends/status", headers=headers)
 
   def nickname(self, friend_id, alias):
-    endpoint = f"{BASE_URL_FRIEND}/friends/{friend_id}/alias"
-    params = { "alias": alias }
-    return self._post(endpoint, headers=self.headers, params=params)
+    return self._post(f"{BASE_URL_FRIEND}/friends/{friend_id}/alias", headers=self.headers, params={"alias": alias})
 
   def friend_approve(self, friend_id):
     return self._put(f"{BASE_URL_FRIEND}/friends/{friend_id}/agreement", headers=self.headers)
 
   def friend_blacklist(self, friend_id):
-    endpoint = f"{BASE_URL_FRIEND}/friends/black"
-    params = { "friendId": friend_id }
-    return self._delete(endpoint, headers=self.headers, params=params)
+    return self._delete(f"{BASE_URL_FRIEND}/friends/black", headers=self.headers, params={"friendId": friend_id})
 
   def reject_all(self):
     return self._post(f"{BASE_URL_FRIEND}/friends/requests/reject-all", headers=self.headers)
 
   def approve_all(self):
     return self._post(f"{BASE_URL_FRIEND}/friends/requests/approve-all", headers=self.headers)
```

### Comparing `blockmango-1.4.4/blockmango/groupchat.py` & `blockmango-1.4.5/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.4/blockmango/user.py` & `blockmango-1.4.5/blockmango/user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,39 @@
 from .http import HTTPMixin
 
-
 BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
 BASE_URL_ROUTE = "http://route.sandboxol.com/user/api"
-BASE_URL_USER_INFO = "http://modsgs.sandboxol.com/api"
+BASE_URL_USER_INFO = "http://modsgs.sandboxol.com/user/api"
 
 class User(HTTPMixin):
-  __slots__ = ("headers",)
+    __slots__ = ("headers",)
+
+    def __init__(self, user_id, access_token):
+        self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+
+    def get_user_info(self):
+        return self._get(f"{BASE_URL_USER_INFO}/v2/user/details/info", headers=self.headers)
+
+    def set_birthday(self, birthday):
+        return self._put(f"{BASE_URL_USER}/user/info", headers=self.headers, json_data={"birthday": birthday})
+
+    def login(self, device_id, device_sign, password, userId):
+        headers = { **self.headers, "bmg-sign": device_sign, "bmg-device-id": device_id }
+        return self._post(f"{BASE_URL_ROUTE}/v1/app/login", headers=headers, json_data={"password": password, "uid": userId})
+
+    def change_name(self, new_name, old_name):
+        return self._put(f"{BASE_URL_USER_INFO}/v3/user/nickName", headers=self.headers, params={"newName": new_name, "oldName": old_name})
+
+    def change_details(self, new_details):
+        return self._put(f"{BASE_URL_USER_INFO}/v1/user/info", headers=self.headers, json_data={"details": new_details})
+
+    def change_pfp(self, pfp_url):
+        return self._put(f"{BASE_URL_USER}/user/info", headers=self.headers, json_data={"picUrl": pfp_url})
 
-  def __init__(self, user_id, access_token):
-    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+    def modify_password(self, old_password, new_password):
+        return self._post(f"{BASE_URL_USER}/user/password/modify", headers=self.headers, json_data={"confirmPassword": "", "newPassword": new_password, "oldPassword": old_password})
 
-  def get_user_info(self):
-    return self._get(f"{BASE_URL_USER_INFO}/v2/user/details/info", headers=self.headers)
+    def bind_email(self, email, verify_code):
+        return self._post(f"{BASE_URL_USER}/users/bind/email", headers=self.headers, json_data={"email": email, "verifyCode": verify_code})
 
-  def set_birthday(self, birthday):
-    endpoint = f"{BASE_URL_USER}/user/info"
-    json_data = { "birthday": birthday }
-    return self._put(endpoint, headers=self.headers, json_data=json_data)
-
-  def login(self, device_id, device_sign, password, userId):
-    endpoint = f"{BASE_URL_ROUTE}/v1/app/login"
-    headers = { **self.headers, "bmg-sign": device_sign, "bmg-device-id": device_id }
-    json_data = { "password": password, "uid": userId }
-    return self._post(endpoint, headers=headers, json_data=json_data)
-
-  def change_name(self, new_name, old_name):
-    endpoint = f"{BASE_URL_USER_INFO}/v3/user/nickName"
-    params = { "newName": new_name, "oldName": old_name }
-    return self._put(endpoint, headers=self.headers, params=params)
-
-  def change_details(self, new_details):
-    endpoint = f"{BASE_URL_USER_INFO}/v1/user/info"
-    json_data = { "details": new_details }
-    return self._put(endpoint, headers=self.headers, json_data=json_data)
-
-  def change_pfp(self, pfp_url):
-    endpoint = f"{BASE_URL_USER}/user/info"
-    json_data = { "picUrl": pfp_url }
-    return self._put(endpoint, headers=self.headers, json_data=json_data)
-
-  def modify_password(self, old_password, new_password):
-    endpoint = f"{BASE_URL_USER}/user/password/modify"
-    json_data = {"confirmPassword": "", "newPassword": new_password, "oldPassword": old_password}
-    return self._post(endpoint, headers=self.headers, json_data=json_data)
-
-  def bind_email(self, email, verify_code):
-    endpoint = f"{BASE_URL_USER}/users/bind/email"
-    json_data = { "email": email, "verifyCode": verify_code }
-    return self._post(endpoint, headers=self.headers, json_data=json_data)
-
-  def unbind_email(self, verify_code, email):
-    endpoint = f"{BASE_URL_USER_INFO}/v2/users/{self.headers['userId']}/emails"
-    params = { "email": email, "verifyCode": verify_code }
-    return self._delete(endpoint, headers=self.headers, params=params)
+    def unbind_email(self, verify_code, email):
+        return self._delete(f"{BASE_URL_USER_INFO}/v2/users/{self.headers['userId']}/emails", headers=self.headers, params={"email": email, "verifyCode": verify_code})
```

