# Comparing `tmp/nokey-0.7.3.tar.gz` & `tmp/nokey-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.7.3.tar", max compression
+gzip compressed data, was "nokey-0.7.4.tar", max compression
```

## Comparing `nokey-0.7.3.tar` & `nokey-0.7.4.tar`

### file list

```diff
@@ -1,67 +1,66 @@
--rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.7.3/LICENSE
--rw-r--r--   0        0        0     3407 2024-05-25 13:37:22.426835 nokey-0.7.3/README.md
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.3/nokey/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 20:14:26.068986 nokey-0.7.3/nokey/activities/__init__.py
--rw-r--r--   0        0        0     5359 2024-05-27 14:42:41.748021 nokey-0.7.3/nokey/activities/bored_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.010835 nokey-0.7.3/nokey/animals/__init__.py
--rw-r--r--   0        0        0     2991 2024-05-27 14:42:17.448020 nokey-0.7.3/nokey/animals/dog_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.130835 nokey-0.7.3/nokey/art_and_images/__init__.py
--rw-r--r--   0        0        0    93276 2024-05-25 13:32:21.126835 nokey-0.7.3/nokey/art_and_images/artic.py
--rw-r--r--   0        0        0     8014 2024-05-25 13:32:21.134835 nokey-0.7.3/nokey/art_and_images/lorem_picsum.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.118835 nokey-0.7.3/nokey/books_and_literature/__init__.py
--rw-r--r--   0        0        0     6320 2024-05-25 13:32:21.122835 nokey-0.7.3/nokey/books_and_literature/gutendex.py
--rw-r--r--   0        0        0     3495 2024-05-25 13:32:21.106835 nokey-0.7.3/nokey/books_and_literature/stephen_king.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.898835 nokey-0.7.3/nokey/calendar/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-25 13:32:20.894835 nokey-0.7.3/nokey/calendar/nager_date.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.978835 nokey-0.7.3/nokey/country_info/__init__.py
--rw-r--r--   0        0        0     4985 2024-05-25 13:32:20.978835 nokey-0.7.3/nokey/country_info/rest_country.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.162835 nokey-0.7.3/nokey/developer_tools/__init__.py
--rw-r--r--   0        0        0     4187 2024-05-25 13:32:21.158835 nokey-0.7.3/nokey/developer_tools/apis_guru.py
--rw-r--r--   0        0        0     3809 2024-05-25 13:32:21.150835 nokey-0.7.3/nokey/developer_tools/filter_lists.py
--rw-r--r--   0        0        0     2862 2024-05-25 13:32:21.154835 nokey-0.7.3/nokey/developer_tools/microlink.py
--rw-r--r--   0        0        0     7552 2024-05-25 13:32:21.166835 nokey-0.7.3/nokey/developer_tools/url_haus.py
--rw-r--r--   0        0        0     1964 2024-05-25 13:32:21.162835 nokey-0.7.3/nokey/developer_tools/url_shortener.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.966835 nokey-0.7.3/nokey/education/__init__.py
--rw-r--r--   0        0        0     2591 2024-05-25 13:32:20.970835 nokey-0.7.3/nokey/education/university_domains_and_names.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.042835 nokey-0.7.3/nokey/finance_and_crypto/__init__.py
--rw-r--r--   0        0        0     6117 2024-05-25 13:32:21.050835 nokey-0.7.3/nokey/finance_and_crypto/coinmap.py
--rw-r--r--   0        0        0     2758 2024-05-25 13:32:21.046835 nokey-0.7.3/nokey/finance_and_crypto/exchange_api.py
--rw-r--r--   0        0        0     1382 2024-05-25 13:32:21.054835 nokey-0.7.3/nokey/finance_and_crypto/wallstreet_bets.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.090835 nokey-0.7.3/nokey/food/__init__.py
--rw-r--r--   0        0        0     3441 2024-05-25 13:32:21.094835 nokey-0.7.3/nokey/food/fruityvice.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.082835 nokey-0.7.3/nokey/games/__init__.py
--rw-r--r--   0        0        0     6785 2024-05-25 13:32:21.082835 nokey-0.7.3/nokey/games/free_to_game.py
--rw-r--r--   0        0        0     5626 2024-05-25 13:32:21.074835 nokey-0.7.3/nokey/games/open_trivia_db.py
--rw-r--r--   0        0        0    30480 2024-05-25 13:32:21.078835 nokey-0.7.3/nokey/games/shadify.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.866835 nokey-0.7.3/nokey/geolocation/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-25 13:32:20.862835 nokey-0.7.3/nokey/geolocation/ip_api.py
--rw-r--r--   0        0        0     2119 2024-05-25 13:32:20.866835 nokey-0.7.3/nokey/geolocation/zippopotamus.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.062835 nokey-0.7.3/nokey/government/__init__.py
--rw-r--r--   0        0        0    10908 2024-05-25 13:32:21.062835 nokey-0.7.3/nokey/government/federal_register.py
--rw-r--r--   0        0        0   157578 2024-05-25 13:32:21.066835 nokey-0.7.3/nokey/government/usa_spending.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.906835 nokey-0.7.3/nokey/health/__init__.py
--rw-r--r--   0        0        0    32273 2024-05-25 13:32:20.906835 nokey-0.7.3/nokey/health/open_disease.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.926835 nokey-0.7.3/nokey/helperFuncs/__init__.py
--rw-r--r--   0        0        0      822 2024-05-25 13:32:20.930835 nokey-0.7.3/nokey/helperFuncs/get_api_list.py
--rw-r--r--   0        0        0     6904 2024-05-27 22:33:52.561311 nokey-0.7.3/nokey/helperFuncs/make_request.py
--rw-r--r--   0        0        0     1076 2024-05-25 13:32:20.934835 nokey-0.7.3/nokey/helperFuncs/nokey_apis.py
--rw-r--r--   0        0        0     1514 2024-05-25 13:32:20.962835 nokey-0.7.3/nokey/helperFuncs/throttler.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.838835 nokey-0.7.3/nokey/inspiration/__init__.py
--rw-r--r--   0        0        0     6164 2024-05-25 13:32:20.834835 nokey-0.7.3/nokey/inspiration/dictum.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.038835 nokey-0.7.3/nokey/jokes/__init__.py
--rw-r--r--   0        0        0     3342 2024-05-25 13:32:21.034835 nokey-0.7.3/nokey/jokes/joke_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.006835 nokey-0.7.3/nokey/language/__init__.py
--rw-r--r--   0        0        0     1433 2024-05-25 13:32:21.006835 nokey-0.7.3/nokey/language/free_dictionary.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.998835 nokey-0.7.3/nokey/random/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-25 13:32:20.998835 nokey-0.7.3/nokey/random/random_user.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.182835 nokey-0.7.3/nokey/science_and_nature/__init__.py
--rw-r--r--   0        0        0    50832 2024-05-25 13:32:21.174835 nokey-0.7.3/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-r--r--   0        0        0     3192 2024-05-25 13:32:21.178835 nokey-0.7.3/nokey/science_and_nature/nobel_prize.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.3/nokey/spaceflight/__init__.py
--rw-r--r--   0        0        0     9033 2024-05-25 13:32:20.986835 nokey-0.7.3/nokey/spaceflight/spaceflight_news.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.874835 nokey-0.7.3/nokey/tv_and_film/__init__.py
--rw-r--r--   0        0        0    43761 2024-05-25 13:32:20.878835 nokey-0.7.3/nokey/tv_and_film/star_trek_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.846835 nokey-0.7.3/nokey/weather/__init__.py
--rw-r--r--   0        0        0    26351 2024-05-25 13:32:20.842835 nokey-0.7.3/nokey/weather/national_weather_service.py
--rw-r--r--   0        0        0      711 2024-05-27 22:35:31.925311 nokey-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 nokey-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3407 2024-05-25 13:37:22.426835 nokey-0.7.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.396011 nokey-0.7.4/nokey/__init__.py
+-rw-r--r--   0        0        0     5402 2024-05-29 00:22:24.580011 nokey-0.7.4/nokey/activities/bored_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.416011 nokey-0.7.4/nokey/animals/__init__.py
+-rw-r--r--   0        0        0     3018 2024-05-29 00:22:24.420011 nokey-0.7.4/nokey/animals/dog_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.612011 nokey-0.7.4/nokey/art_and_images/__init__.py
+-rw-r--r--   0        0        0    94174 2024-05-29 00:22:24.632011 nokey-0.7.4/nokey/art_and_images/artic.py
+-rw-r--r--   0        0        0     8063 2024-05-29 00:22:24.628011 nokey-0.7.4/nokey/art_and_images/lorem_picsum.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.500011 nokey-0.7.4/nokey/books_and_literature/__init__.py
+-rw-r--r--   0        0        0     6384 2024-05-29 00:22:24.500011 nokey-0.7.4/nokey/books_and_literature/gutendex.py
+-rw-r--r--   0        0        0     3527 2024-05-29 00:22:24.516011 nokey-0.7.4/nokey/books_and_literature/stephen_king.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.596011 nokey-0.7.4/nokey/calendar/__init__.py
+-rw-r--r--   0        0        0     5132 2024-05-29 00:22:24.600011 nokey-0.7.4/nokey/calendar/nager_date.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.592011 nokey-0.7.4/nokey/country_info/__init__.py
+-rw-r--r--   0        0        0     5029 2024-05-29 00:22:24.588011 nokey-0.7.4/nokey/country_info/rest_country.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.556011 nokey-0.7.4/nokey/developer_tools/__init__.py
+-rw-r--r--   0        0        0     4229 2024-05-29 00:22:24.556011 nokey-0.7.4/nokey/developer_tools/apis_guru.py
+-rw-r--r--   0        0        0     3849 2024-05-29 00:22:24.552011 nokey-0.7.4/nokey/developer_tools/filter_lists.py
+-rw-r--r--   0        0        0     2886 2024-05-29 00:22:24.568011 nokey-0.7.4/nokey/developer_tools/microlink.py
+-rw-r--r--   0        0        0     7600 2024-05-29 00:22:24.564011 nokey-0.7.4/nokey/developer_tools/url_haus.py
+-rw-r--r--   0        0        0     1978 2024-05-29 00:22:24.560011 nokey-0.7.4/nokey/developer_tools/url_shortener.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.456011 nokey-0.7.4/nokey/education/__init__.py
+-rw-r--r--   0        0        0     2613 2024-05-29 00:22:24.460011 nokey-0.7.4/nokey/education/university_domains_and_names.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.372011 nokey-0.7.4/nokey/finance_and_crypto/__init__.py
+-rw-r--r--   0        0        0     6397 2024-05-29 00:22:24.372011 nokey-0.7.4/nokey/finance_and_crypto/coinmap.py
+-rw-r--r--   0        0        0     2778 2024-05-29 00:22:24.368011 nokey-0.7.4/nokey/finance_and_crypto/exchange_api.py
+-rw-r--r--   0        0        0     1371 2024-05-29 00:22:24.364011 nokey-0.7.4/nokey/finance_and_crypto/wallstreet_bets.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.720011 nokey-0.7.4/nokey/food/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-29 00:22:24.716011 nokey-0.7.4/nokey/food/fruityvice.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.528011 nokey-0.7.4/nokey/games/__init__.py
+-rw-r--r--   0        0        0     6830 2024-05-29 00:22:24.520011 nokey-0.7.4/nokey/games/free_to_game.py
+-rw-r--r--   0        0        0     5646 2024-05-29 00:22:24.532011 nokey-0.7.4/nokey/games/open_trivia_db.py
+-rw-r--r--   0        0        0    30709 2024-05-29 00:22:24.524011 nokey-0.7.4/nokey/games/shadify.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.448011 nokey-0.7.4/nokey/geolocation/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-29 00:22:24.444011 nokey-0.7.4/nokey/geolocation/ip_api.py
+-rw-r--r--   0        0        0     2141 2024-05-29 00:22:24.452011 nokey-0.7.4/nokey/geolocation/zippopotamus.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.536011 nokey-0.7.4/nokey/government/__init__.py
+-rw-r--r--   0        0        0    10990 2024-05-29 00:22:24.544011 nokey-0.7.4/nokey/government/federal_register.py
+-rw-r--r--   0        0        0   158856 2024-05-29 00:22:24.540011 nokey-0.7.4/nokey/government/usa_spending.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.388011 nokey-0.7.4/nokey/health/__init__.py
+-rw-r--r--   0        0        0    32506 2024-05-29 00:22:24.392011 nokey-0.7.4/nokey/health/open_disease.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.708011 nokey-0.7.4/nokey/helperFuncs/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-29 00:22:24.708011 nokey-0.7.4/nokey/helperFuncs/get_api_list.py
+-rw-r--r--   0        0        0     6970 2024-05-29 00:22:24.676011 nokey-0.7.4/nokey/helperFuncs/make_request.py
+-rw-r--r--   0        0        0     1076 2024-05-29 00:22:24.680011 nokey-0.7.4/nokey/helperFuncs/nokey_apis.py
+-rw-r--r--   0        0        0     3146 2024-05-29 00:22:24.676011 nokey-0.7.4/nokey/helperFuncs/throttler.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.488011 nokey-0.7.4/nokey/inspiration/__init__.py
+-rw-r--r--   0        0        0     6223 2024-05-29 00:22:24.492011 nokey-0.7.4/nokey/inspiration/dictum.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.484011 nokey-0.7.4/nokey/jokes/__init__.py
+-rw-r--r--   0        0        0     3364 2024-05-29 00:22:24.480011 nokey-0.7.4/nokey/jokes/joke_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.636011 nokey-0.7.4/nokey/language/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-29 00:22:24.640011 nokey-0.7.4/nokey/language/free_dictionary.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.472011 nokey-0.7.4/nokey/random/__init__.py
+-rw-r--r--   0        0        0     1376 2024-05-29 00:22:24.476011 nokey-0.7.4/nokey/random/random_user.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.656011 nokey-0.7.4/nokey/science_and_nature/__init__.py
+-rw-r--r--   0        0        0    51134 2024-05-29 00:22:24.652011 nokey-0.7.4/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-r--r--   0        0        0     3218 2024-05-29 00:22:24.656011 nokey-0.7.4/nokey/science_and_nature/nobel_prize.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.608011 nokey-0.7.4/nokey/spaceflight/__init__.py
+-rw-r--r--   0        0        0     9093 2024-05-29 00:22:24.604011 nokey-0.7.4/nokey/spaceflight/spaceflight_news.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.464011 nokey-0.7.4/nokey/tv_and_film/__init__.py
+-rw-r--r--   0        0        0    44173 2024-05-29 00:22:24.468011 nokey-0.7.4/nokey/tv_and_film/star_trek_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 00:22:24.424011 nokey-0.7.4/nokey/weather/__init__.py
+-rw-r--r--   0        0        0    26611 2024-05-29 00:22:24.428011 nokey-0.7.4/nokey/weather/national_weather_service.py
+-rw-r--r--   0        0        0      711 2024-05-29 00:23:14.120011 nokey-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 nokey-0.7.4/PKG-INFO
```

### Comparing `nokey-0.7.3/LICENSE` & `nokey-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.7.3/README.md` & `nokey-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `nokey-0.7.3/nokey/activities/bored_api.py` & `nokey-0.7.4/nokey/activities/bored_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,145 +2,145 @@
 from .. helperFuncs import make_request as mr
 
 class BoredAPI:
     """
     A class to interact with Bored API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="bored_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://www.boredapi.com/api/"
         self.about = "The Bored API helps you find things to do when you're bored. There are fields like the number of participants, activity type, and more that help you narrow down your results."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Bored API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://www.boredapi.com/documentation"
         
     def get_random_activity(self):
         """
         Returns a random activity with related information.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing an activity along with related information.
+            dict: A dictionary containing an activity along with related information.
         """
         endpoint = "activity"
         return mr.make_request(self.base_url+endpoint)
         
     def get_activity_by_key(self, key):
         """
         Returns an activity by its key.
         
         Args:
-        - key (int): A unique number identifying a specific activity listed in the API (from 1000001 to 9999998).
+            key (int): A unique number identifying a specific activity listed in the API (from 1000001 to 9999998).
         
         Returns:
-        - dict: A dictionary containing a specific activity along with related information.
+            dict: A dictionary containing a specific activity along with related information.
         """
         endpoint = f"activity/?key={key}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_by_type(self, activityType):
         """
         Returns a random activity by its type.
         
         Args:
-        - activityType (str): The type of activity. Supported values are education, recreational, social, diy, charity, cooking, relaxation, music, busywork.
+            activityType (str): The type of activity. Supported values are education, recreational, social, diy, charity, cooking, relaxation, music, busywork.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?type={activityType}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_by_participants(self, numParticipants):
         """
         Returns a random activity by its number of participants.
         
         Args:
-        - numParticipants (int): The number of participants required by the activity. Supported values are 1 to n.
+            numParticipants (int): The number of participants required by the activity. Supported values are 1 to n.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?participants={numParticipants}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_by_price(self, price):
         """
         Returns a random activity by a specified price.
         
         Args:
-        - price (float): The price of the activity, as imagined within a range from 0.0 to 1.0.
+            price (float): The price of the activity, as imagined within a range from 0.0 to 1.0.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?price={price}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_within_price_range(self, minprice, maxprice):
         """
         Returns a random activity within a specified price range.
         
         Args:
-        - minprice (float): The minimum price of the activity, starting from 0.0.
-        - maxprice (float): The maximum price of the activity, no greater than 1.0.
+            minprice (float): The minimum price of the activity, starting from 0.0.
+            maxprice (float): The maximum price of the activity, no greater than 1.0.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?minprice={minprice}&maxprice={maxprice}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_by_accessibility(self, accessibility):
         """
         Returns a random activity by a specified accessibility.
         
         Args:
-        - accessibility (float): The accessibility of the activity, as imagined within a range from 0.0 to 1.0., with 0.0 being most accessible.
+            accessibility (float): The accessibility of the activity, as imagined within a range from 0.0 to 1.0., with 0.0 being most accessible.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?accessibility={accessibility}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_activity_within_accessibility_range(self, minAccessibility, maxAccessibility):
         """
         Returns a random activity within a specified accessibility range.
         
         Args:
-        - minAccessibility (float): The minimum accessibility of the activity, with 0.0 being the most accessible.
-        - maxAccessibility (float): The maximum accessibility of the activity, no greater than 1.0.
+            minAccessibility (float): The minimum accessibility of the activity, with 0.0 being the most accessible.
+            maxAccessibility (float): The maximum accessibility of the activity, no greater than 1.0.
         
         Returns:
-        - dict: A dictionary containing a random activity along with related information.
+            dict: A dictionary containing a random activity along with related information.
         """
         endpoint = f"activity/?minaccessibility={minAccessibility}&maxaccessibility={maxAccessibility}"
         return mr.make_request(self.base_url+endpoint)
      
    
   
   
         
         
     
     
     
     
-        
+
```

### Comparing `nokey-0.7.3/nokey/animals/dog_api.py` & `nokey-0.7.4/nokey/animals/dog_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,97 +2,97 @@
 from .. helperFuncs import make_request as mr
 
 class DogAPI:
     """
     A class to interact with the Dog API.
     
     Attributes:
-    - base_url: The base URL for the API.
-    - about: A short description of the API.
+        base_url: The base URL for the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="dog_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://dog.ceo/api/"
         self.about = "The Dog API returns URLs for dog images, either at random or by breed."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
         
     def get_docs_url(self):
         """
         Returns the URL for the Dog API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the Dog API documentation.
+            string: The URL for the Dog API documentation.
         """
         return "https://dog.ceo/dog-api/documentation/"
         
     def get_all_dog_breeds(self):
         """
         Returns a list of all the dog breeds in the Dog API.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: Returns a dictionary containing a list of all the dog breeds in the Dog API.
+            dict: Returns a dictionary containing a list of all the dog breeds in the Dog API.
         """
         endpoint = "breeds/list/all"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_dog_image(self):
         """
         Returns the URL for a random dog image.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: Dictionary containing the URL for a random dog image.
+            dict: Dictionary containing the URL for a random dog image.
         """
         endpoint = "breeds/image/random"
         return mr.make_request(self.base_url+endpoint)
         
     def get_dog_images_by_breed(self, breed):
         """
         Returns an array of URLs for images of dogs of the specified breed.
         
         Args:
-        - breed (str): The breed of the dog.
+            breed (str): The breed of the dog.
         
         Returns:
-        - dict: Dictionary containing a list of URLs of images for the specified dog breed.
+            dict: Dictionary containing a list of URLs of images for the specified dog breed.
         """
         endpoint = f"breed/{breed.lower()}/images"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_subBreeds(self, breed):
         """
         Returns a list of all sub-breeds for the specified dog breed.
         
         Args:
-        - breed (str): The breed of the dog.
+            breed (str): The breed of the dog.
         
         Returns:
-        - dict: Dictionary containing a list of all sub-breeds for the specified dog breed.
+            dict: Dictionary containing a list of all sub-breeds for the specified dog breed.
         """
         endpoint = f"breed/{breed.lower()}/list"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_dog_image_by_breed(self, breed):
         """
         Returns the URL for a random dog image of the specified breed.
         
         Args:
-        - breed (str): The breed of the dog.
+            breed (str): The breed of the dog.
         
         Returns:
-        - dict: Dictionary the URL for a random dog image of the specified breed.
+            dict: Dictionary the URL for a random dog image of the specified breed.
         """
         endpoint = f"breed/{breed.lower()}/images/random"
         return mr.make_request(self.base_url+endpoint)
   
    
         
-    
+
```

### Comparing `nokey-0.7.3/nokey/art_and_images/artic.py` & `nokey-0.7.4/nokey/art_and_images/artic.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,2360 +4,2360 @@
 
 @throttle_class(rate_limit=1, period=1)
 class Artic:
     """
     A class for interacting with the Art Institute of Chicago API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - image_api_url: The base URL for accessing the images in this API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        image_api_url: The base URL for accessing the images in this API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="artic_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.artic.edu/api/v1/"
         self.image_api_url ="https://www.artic.edu/iiif/2/"
         self.about = "The Art Institute of Chicago's API provides JSON-formatted data as a REST-style service that allows developers to explore and integrate the museum’s public data into their projects. This API is the same tool that powers our website, our mobile app, and many other technologies in the museum."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Art Institute of Chicago API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://api.artic.edu/docs/"
     
     # Artworks    
     def get_all_artworks(self, page=1, limit=10):
         """
         Returns data about all the artwork at Art Institute of Chicago.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork data.
+            dict: A dictionary containing artwork data.
         """
         endpoint = f"artworks?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_by_id(self, artwork_id):
         """
         Returns data about a specific artwork in the Art Institute of Chicago's database.
         
         Args:
-        - artwork_id (int): A unique number identifying the artwork.
+            artwork_id (int): A unique number identifying the artwork.
         
         Returns:
-        - dict: A dictionary containing data about a specific artwork.
+            dict: A dictionary containing data about a specific artwork.
         """
         endpoint = f"artworks/{artwork_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artworks_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the artwork contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artworks_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artworks_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork data.
+            dict: A dictionary containing artwork data.
         """
         endpoint = f"artworks/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artworks_data_fields(self):
         """
         Returns the list of artwork fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_artworks()["data"][0].keys()
         
     def search_artworks(self, query, page=1, limit=10):
         """
         Returns data about a artwork in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about artwork.
+            dict: A dictionary containing data about artwork.
         """
         endpoint = f"artworks/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
     
     # Places    
     def get_all_artists(self, page=1, limit=10):
         """
         Returns data about all the artists in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artist data.
+            dict: A dictionary containing artist data.
         """
         endpoint = f"artists?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artist_by_id(self, artist_id):
         """
         Returns data about a specific artist in the Art Institute of Chicago's database.
         
         Args:
-        - artist_id (int): A unique number identifying the artist
+            artist_id (int): A unique number identifying the artist
         
         Returns:
-        - dict: A dictionary containing data about a specific artist.
+            dict: A dictionary containing data about a specific artist.
         """
         endpoint = f"artists/{artist_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artists_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the artists contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artists_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artists_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artist data.
+            dict: A dictionary containing artist data.
         """
         endpoint = f"artists/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artists_data_fields(self):
         """
         Returns the list of artist fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_artists()["data"][0].keys()
         
     def search_artists(self, query, page=1, limit=10):
         """
         Returns data about artists in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about artists
+            dict: A dictionary containing data about artists
         """
         endpoint = f"artists/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)        
     
     # Places    
     def get_all_places(self, page=1, limit=10):
         """
         Returns data about all the places in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing places data.
+            dict: A dictionary containing places data.
         """
         endpoint = f"places?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_place_by_id(self, place_id):
         """
         Returns data about a specific place in the Art Institute of Chicago's database.
         
         Args:
-        - place_id (negative int): A unique (negative) number identifying the place.
+            place_id (negative int): A unique (negative) number identifying the place.
         
         Returns:
-        - dict: A dictionary containing data about a specific place.
+            dict: A dictionary containing data about a specific place.
         """
         endpoint = f"places/{place_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_places_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the places contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_places_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_places_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing places data.
+            dict: A dictionary containing places data.
         """
         endpoint = f"places/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_places_data_fields(self):
         """
         Returns the list of places fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_places()["data"][0].keys()
         
     def search_places(self, query, page=1, limit=10):
         """
         Returns data about places in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about places.
+            dict: A dictionary containing data about places.
         """
         endpoint = f"places/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Agents
     def get_all_agents(self, page=1, limit=10):
         """
         Returns data about all the agents in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agents data.
+            dict: A dictionary containing agents data.
         """
         endpoint = f"agents?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_by_id(self, agent_id):
         """
         Returns data about a specific agent in the Art Institute of Chicago's database.
         
         Args:
-        - agent_id (int): A unique number identifying the agent.
+            agent_id (int): A unique number identifying the agent.
         
         Returns:
-        - dict: A dictionary containing data about a specific agent.
+            dict: A dictionary containing data about a specific agent.
         """
         endpoint = f"agents/{agent_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agents_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the agents contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agents_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agents_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agents data.
+            dict: A dictionary containing agents data.
         """
         endpoint = f"agents/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agents_data_fields(self):
         """
         Returns the list of agents fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_agents()["data"][0].keys()
         
     def search_agents(self, query, page=1, limit=10):
         """
         Returns data about agents in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about agents.
+            dict: A dictionary containing data about agents.
         """
         endpoint = f"agents/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Galleries
     def get_all_galleries(self, page=1, limit=10):
         """
         Returns data about all the galleries in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing galleries data.
+            dict: A dictionary containing galleries data.
         """
         endpoint = f"galleries?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_gallery_by_id(self, gallery_id):
         """
         Returns data about a specific gallery in the Art Institute of Chicago's database.
         
         Args:
-        - agent_id (int): A unique number identifying the gallery.
+            agent_id (int): A unique number identifying the gallery.
         
         Returns:
-        - dict: A dictionary containing data about a specific gallery.
+            dict: A dictionary containing data about a specific gallery.
         """
         endpoint = f"galleries/{gallery_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_galleries_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the galleries contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_galleries_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_galleries_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing galleries data.
+            dict: A dictionary containing galleries data.
         """
         endpoint = f"galleries/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_galleries_data_fields(self):
         """
         Returns the list of galleries fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_galleries()["data"][0].keys()
         
     def search_galleries(self, query, page=1, limit=10):
         """
         Returns data about galleries in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about galleries.
+            dict: A dictionary containing data about galleries.
         """
         endpoint = f"galleries/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Exhibitions
     def get_all_exhibitions(self, page=1, limit=10):
         """
         Returns data about all the exhibitions in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing exhibitions data.
+            dict: A dictionary containing exhibitions data.
         """
         endpoint = f"exhibitions?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_exhibition_by_id(self, exhibition_id):
         """
         Returns data about a specific exhibition in the Art Institute of Chicago's database.
         
         Args:
-        - exhibition_id (int): A unique number identifying the exhibition.
+            exhibition_id (int): A unique number identifying the exhibition.
         
         Returns:
-        - dict: A dictionary containing data about a specific exhibition.
+            dict: A dictionary containing data about a specific exhibition.
         """
         endpoint = f"exhibitions/{exhibition_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_exhibitions_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the exhibitions contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_exhibitions_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_exhibitions_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing exhibitions data.
+            dict: A dictionary containing exhibitions data.
         """
         endpoint = f"exhibitions/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_exhibitions_data_fields(self):
         """
         Returns the list of exhibitions fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_exhibitions()["data"][0].keys()
         
     def search_exhibitions(self, query, page=1, limit=10):
         """
         Returns data about exhibitions in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about exhibitions.
+            dict: A dictionary containing data about exhibitions.
         """
         endpoint = f"exhibitions/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Agent Types
     def get_all_agent_types(self, page=1, limit=10):
         """
         Returns data about all the agent types in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agent types data.
+            dict: A dictionary containing agent types data.
         """
         endpoint = f"agent-types?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_type_by_id(self, agent_type_id):
         """
         Returns data about a specific agent type in the Art Institute of Chicago's database.
         
         Args:
-        - agent_type_id (int): A unique number identifying the agent type.
+            agent_type_id (int): A unique number identifying the agent type.
         
         Returns:
-        - dict: A dictionary containing data about a specific agent type.
+            dict: A dictionary containing data about a specific agent type.
         """
         endpoint = f"agent-types/{agent_type_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_types_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the agent types contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agent_types_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agent_types_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agent types data.
+            dict: A dictionary containing agent types data.
         """
         endpoint = f"agent-types/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_types_data_fields(self):
         """
         Returns the list of agent types fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_agent_types()["data"][0].keys()
         
     def search_agent_types(self, query, page=1, limit=10):
         """
         Returns data about agent types in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about agent types.
+            dict: A dictionary containing data about agent types.
         """
         endpoint = f"agent-types/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Agent Roles
     def get_all_agent_roles(self, page=1, limit=10):
         """
         Returns data about all the agent roles in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agent roles data.
+            dict: A dictionary containing agent roles data.
         """
         endpoint = f"agent-roles?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_role_by_id(self, agent_role_id):
         """
         Returns data about a specific agent role in the Art Institute of Chicago's database.
         
         Args:
-        - agent_role_id (int): A unique number identifying the agent role.
+            agent_role_id (int): A unique number identifying the agent role.
         
         Returns:
-        - dict: A dictionary containing data about a specific agent role.
+            dict: A dictionary containing data about a specific agent role.
         """
         endpoint = f"agent-role/{agent_role_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_roles_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the agent roles contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agent_roles_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_agent_roles_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing agent roles data.
+            dict: A dictionary containing agent roles data.
         """
         endpoint = f"agent-roles/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agent_roles_data_fields(self):
         """
         Returns the list of agent roles fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_agent_roles()["data"][0].keys()
         
     def search_agent_roles(self, query, page=1, limit=10):
         """
         Returns data about agent roles in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about agent roles.
+            dict: A dictionary containing data about agent roles.
         """
         endpoint = f"agent-roles/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Artwork place qualifiers
     def get_all_artwork_place_qualifiers(self, page=1, limit=10):
         """
         Returns data about all the artwork place qualifiers in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork place qualifiers data.
+            dict: A dictionary containing artwork place qualifiers data.
         """
         endpoint = f"artwork-place-qualifiers?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_place_qualifier_by_id(self, artwork_place_qualifier_id):
         """
         Returns data about a specific artwork place qualifier in the Art Institute of Chicago's database.
         
         Args:
-        - artwork_place_qualifier_id (int): A unique number identifying the artwork place qualifier.
+            artwork_place_qualifier_id (int): A unique number identifying the artwork place qualifier.
         
         Returns:
-        - dict: A dictionary containing data about a specific artwork place qualifier.
+            dict: A dictionary containing data about a specific artwork place qualifier.
         """
         endpoint = f"artwork-place-qualifier/{artwork_place_qualifier_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_place_qualifiers_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the artwork place qualifiers contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_place_qualifiers_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_place_qualifiers_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork place qualifiers data.
+            dict: A dictionary containing artwork place qualifiers data.
         """
         endpoint = f"artwork-place-qualifiers/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_place_qualifiers_data_fields(self):
         """
         Returns the list of artwork place qualifiers fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_artwork_place_qualifiers()["data"][0].keys()
         
     def search_artwork_place_qualifiers(self, query, page=1, limit=10):
         """
         Returns data about artwork place qualifiers in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about artwork place qualifiers.
+            dict: A dictionary containing data about artwork place qualifiers.
         """
         endpoint = f"artwork-place-qualifiers/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Artwork date qualifiers
     def get_all_artwork_date_qualifiers(self, page=1, limit=10):
         """
         Returns data about all the artwork date qualifiers in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork date qualifiers data.
+            dict: A dictionary containing artwork date qualifiers data.
         """
         endpoint = f"artwork-date-qualifiers?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_date_qualifier_by_id(self, artwork_date_qualifier_id):
         """
         Returns data about a specific artwork date qualifier in the Art Institute of Chicago's database.
         
         Args:
-        - artwork_date_qualifier_id (int): A unique number identifying the artwork date qualifier.
+            artwork_date_qualifier_id (int): A unique number identifying the artwork date qualifier.
         
         Returns:
-        - dict: A dictionary containing data about a specific artwork date qualifier.
+            dict: A dictionary containing data about a specific artwork date qualifier.
         """
         endpoint = f"artwork-date-qualifier/{artwork_date_qualifier_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_date_qualifiers_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the artwork date qualifiers contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_date_qualifiers_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_date_qualifiers_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork date qualifiers data.
+            dict: A dictionary containing artwork date qualifiers data.
         """
         endpoint = f"artwork-date-qualifiers/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_date_qualifiers_data_fields(self):
         """
         Returns the list of artwork date qualifiers fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_artwork_date_qualifiers()["data"][0].keys()
         
     def search_artwork_date_qualifiers(self, query, page=1, limit=10):
         """
         Returns data about artwork date qualifiers in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about artwork date qualifiers.
+            dict: A dictionary containing data about artwork date qualifiers.
         """
         endpoint = f"artwork-date-qualifiers/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Artwork types
     def get_all_artwork_types(self, page=1, limit=10):
         """
         Returns data about all the artwork types in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork type data.
+            dict: A dictionary containing artwork type data.
         """
         endpoint = f"artwork-types?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_type_by_id(self, artwork_type_id):
         """
         Returns data about a specific artwork type in the Art Institute of Chicago's database.
         
         Args:
-        - artwork_type_id (int): A unique number identifying the artwork type.
+            artwork_type_id (int): A unique number identifying the artwork type.
         
         Returns:
-        - dict: A dictionary containing data about a specific artwork type.
+            dict: A dictionary containing data about a specific artwork type.
         """
         endpoint = f"artwork-types/{artwork_type_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_types_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the artwork types contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_types_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_artwork_types_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing artwork types data.
+            dict: A dictionary containing artwork types data.
         """
         endpoint = f"artwork-types/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_artwork_types_data_fields(self):
         """
         Returns the list of artwork types fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_artwork_types()["data"][0].keys()
         
     def search_artwork_types(self, query, page=1, limit=10):
         """
         Returns data about artwork types in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about artwork types.
+            dict: A dictionary containing data about artwork types.
         """
         endpoint = f"artwork-types/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Category Terms
     def get_all_category_terms(self, page=1, limit=10):
         """
         Returns data about all the category terms in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing category terms.
+            dict: A dictionary containing category terms.
         """
         endpoint = f"category-terms?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_category_term_by_id(self, category_term_id):
         """
         Returns data about a specific category term in the Art Institute of Chicago's database.
         
         Args:
-        - category_term_id (str): A unique id identifying the category term.
+            category_term_id (str): A unique id identifying the category term.
         
         Returns:
-        - dict: A dictionary containing data about a specific category term.
+            dict: A dictionary containing data about a specific category term.
         """
         endpoint = f"category-terms/{category_term_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_category_terms_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the category terms contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_category_terms_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_category_terms_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing category terms data.
+            dict: A dictionary containing category terms data.
         """
         endpoint = f"category-terms/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_category_terms_data_fields(self):
         """
         Returns the list of category terms fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_category_terms()["data"][0].keys()
         
     def search_category_terms(self, query, page=1, limit=10):
         """
         Returns data about category terms in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about category terms.
+            dict: A dictionary containing data about category terms.
         """
         endpoint = f"category-terms/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Images
     def get_all_images(self, page=1, limit=10):
         """
         Returns data about all the images in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing image data.
+            dict: A dictionary containing image data.
         """
         endpoint = f"images?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_image_by_id(self, image_id):
         """
         Returns data about a specific image in the Art Institute of Chicago's database.
         
         Args:
-        - image_id (str): A unique id identifying the image.
+            image_id (str): A unique id identifying the image.
         
         Returns:
-        - dict: A dictionary containing data about a specific image.
+            dict: A dictionary containing data about a specific image.
         """
         endpoint = f"images/{image_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_images_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the images contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_images_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_images_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing images data.
+            dict: A dictionary containing images data.
         """
         endpoint = f"images/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_images_data_fields(self):
         """
         Returns the list of images fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_images()["data"][0].keys()
         
     def search_images(self, query, page=1, limit=10):
         """
         Returns data about images in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about images.
+            dict: A dictionary containing data about images.
         """
         endpoint = f"images/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Videos
     def get_all_videos(self, page=1, limit=10):
         """
         Returns data about all the videos in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing videos data.
+            dict: A dictionary containing videos data.
         """
         endpoint = f"videos?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_video_by_id(self, video_id):
         """
         Returns data about a specific video in the Art Institute of Chicago's database.
         
         Args:
-        - video_id (str): A unique id identifying the video.
+            video_id (str): A unique id identifying the video.
         
         Returns:
-        - dict: A dictionary containing data about a specific video.
+            dict: A dictionary containing data about a specific video.
         """
         endpoint = f"videos/{video_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_videos_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the videos contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_videos_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_videos_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing videos data.
+            dict: A dictionary containing videos data.
         """
         endpoint = f"videos/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_videos_data_fields(self):
         """
         Returns the list of videos fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_videos()["data"][0].keys()
         
     def search_videos(self, query, page=1, limit=10):
         """
         Returns data about videos in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about videos.
+            dict: A dictionary containing data about videos.
         """
         endpoint = f"videos/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Sounds
     def get_all_sounds(self, page=1, limit=10):
         """
         Returns data about all the sounds in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sounds data.
+            dict: A dictionary containing sounds data.
         """
         endpoint = f"sounds?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sound_by_id(self, sound_id):
         """
         Returns data about a specific sound in the Art Institute of Chicago's database.
         
         Args:
-        - sound_id (str): A unique id identifying the sound.
+            sound_id (str): A unique id identifying the sound.
         
         Returns:
-        - dict: A dictionary containing data about a specific sound.
+            dict: A dictionary containing data about a specific sound.
         """
         endpoint = f"sounds/{sound_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sounds_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the sounds contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sounds_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sounds_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sounds data.
+            dict: A dictionary containing sounds data.
         """
         endpoint = f"sounds/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sounds_data_fields(self):
         """
         Returns the list of sounds fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_sounds()["data"][0].keys()
         
     def search_sounds(self, query, page=1, limit=10):
         """
         Returns data about sounds in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about sounds.
+            dict: A dictionary containing data about sounds.
         """
         endpoint = f"sounds/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Texts
     def get_all_texts(self, page=1, limit=10):
         """
         Returns data about all the texts in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing texts data.
+            dict: A dictionary containing texts data.
         """
         endpoint = f"texts?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_by_id(self, text_id):
         """
         Returns data about a specific text in the Art Institute of Chicago's database.
         
         Args:
-        - text_id (str): A unique id identifying the text.
+            text_id (str): A unique id identifying the text.
         
         Returns:
-        - dict: A dictionary containing data about a specific text.
+            dict: A dictionary containing data about a specific text.
         """
         endpoint = f"texts/{text_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_texts_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the texts contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_texts_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_texts_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing texts data.
+            dict: A dictionary containing texts data.
         """
         endpoint = f"texts/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_texts_data_fields(self):
         """
         Returns the list of texts fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_texts()["data"][0].keys()
         
     def search_texts(self, query, page=1, limit=10):
         """
         Returns data about texts in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about texts.
+            dict: A dictionary containing data about texts.
         """
         endpoint = f"texts/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Products
     def get_all_products(self, page=1, limit=10):
         """
         Returns data about all the products in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing products data.
+            dict: A dictionary containing products data.
         """
         endpoint = f"products?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_product_by_id(self, product_id):
         """
         Returns data about a specific product in the Art Institute of Chicago's database.
         
         Args:
-        - product_id (int): A unique number identifying the product.
+            product_id (int): A unique number identifying the product.
         
         Returns:
-        - dict: A dictionary containing data about a specific product.
+            dict: A dictionary containing data about a specific product.
         """
         endpoint = f"products/{product_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_products_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the products contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_products_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_products_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing products data.
+            dict: A dictionary containing products data.
         """
         endpoint = f"products/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_products_data_fields(self):
         """
         Returns the list of products fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_products()["data"][0].keys()
         
     def search_products(self, query, page=1, limit=10):
         """
         Returns data about products in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about products.
+            dict: A dictionary containing data about products.
         """
         endpoint = f"products/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Tours
     def get_all_tours(self, page=1, limit=10):
         """
         Returns data about all the tours in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing tours data.
+            dict: A dictionary containing tours data.
         """
         endpoint = f"tours?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tour_by_id(self, tour_id):
         """
         Returns data about a specific tour in the Art Institute of Chicago's database.
         
         Args:
-        - tour_id (int): A unique number identifying the tour.
+            tour_id (int): A unique number identifying the tour.
         
         Returns:
-        - dict: A dictionary containing data about a specific tour.
+            dict: A dictionary containing data about a specific tour.
         """
         endpoint = f"tours/{tour_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tours_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the tours contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_tours_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_tours_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing tours data.
+            dict: A dictionary containing tours data.
         """
         endpoint = f"tours/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tours_data_fields(self):
         """
         Returns the list of tours fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_tours()["data"][0].keys()
         
     def search_tours(self, query, page=1, limit=10):
         """
         Returns data about tours in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about tours.
+            dict: A dictionary containing data about tours.
         """
         endpoint = f"tours/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Mobile Sounds
     def get_all_mobile_sounds(self, page=1, limit=10):
         """
         Returns data about all the mobile sounds in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing mobile sounds data.
+            dict: A dictionary containing mobile sounds data.
         """
         endpoint = f"mobile-sounds?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_mobile_sound_by_id(self, mobile_sound_id):
         """
         Returns data about a specific mobile sound in the Art Institute of Chicago's database.
         
         Args:
-        - mobile_sound_id (int): A unique number identifying the mobile sound.
+            mobile_sound_id (int): A unique number identifying the mobile sound.
         
         Returns:
-        - dict: A dictionary containing data about a specific mobile sound.
+            dict: A dictionary containing data about a specific mobile sound.
         """
         endpoint = f"mobile-sounds/{mobile_sound_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_mobile_sounds_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the mobile sounds contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_mobile_sounds_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_mobile_sounds_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing mobile sounds data.
+            dict: A dictionary containing mobile sounds data.
         """
         endpoint = f"mobile-sounds/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_mobile_sounds_data_fields(self):
         """
         Returns the list of mobile sounds fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_mobile_sounds()["data"][0].keys()
         
     def search_mobile_sounds(self, query, page=1, limit=10):
         """
         Returns data about mobile sounds in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about mobile sounds.
+            dict: A dictionary containing data about mobile sounds.
         """
         endpoint = f"mobile-sounds/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Publications 
     def get_all_publications(self, page=1, limit=10):
         """
         Returns data about all the publications in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing publications data.
+            dict: A dictionary containing publications data.
         """
         endpoint = f"publications?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_publication_by_id(self, publication_id):
         """
         Returns data about a specific publication in the Art Institute of Chicago's database.
         
         Args:
-        - publication_id (int): A unique number identifying the publication.
+            publication_id (int): A unique number identifying the publication.
         
         Returns:
-        - dict: A dictionary containing data about a specific publication.
+            dict: A dictionary containing data about a specific publication.
         """
         endpoint = f"publications/{publication_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_publications_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the publications contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_publications_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_publications_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing publications data.
+            dict: A dictionary containing publications data.
         """
         endpoint = f"publications/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_publications_data_fields(self):
         """
         Returns the list of publications fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_publications()["data"][0].keys()
         
     def search_publications(self, query, page=1, limit=10):
         """
         Returns data about publications in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about publications.
+            dict: A dictionary containing data about publications.
         """
         endpoint = f"publications/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Sections 
     def get_all_sections(self, page=1, limit=10):
         """
         Returns data about all the sections in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sections data.
+            dict: A dictionary containing sections data.
         """
         endpoint = f"sections?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_section_by_id(self, section_id):
         """
         Returns data about a specific section in the Art Institute of Chicago's database.
         
         Args:
-        - section_id (int): A unique number identifying the publication.
+            section_id (int): A unique number identifying the publication.
         
         Returns:
-        - dict: A dictionary containing data about a specific section.
+            dict: A dictionary containing data about a specific section.
         """
         endpoint = f"sections/{section_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sections_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the sections contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sections_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sections_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sections data.
+            dict: A dictionary containing sections data.
         """
         endpoint = f"sections/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sections_data_fields(self):
         """
         Returns the list of sections fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_sections()["data"][0].keys()
         
     def search_sections(self, query, page=1, limit=10):
         """
         Returns data about sections in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about sections.
+            dict: A dictionary containing data about sections.
         """
         endpoint = f"sections/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Sites
     def get_all_sites(self, page=1, limit=10):
         """
         Returns data about all the sites in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sites data.
+            dict: A dictionary containing sites data.
         """
         endpoint = f"sites?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_site_by_id(self, site_id):
         """
         Returns data about a specific site in the Art Institute of Chicago's database.
         
         Args:
-        - site_id (int): A unique number identifying the site.
+            site_id (int): A unique number identifying the site.
         
         Returns:
-        - dict: A dictionary containing data about a specific site.
+            dict: A dictionary containing data about a specific site.
         """
         endpoint = f"sites/{site_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sites_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the sites contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sites_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_sites_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing sites data.
+            dict: A dictionary containing sites data.
         """
         endpoint = f"sites/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sites_data_fields(self):
         """
         Returns the list of sites fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_sites()["data"][0].keys()
         
     def search_sites(self, query, page=1, limit=10):
         """
         Returns data about sites in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about sites.
+            dict: A dictionary containing data about sites.
         """
         endpoint = f"sites/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Events
     def get_all_events(self, page=1, limit=10):
         """
         Returns data about all the events in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing events data.
+            dict: A dictionary containing events data.
         """
         endpoint = f"events?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_by_id(self, event_id):
         """
         Returns data about a specific event in the Art Institute of Chicago's database.
         
         Args:
-        - event_id (int): A unique number identifying the event.
+            event_id (int): A unique number identifying the event.
         
         Returns:
-        - dict: A dictionary containing data about a specific event.
+            dict: A dictionary containing data about a specific event.
         """
         endpoint = f"event/{event_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_events_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the events contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing events data.
+            dict: A dictionary containing events data.
         """
         endpoint = f"events/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_events_data_fields(self):
         """
         Returns the list of events fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_events()["data"][0].keys()
         
     def search_events(self, query, page=1, limit=10):
         """
         Returns data about events in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about events.
+            dict: A dictionary containing data about events.
         """
         endpoint = f"events/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Event Occurrences 
     def get_all_event_occurrences(self, page=1, limit=10):
         """
         Returns data about all the event occurrences in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing event occurrences data.
+            dict: A dictionary containing event occurrences data.
         """
         endpoint = f"event-occurrences?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_occurrence_by_id(self, event_occurrence_id):
         """
         Returns data about a specific event occurrence in the Art Institute of Chicago's database.
         
         Args:
-        - event_occurrence_id (str): A unique id identifying the event occurrence.
+            event_occurrence_id (str): A unique id identifying the event occurrence.
         
         Returns:
-        - dict: A dictionary containing data about a specific event occurrence.
+            dict: A dictionary containing data about a specific event occurrence.
         """
         endpoint = f"event-occurrences/{event_occurrence_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_occurrences_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the event occurrences contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_occurrences_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_occurrences_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing event occurrences data.
+            dict: A dictionary containing event occurrences data.
         """
         endpoint = f"event-occurrences/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_occurrences_data_fields(self):
         """
         Returns the list of event occurrences fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields
+            object: A dict_keys object containing a list of the fields
         """
         return self.get_all_event_occurrences()["data"][0].keys()
         
     def search_event_occurrences(self, query, page=1, limit=10):
         """
         Returns data about event occurrences in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about event occurrences.
+            dict: A dictionary containing data about event occurrences.
         """
         endpoint = f"event-occurrences/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Event Programs
     def get_all_event_programs(self, page=1, limit=10):
         """
         Returns data about all the event programs in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing event programs data.
+            dict: A dictionary containing event programs data.
         """
         endpoint = f"event-programs?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_program_by_id(self, event_program_id):
         """
         Returns data about a specific event program in the Art Institute of Chicago's database.
         
         Args:
-        - event_program_id (int): A unique number identifying the event program.
+            event_program_id (int): A unique number identifying the event program.
         
         Returns:
-        - dict: A dictionary containing data about a specific event program.
+            dict: A dictionary containing data about a specific event program.
         """
         endpoint = f"event-programs/{event_program_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_programs_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the event programs contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_programs_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_events_programs_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing event programs data.
+            dict: A dictionary containing event programs data.
         """
         endpoint = f"event-programs/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_event_programs_data_fields(self):
         """
         Returns the list of event programs fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_event_programs()["data"][0].keys()
         
     def search_event_programs(self, query, page=1, limit=10):
         """
         Returns data about event programs in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about event programs.
+            dict: A dictionary containing data about event programs.
         """
         endpoint = f"event-programs/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Articles
     def get_all_articles(self, page=1, limit=10):
         """
         Returns data about all the articles in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing articles data.
+            dict: A dictionary containing articles data.
         """
         endpoint = f"articles?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_article_by_id(self, article_id):
         """
         Returns data about a specific article in the Art Institute of Chicago's database.
         
         Args:
-        - article_id (int): A unique number identifying the article.
+            article_id (int): A unique number identifying the article.
         
         Returns:
-        - dict: A dictionary containing data about a specific article.
+            dict: A dictionary containing data about a specific article.
         """
         endpoint = f"articles/{article_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_articles_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the articles contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_articles_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_articles_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing articles data.
+            dict: A dictionary containing articles data.
         """
         endpoint = f"articles/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_articles_data_fields(self):
         """
         Returns the list of articles fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_articles()["data"][0].keys()
         
     def search_articles(self, query, page=1, limit=10):
         """
         Returns data about articles in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about articles.
+            dict: A dictionary containing data about articles.
         """
         endpoint = f"articles/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Highlights
     def get_all_highlights(self, page=1, limit=10):
         """
         Returns data about all the highlights in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing highlights data.
+            dict: A dictionary containing highlights data.
         """
         endpoint = f"highlights?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_highlight_by_id(self, highlight_id):
         """
         Returns data about a specific highlight in the Art Institute of Chicago's database.
         
         Args:
-        - highlight_id (int): A unique number identifying the highlight.
+            highlight_id (int): A unique number identifying the highlight.
         
         Returns:
-        - dict: A dictionary containing data about a specific highlight.
+            dict: A dictionary containing data about a specific highlight.
         """
         endpoint = f"highlights/{highlight_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_highlights_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the highlights contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_highlights_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_highlights_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing highlights data.
+            dict: A dictionary containing highlights data.
         """
         endpoint = f"highlights/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_highlights_data_fields(self):
         """
         Returns the list of highlights fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_highlights()["data"][0].keys()
         
     def search_highlights(self, query, page=1, limit=10):
         """
         Returns data about highlights in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about highlights.
+            dict: A dictionary containing data about highlights.
         """
         endpoint = f"highlights/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Static Pages
     def get_all_static_pages(self, page=1, limit=10):
         """
         Returns data about all the static pages in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing static pages data.
+            dict: A dictionary containing static pages data.
         """
         endpoint = f"static-pages?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_static_page_by_id(self, static_page_id):
         """
         Returns data about a specific static page in the Art Institute of Chicago's database.
         
         Args:
-        - static_page_id (int): A unique number identifying the static page.
+            static_page_id (int): A unique number identifying the static page.
         
         Returns:
-        - dict: A dictionary containing data about a specific static page.
+            dict: A dictionary containing data about a specific static page.
         """
         endpoint = f"static-pages/{static_page_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_static_pages_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the static pages contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_static_pages_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_static_pages_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing static pages data.
+            dict: A dictionary containing static pages data.
         """
         endpoint = f"static-pages/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_static_pages_data_fields(self):
         """
         Returns the list of static pages fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_static_pages()["data"][0].keys()
         
     def search_static_pages(self, query, page=1, limit=10):
         """
         Returns data about static pages in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about static pages.
+            dict: A dictionary containing data about static pages.
         """
         endpoint = f"static-pages/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Generic Pages
     def get_all_generic_pages(self, page=1, limit=10):
         """
         Returns data about all the generic pages in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing generic pages data.
+            dict: A dictionary containing generic pages data.
         """
         endpoint = f"generic-pages?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_generic_page_by_id(self, generic_page_id):
         """
         Returns data about a specific generic page in the Art Institute of Chicago's database.
         
         Args:
-        - generic_page_id (int): A unique number identifying the generic page.
+            generic_page_id (int): A unique number identifying the generic page.
         
         Returns:
-        - dict: A dictionary containing data about a specific generic page.
+            dict: A dictionary containing data about a specific generic page.
         """
         endpoint = f"generic-pages/{generic_page_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_generic_pages_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the generic pages contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_generic_pages_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_generic_pages_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing generic pages data.
+            dict: A dictionary containing generic pages data.
         """
         endpoint = f"generic-pages/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_generic_pages_data_fields(self):
         """
         Returns the list of generic pages fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_generic_pages()["data"][0].keys()
         
     def search_generic_pages(self, query, page=1, limit=10):
         """
         Returns data about generic pages in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about generic pages.
+            dict: A dictionary containing data about generic pages.
         """
         endpoint = f"generic-pages/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Press Releases
     def get_all_press_releases(self, page=1, limit=10):
         """
         Returns data about all the press releases in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing press releases data.
+            dict: A dictionary containing press releases data.
         """
         endpoint = f"press-releases?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_press_release_by_id(self, press_release_id):
         """
         Returns data about a specific press release in the Art Institute of Chicago's database.
         
         Args:
-        - press_release_id (int): A unique number identifying the press release.
+            press_release_id (int): A unique number identifying the press release.
         
         Returns:
-        - dict: A dictionary containing data about a specific press release.
+            dict: A dictionary containing data about a specific press release.
         """
         endpoint = f"press-releases/{press_release_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_press_releases_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the press releases contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_press_releases_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_press_releases_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing press releases data.
+            dict: A dictionary containing press releases data.
         """
         endpoint = f"press-releases/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_press_releases_data_fields(self):
         """
         Returns the list of press releases fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_press_releases()["data"][0].keys()
         
     def search_press_releases(self, query, page=1, limit=10):
         """
         Returns data about press releases in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about press releases.
+            dict: A dictionary containing data about press releases.
         """
         endpoint = f"press-releases/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Educator Resources
     def get_all_educator_resources(self, page=1, limit=10):
         """
         Returns data about all the educator resources in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing educator resources data.
+            dict: A dictionary containing educator resources data.
         """
         endpoint = f"educator-resources?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_educator_resource_by_id(self, educator_resource_id):
         """
         Returns data about a specific educator resource in the Art Institute of Chicago's database.
         
         Args:
-        - educator_resource_id (int): A unique number identifying the educator resource.
+            educator_resource_id (int): A unique number identifying the educator resource.
         
         Returns:
-        - dict: A dictionary containing data about a specific educator resource.
+            dict: A dictionary containing data about a specific educator resource.
         """
         endpoint = f"educator-resources/{educator_resource_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_educator_resources_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the educator resources contained in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_educator_resources_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_educator_resources_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing educator resources data.
+            dict: A dictionary containing educator resources data.
         """
         endpoint = f"educator-resources/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_educator_resources_data_fields(self):
         """
         Returns the list of educator resources fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_educator_resources()["data"][0].keys()
         
     def search_educator_resources(self, query, page=1, limit=10):
         """
         Returns data about educator resources in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about educator resources.
+            dict: A dictionary containing data about educator resources.
         """
         endpoint = f"educator-resources/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Digital Catalogs
     def get_all_digital_catalogs(self, page=1, limit=10):
         """
         Returns data about all the digital catalogs in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing digital catalogs data.
+            dict: A dictionary containing digital catalogs data.
         """
         endpoint = f"digital-catalogs?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_catalog_by_id(self, digital_catalog_id):
         """
         Returns data about a specific digital catalog in the Art Institute of Chicago's database.
         
         Args:
-        - digital_catalog_id (int): A unique number identifying the digital catalog.
+            digital_catalog_id (int): A unique number identifying the digital catalog.
         
         Returns:
-        - dict: A dictionary containing data about a specific digital catalog.
+            dict: A dictionary containing data about a specific digital catalog.
         """
         endpoint = f"digital-catalogs/{digital_catalog_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_catalogs_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the digital catalogs in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_digital_catalogs_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_digital_catalogs_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing digital catalogs data.
+            dict: A dictionary containing digital catalogs data.
         """
         endpoint = f"digital-catalogs/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_catalogs_data_fields(self):
         """
         Returns the list of digital catalogs fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_digital_catalogs()["data"][0].keys()
         
     def search_digital_catalogs(self, query, page=1, limit=10):
         """
         Returns data about digital catalogs in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about digital catalogs.
+            dict: A dictionary containing data about digital catalogs.
         """
         endpoint = f"digital-catalogs/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Digital Publication Sections
     def get_all_digital_publication_sections(self, page=1, limit=10):
         """
         Returns data about all the digital publication sections in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing digital publication sections data.
+            dict: A dictionary containing digital publication sections data.
         """
         endpoint = f"digital-publication-sections?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_publication_section_by_id(self, digital_publication_section_id):
         """
         Returns data about a specific digital publication section in the Art Institute of Chicago's database.
         
         Args:
-        - digital_publication_section_id (int): A unique number identifying the digital publication section.
+            digital_publication_section_id (int): A unique number identifying the digital publication section.
         
         Returns:
-        - dict: A dictionary containing data about a specific digital publication section.
+            dict: A dictionary containing data about a specific digital publication section.
         """
         endpoint = f"digital-publication-sections/{digital_publication_section_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_publication_sections_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the digital publication sections in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_digital_publication_sections_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_digital_publication_sections_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing digital publication sections data.
+            dict: A dictionary containing digital publication sections data.
         """
         endpoint = f"digital-publication-sections/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_digital_publication_sections_data_fields(self):
         """
         Returns the list of digital publication sections fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_digital_publication_sections()["data"][0].keys()
         
     def search_digital_publication_sections(self, query, page=1, limit=10):
         """
         Returns data about digital publication sections in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about digital publication sections.
+            dict: A dictionary containing data about digital publication sections.
         """
         endpoint = f"digital-publication-sections/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     # Printed Catalogs
     def get_all_printed_catalogs(self, page=1, limit=10):
         """
         Returns data about all the printed catalogs in Art Institute of Chicago database.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing printed catalogs data.
+            dict: A dictionary containing printed catalogs data.
         """
         endpoint = f"printed-catalogs?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_printed_catalog_by_id(self, printed_catalog_id):
         """
         Returns data about a specific printed catalog in the Art Institute of Chicago's database.
         
         Args:
-        - printed_catalog_id (int): A unique number identifying the printed catalog.
+            printed_catalog_id (int): A unique number identifying the printed catalog.
         
         Returns:
-        - dict: A dictionary containing data about a specific printed catalog.
+            dict: A dictionary containing data about a specific printed catalog.
         """
         endpoint = f"printed-catalogs/{printed_catalog_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_printed_catalogs_by_fields(self, fields, page=1, limit=10):
         """
         Returns data about all the printed catalogs in the ARTIC database, but only by the specified fields.
         
         Args:
-        - field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_printed_catalogs_data_fields function to get the available fields.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Default is 10.
+            field (str): A comma separated, no spaced string of field names. For retrieving only certain fields. Call get_printed_catalogs_data_fields function to get the available fields.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Default is 10.
         
         Returns:
-        - dict: A dictionary containing printed catalogs data.
+            dict: A dictionary containing printed catalogs data.
         """
         endpoint = f"printed-catalogs/?fields={fields}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_printed_catalogs_data_fields(self):
         """
         Returns the list of printed catalogs fields (dictionary keys) used in the ARTIC database.
         
         Args:
-        - None
+            None
         
         Returns:
-        - object: A dict_keys object containing a list of the fields.
+            object: A dict_keys object containing a list of the fields.
         """
         return self.get_all_printed_catalogs()["data"][0].keys()
         
     def search_printed_catalogs(self, query, page=1, limit=10):
         """
         Returns data about printed catalogs in the Art Institute of Chicago's database matching the specified query term and field values.
         
         Args:
-        - query (str): A search term.
+            query (str): A search term.
         
         Returns:
-        - dict: A dictionary containing data about printed catalogs.
+            dict: A dictionary containing data about printed catalogs.
         """
         endpoint = f"printed-catalogs/search?q={query}&page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     #Download Images
     def download_image(self, image_id):
         """
         Downloads a jpg of the image matching the id.
         
         Args:
-        - image_id (str): The unique identifier for the image. These can be obtained from both the images and exhibitions endpoints of the Artic API.
+            image_id (str): The unique identifier for the image. These can be obtained from both the images and exhibitions endpoints of the Artic API.
         
         Returns:
-        - image, str: Downloads an image and returns a string confirming the download.
+            image, str: Downloads an image and returns a string confirming the download.
         """
         endpoint = f"{image_id}/full/843,/0/default.jpg"
         image_bin = mr.make_request_for_content(self.image_api_url+endpoint)
         with open(image_id+".jpg", "wb") as f:
             f.write(image_bin)
         return f"Image with id {image_id} downloaded"
```

### Comparing `nokey-0.7.3/nokey/art_and_images/lorem_picsum.py` & `nokey-0.7.4/nokey/art_and_images/lorem_picsum.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 from .. helperFuncs import make_request as mr
 
 class LoremPicsum:
     """
     A class for interacting with the Lorem Picsum API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="lorem_picsum_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://picsum.photos/"
         self.about = "This is an API for getting placeholder images, a Lorem Ipsum for images."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Lorem Picsum API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://picsum.photos/"
         
     def get_random_image(self, width, height=None, grayscale=False, blur=None):
         """
         Returns the URL for to a random placeholder image with the given dimensions.
         
         Args:
-        - width (int): The width of the image.
-        - height (int): The height of the image. Defaults to None in which case the image is square.
-        - grayscale (boolean): Optional argument for returning a grayscale picture. The default value is False.
-        - blur (int): An option to return a blurred photo. Values range from 1 to 10.
+            width (int): The width of the image.
+            height (int): The height of the image. Defaults to None in which case the image is square.
+            grayscale (bool): Optional argument for returning a grayscale picture. The default value is False.
+            blur (int): An option to return a blurred photo. Values range from 1 to 10.
         
         Returns:
-        string: The URL of the placeholder image.
+            string: The URL of the placeholder image.
         """
         if height is not None:
             if grayscale:
                 if blur is not None:
                     endpoint = f"{width}/{height}?grayscale&blur={blur}"
                     return self.base_url+endpoint
                 else:
@@ -74,20 +74,20 @@
                     return self.base_url+endpoint
             
     def get_image_by_id(self, image_id, width, height=None, grayscale=False, blur=None):
         """
         Returns the URL for a specific image matching the given id number.
         
         Args:
-        - image_id (int): A unique numerical id matching a specific image.
-        - width (int): The width of the image.
-        - height (int): The height of the image. Defaults to None in which case the image is square.
+            image_id (int): A unique numerical id matching a specific image.
+            width (int): The width of the image.
+            height (int): The height of the image. Defaults to None in which case the image is square.
         
         Returns:
-        - string: The URL to the image matching the given parameters.
+            string: The URL to the image matching the given parameters.
         """
         if height is not None:
             if grayscale:
                 if blur is not None:
                     endpoint = f"id/{image_id}/{width}/{height}?grayscale&blur={blur}"
                     return self.base_url+endpoint
                 else:
@@ -118,20 +118,20 @@
             
             
     def get_static_random_image(self, seed, width, height=None, grayscale=False, blur=None):
         """
         Returns the URL for to a random placeholder image with the given dimensions.
         
         Args:
-        - seed (str): A seed term to ensure the same random image is returned each time.
-        - width (int): The width of the image.
-        - height (int): The height of the image. Defaults to None in which case the image is square.
+            seed (str): A seed term to ensure the same random image is returned each time.
+            width (int): The width of the image.
+            height (int): The height of the image. Defaults to None in which case the image is square.
         
         Returns:
-        string: The URL of the placeholder image.
+            string: The URL of the placeholder image.
         """
         if height is not None:
             if grayscale:
                 if blur is not None:
                     endpoint = f"seed/{seed}/{width}/{height}?grayscale&blur={blur}"
                     return self.base_url+endpoint
                 else:
@@ -161,46 +161,46 @@
                     return self.base_url+endpoint
                     
     def list_images(self, page=1, limit=30):
         """
         Returns a list of images in the Lorem Picsum API.
         
         Args:
-        - page (int): The page of images to return. Default is the first page.
-        - limit (int): The number of items per page. Default is 30.
+            page (int): The page of images to return. Default is the first page.
+            limit (int): The number of items per page. Default is 30.
         
         Returns:
-        - list: A list of images in the Lorem Picsum API.
+            list: A list of images in the Lorem Picsum API.
         """
         endpoint = f"v2/list?page={page}&limit={limit}"
         content = requests.get(self.base_url+endpoint)
         return content.text
         
     def get_image_info_by_id(self, image_id):
         """
         Returns info about a specific image matching the given id.
         
         Args:
-        - image_id (int): A number matching a specific image.
+            image_id (int): A number matching a specific image.
         
         Returns:
-        - dict: A dictionary containing info about a specific image.
+            dict: A dictionary containing info about a specific image.
         """
         endpoint = f"id/{image_id}/info"
         return mr.make_request(self.base_url+endpoint)
         
     def get_image_info_by_seed(self, seed):
         """
         Returns info about a specific image matching the given seed.
         
         Args:
-        - seed (str): The seed matching a specific image.
+            seed (str): The seed matching a specific image.
         
         Returns:
-        - dict: A dictionary containing info about a specific image.
+            dict: A dictionary containing info about a specific image.
         """
         endpoint = f"seed/{seed}/info"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/books_and_literature/gutendex.py` & `nokey-0.7.4/nokey/books_and_literature/gutendex.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,132 +2,132 @@
 from .. helperFuncs import make_request as mr
 
 class Gutendex:
     """
     A class for interacting with the Gutendex API.
     
     Attributes:
-    base_url: The base URL for the API.
-    about: A short description of the API.
+        base_url: The base URL for the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="gutendex_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://gutendex.com/books/"
         self.about = "Gutendex is a JSON web API for Project Gutenberg ebook metadata."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Gutendex API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://gutendex.com/"
         
     def get_books(self, page=1, sort="popular", language="en"):
         """
         Returns a list of book metadata contained in the API.
         
         Args:
-        - page (int): The page of the book list. Defaults to the first page.
-        - sort (str): Sort option for the book metadata. The default is popular, based on number of downloads. Other supported values are ascending and descending.
-        - language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
+            page (int): The page of the book list. Defaults to the first page.
+            sort (str): Sort option for the book metadata. The default is popular, based on number of downloads. Other supported values are ascending and descending.
+            language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
        
         Returns:
-        - dict: A dictionary containing the book metadata for the given page.
+            dict: A dictionary containing the book metadata for the given page.
         """
         endpoint = f"?page={page}&sort={sort}&languages={language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_by_id(self, book_id):
         """
         Returns metadata for a single book matching the given id.
         
         Args:
-        - book_id (int): A unique integer identifying the book in the API database.
+            book_id (int): A unique integer identifying the book in the API database.
         
         Returns:
-        - dict: A dictionary containing metadata for a single book.
+            dict: A dictionary containing metadata for a single book.
         """
         endpoint = f"{book_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_books_by_ids(self, book_ids):
         """
         Returns metadata for a single book matching the given id.
         
         Args:
-        - book_ids (str): Comma separated (no spaces) integers, written as a string, identifying the book in the API database.
+            book_ids (str): Comma separated (no spaces) integers, written as a string, identifying the book in the API database.
         
         Returns:
-        - dict: A dictionary containing metadata for a single book.
+            dict: A dictionary containing metadata for a single book.
         """
         endpoint = f"?ids={book_ids}"
         return mr.make_request(self.base_url+endpoint)
         
     def search_books_by_author_and_title(self, author, title, sort="popular", language="en"):
         """
         Returns metadata on books from the given author and/or a give title.
         
         Args:
-        - author (str): Any part of the author's name.
-        - title (str): Any part of the book's title.
-        - sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
-        - language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
+            author (str): Any part of the author's name.
+            title (str): Any part of the book's title.
+            sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
+            language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
         
         Returns:
-        - dict: A dictionary containing metadata on books from the given author and/or given title. 
+            dict: A dictionary containing metadata on books from the given author and/or given title. 
         """
         endpoint = f"?search={author}%20{title}&sort={sort}&languages={language}"
         print(self.base_url+endpoint)
         return mr.make_request(self.base_url+endpoint)
         
     def search_books_by_topic(self, topic, sort="popular", language="en"):
         """
         Returns metadata on books matching the given topic.
         
         Args:
-        - topic (str): The topic to search.
-        - sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
-        - language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
+            topic (str): The topic to search.
+            sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
+            language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
         
         Returns:
-        - dict: A dictionary containing metadata for books matching the given topic.
+            dict: A dictionary containing metadata for books matching the given topic.
         """
         endpoint = f"?topic={topic}&sort={sort}&languages={language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_authors_within_date_range(self, author_year_start, author_year_end, sort="popular", language="en"):
         """
         Returns authors and metadata for their books within the specified year range.
         
         Args:
-        - author_year_start (int): The year marking the beginning of range. Can be negative (for BC era) or positive.
-        - author_year_end (int): The year marking the end of range. Can be negative (for BC era) or positive.
-        - sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
-        - language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
+            author_year_start (int): The year marking the beginning of range. Can be negative (for BC era) or positive.
+            author_year_end (int): The year marking the end of range. Can be negative (for BC era) or positive.
+            sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
+            language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
         
         Returns:
-        - dict: A dictionary containing a list of books whose authors lived within the specified range.
+            dict: A dictionary containing a list of books whose authors lived within the specified range.
         """
         endpoint = f"?author_year_start={author_year_start}&author_year_end={author_year_end}&sort={sort}&languages={language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_authors_before_specified_year(self, author_year_end, sort="popular", language="en"):
         """
         Returns authors and metadata for their books existing before the specified year.
         
         Args:
-        - author_year_end (int): The year before which the author was alive. Can be negative (for BC era) or positive.
-        - sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
-        - language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
+            author_year_end (int): The year before which the author was alive. Can be negative (for BC era) or positive.
+            sort (str): Parameter by which to sort the data. Default is popular, and other supported values are ascending and descending.
+            language (str): The language in which the books are written. Defaults to en (English). Can take multiple comma separated (non-spaced) values.
         
         Returns:
-        - dict: Returns a dictionary containing metadata for books by authors who were alive before the specified year.
+            dict: Returns a dictionary containing metadata for books by authors who were alive before the specified year.
         """
         endpoint = f"?author_year_end={author_year_end}&sort={sort}&languages={language}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/books_and_literature/stephen_king.py` & `nokey-0.7.4/nokey/books_and_literature/stephen_king.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,110 +2,110 @@
 from .. helperFuncs import make_request as mr
 
 class StephenKingAPI:
     """
     A class to interact with the Stephen King API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="stephen_king_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://stephen-king-api.onrender.com/api/"
         self.about = "The Stephen King API is for accessing the varied worked and villains of Stephen King's books and stories. (Note: This API is not entirely up to date.)"
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Stephen King API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://stephen-king-api.onrender.com/"
         
     def get_stephen_king_books(self):
         """
         Returns all of the Stephen King books and related metadata.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing book metadata.
+            dict: A dictionary containing book metadata.
         """
         endpoint = "books"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stephen_king_book_by_id(self, book_id):
         """
         Returns the Stephen King book matching the id, with related metadata.
         
         Args:
-        - book_id (int): A unique number identifying the Stephen King book.
+            book_id (int): A unique number identifying the Stephen King book.
         
         Returns:
-        - dict: A dictionary containing book metadata.
+            dict: A dictionary containing book metadata.
         """
         endpoint = f"book/{book_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stephen_king_short_stories(self):
         """
         Returns all of the Stephen King short stories and related metadata.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing short story metadata.
+            dict: A dictionary containing short story metadata.
         """
         endpoint = "shorts"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stephen_king_short_story_by_id(self, story_id):
         """
         Returns the Stephen King short story matching the id, with related metadata.
         
         Args:
-        - story_id (int): A unique number identifying the Stephen King short story.
+            story_id (int): A unique number identifying the Stephen King short story.
         
         Returns:
-        - dict: A dictionary containing short story metadata.
+            dict: A dictionary containing short story metadata.
         """
         endpoint = f"short/{story_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stephen_king_villains(self):
         """
         Returns all of the Stephen King villains and related metadata.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing villain metadata.
+            dict: A dictionary containing villain metadata.
         """
         endpoint = "villains"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stephen_king_villain_by_id(self, villain_id):
         """
         Returns the Stephen King villain matching the id, with related metadata.
         
         Args:
-        - villain_id (int): A unique number identifying the Stephen King villain.
+            villain_id (int): A unique number identifying the Stephen King villain.
         
         Returns:
-        - dict: A dictionary containing villain metadata.
+            dict: A dictionary containing villain metadata.
         """
         endpoint = f"villain/{villain_id}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/calendar/nager_date.py` & `nokey-0.7.4/nokey/calendar/nager_date.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,100 +3,100 @@
 from .. helperFuncs import make_request as mr
 
 class NagerDate:
     """
     A class to interact with the Nager.Date API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="nager_date_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://date.nager.at/api/v3/"
         self.about = "The Nager.Date API provides a simple way to query the holidays of over 100 countries. It is also possible to query long weekends."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Nager.Date API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://date.nager.at/swagger/index.html"
         
     def get_country_info(self, countryCode):
         """
         Returns information about a given country.
         
         Args:
-        - countryCode (str): The code representing one of over a hundred countries supported by the API.
+            countryCode (str): The code representing one of over a hundred countries supported by the API.
         
         Returns:
-        - dict: A dictionary containing information about the given country.
+            dict: A dictionary containing information about the given country.
         """
         endpoint = f"CountryInfo/{countryCode}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_available_countries(self):
         """
         Returns all the countries available in the API.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing all the countries available in the API.
+            list: A list containing all the countries available in the API.
         """
         endpoint = "AvailableCountries"
         return mr.make_request(self.base_url+endpoint)
         
     def get_long_weekends_by_country(self, year, countryCode):
         """
         Returns a list of long weekends for a given country in a given year.
         
         Args:
-        - year (int): The year in question.
-        - countryCode (str): The code representing one of over a hundred countries supported by the API.
+            year (int): The year in question.
+            countryCode (str): The code representing one of over a hundred countries supported by the API.
         
         Returns:
-        - list: A list containing the long weekends for a given country in a given year.
+            list: A list containing the long weekends for a given country in a given year.
         """
         endpoint = f"LongWeekend/{year}/{countryCode}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_public_holidays(self, year, countryCode):
         """
         Returns a list of public holidays for a given country in a given year.
         
         Args:
-        - year (int): The year in question.
-        - countryCode (str): The code representing one of over a hundred countries supported by the API.
+            year (int): The year in question.
+            countryCode (str): The code representing one of over a hundred countries supported by the API.
         
         Returns:
-        - list: A list containing the public holidays for a given country in a given year.
+            list: A list containing the public holidays for a given country in a given year.
         """
         endpoint = f"PublicHolidays/{year}/{countryCode}"
         return mr.make_request(self.base_url+endpoint)
         
     def is_today_a_public_holiday(self, countryCode, utc_offset=0):
         """
         Returns True if today (UTC time zone) is a public holiday for a given country or False if it is not.
         
         Args:
-        - countryCode (str): The code representing one of over a hundred countries supported by the API.
-        - utc_offset (int): Integer offset from UTC time zone to adjust for one's own time zone.
+            countryCode (str): The code representing one of over a hundred countries supported by the API.
+            utc_offset (int): Integer offset from UTC time zone to adjust for one's own time zone.
         
         Returns:
-        - bool: True if today (UTC time zone) is a public holiday for the given country or False if it is not.
+            bool: True if today (UTC time zone) is a public holiday for the given country or False if it is not.
         """
         endpoint = f"IsTodayPublicHoliday/{countryCode}?offset={utc_offset}"
         url = self.base_url+endpoint
         response = requests.get(url)
         if response.status_code == 200:
             return True
         elif response.status_code == 204:
@@ -107,31 +107,31 @@
             return "Country code is unknown"
             
     def get_public_holdiays_for_next_365(self, countryCode):
         """
         Returns a list of the upcoming public holidays for a given country for the next 365 days.
         
         Args:
-        - countryCode (str): The code representing one of over a hundred countries supported by the API.
+            countryCode (str): The code representing one of over a hundred countries supported by the API.
         
         Returns:
-        - list: A list containing the upcoming public holidays for a given country for the next 365 days.
+            list: A list containing the upcoming public holidays for a given country for the next 365 days.
         """
         endpoint = f"NextPublicHolidays/{countryCode}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_public_holidays_worldwide_for_next_7(self):
         """
         Returns a list of all the public holidays worldwide for the next 7 days.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing all the upcoming public holidays worldwide for the next 7 days.
+            list: A list containing all the upcoming public holidays worldwide for the next 7 days.
         """
         endpoint = "NextPublicHolidaysWorldwide"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/country_info/rest_country.py` & `nokey-0.7.4/nokey/country_info/rest_country.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,147 +3,147 @@
 
 
 class RestCountries:
     """
     A class to interact with the RestCountries API.
     
     Attributes:
-    - base_url: The base URL of the RestCountries API.
-    - about: A short description of the API.
+        base_url: The base URL of the RestCountries API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="rest_country_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://restcountries.com/v3.1/"
         self.about = "REST Countries API is a simple REST API from RapidAPI that provides information about countries in the world In JSON format."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns url for API docs.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: Url for the API documentation.
+            string: Url for the API documentation.
         """
         return "https://restcountries.com/"
     
     def get_country_by_name(self, name):
         """
         Returns information about a country by its name.
 
         Args:
-        - name (str): The name of the country.
+            name (str): The name of the country.
 
         Returns:
-        - dict: Information about the country, or an error if country not found.
+            dict: Information about the country, or an error if country not found.
         """
         endpoint = f"name/{name}"
         return mr.make_request(self.base_url+endpoint)
     
     def get_country_by_code(self, code):
         """
         Returns information about a country by its code (cca2, ccn3, cca3, or cioc).
 
         Args:
-        - code (str): The country code.
+            code (str): The country code.
 
         Returns:
-        - dict: Information about the country, or an error if country not found.
+            dict: Information about the country, or an error if country not found.
         """
         endpoint = f"alpha/{code}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_currency(self, currency):
         """
         Returns information about countries that use a specific currency.
 
         Args:
-        - currency (str): The currency code or name.
+            currency (str): The currency code or name.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the currency, or an error if no countries found.
+            list: A list of dictionaries containing information about countries using the currency, or an error if no countries found.
         """
         endpoint = f"currency/{currency}"
         return mr.make_request(self.base_url+endpoint)
 
     def get_country_by_language(self, language):
         """
         Returns information about countries speaking a given language.
 
         Args:
-        - language (str): The name of the spoken language of the country.
+            language (str): The name of the spoken language of the country.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the language, or an error if no countries found.
+            list: A list of dictionaries containing information about countries using the language, or an error if no countries found.
         """
         endpoint = f"lang/{language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_capital(self, capital):
         """
         Returns information about a country with the given capital
 
         Args:
-        - capital (str): The name of the capital city.
+            capital (str): The name of the capital city.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the capital, or an error if no countries found.
+            list: A list of dictionaries containing information about countries using the capital, or an error if no countries found.
         """
         endpoint = f"capital/{capital}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_region(self, region):
         """
         Returns information about countries based on a given region.
 
         Args:
-        - region (str): The name of the region.
+            region (str): The name of the region.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+            list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"region/{region}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_subregion(self, subregion):
         """
         Returns information about countries based on a given subregion.
 
         Args:
-        - subregion (str): The name of the subregion.
+            subregion (str): The name of the subregion.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+            list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"subregion/{subregion}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_translation(self, translation):
         """
         Returns information about countries based on a translation of the name.
 
         Args:
-        - translation (str): The name in a given translation.
+            translation (str): The name in a given translation.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
+            list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"translation/{translation}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_countries(self):
         """
         Returns information about all countries listed in the API.
 
         Args:
-        - None
+            None
 
         Returns:
-        - list: A list of dictionaries containing information about all the countries, or an error if no data is found.
+            list: A list of dictionaries containing information about all the countries, or an error if no data is found.
         """
         endpoint = "all"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/developer_tools/apis_guru.py` & `nokey-0.7.4/nokey/developer_tools/apis_guru.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,126 +2,126 @@
 from .. helperFuncs import make_request as mr
 
 class APIsGuru:
     """
     A class to interact with the APIs.guru API.
     
     Attributes:
-    - base_url: The base url for the APIs.guru API.
-    - about: A short description of the API.
+        base_url: The base url for the APIs.guru API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="api_gurus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.apis.guru/v2/"
         self.about = "The APIs.guru API is a self-proclaimed Wikipedia for APIs, maintaining an Open API directory."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the APIs.guru API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://apis.guru/api-doc/"
         
     def get_all_providers(self):
         """
         Returns a list of all the providers in the API directory.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of all the providers in the directory.
+            dict: A dictionary containing a list of all the providers in the directory.
         """
         endpoint = "providers.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_apis_by_provider(self, provider):
         """
         Returns a list of all the APIs for a particular provider.
         
         Args:
-        - provider (str): The name of the api provider.
+            provider (str): The name of the api provider.
         
         Returns:
-        - dict: A dictionary containing a list of all the APIs for a particular provider.
+            dict: A dictionary containing a list of all the APIs for a particular provider.
         """
         endpoint = f"{provider}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_service_names_by_provider(self, provider):
         """
         Returns a list of all the services for a particular provider.
         
         Args:
-        - provider (str): The name of the provider.
+            provider (str): The name of the provider.
         
         Returns:
-        - dict: A dictionary containing a list of all the services for a particular provider.
+            dict: A dictionary containing a list of all the services for a particular provider.
         """
         endpoint = f"{provider}/services.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_particular_api_version_no_service_name(self, provider, api):
         """
         Returns the API entry for one specific version of an API where there is no service name.
         
         Args:
-        - provider (str): The name of the provider.
-        - api (str): The api.
+            provider (str): The name of the provider.
+            api (str): The api.
         
         Returns:
-        - dict: A dictionary containing the API entry for one specific version of an API where there is no service name.
+            dict: A dictionary containing the API entry for one specific version of an API where there is no service name.
         """
         endpoint = f"specs/{provider}/{api}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_particular_api_version_with_service_name(self, provider, service, api):
         """
         Returns the API entry for one specific version of an API where there is a s ervice name.
         
         Args:
-        - provider (str): The name of the provider.
-        - service (str): The name of the service.
-        - api (str): The name of the API.
+            provider (str): The name of the provider.
+            service (str): The name of the service.
+            api (str): The name of the API.
         
         Returns:
-        - dict: A dictionary containing the API entry for one specific version of an API where there is a service name.
+            dict: A dictionary containing the API entry for one specific version of an API where there is a service name.
         """
         endpoint = f"specs/{provider}/{service}/{api}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_apis(self):
         """
         Returns a list of all the APIs in the API directory.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of all the APIs in the directory.
+            dict: A dictionary containing a list of all the APIs in the directory.
         """
         endpoint = "list.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_basic_metrics(self):
         """
         Returns basic metrics for the entire API directory.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing basic metrics for the entire directory.
+            dict: A dictionary containing basic metrics for the entire directory.
         """
         endpoint = "metrics.json"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/developer_tools/filter_lists.py` & `nokey-0.7.4/nokey/developer_tools/filter_lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,136 +2,136 @@
 from .. helperFuncs import make_request as mr
 
 class FilterLists:
     """
     A class for interacting with the FilterLists API.
     
     Attributes:
-    - base_url: The base URL of the FilterLists API.
-    - about: A short description of the API.
+        base_url: The base URL of the FilterLists API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="filter_lists_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://filterlists.com/api/directory/"
         self.about = "The FilterLists Directory API provides lists of filters used by AD blockers."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the FilterLists API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://filterlists.com/api/#/"
         
     def get_languages(self):
         """
         Returns the languages targeted by the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of languages targeted by the FilterLists.
+            dict: A dictionary containing a list of languages targeted by the FilterLists.
         """
         endpoint = "languages"
         return mr.make_request(self.base_url+endpoint)
         
     def get_licenses(self):
         """
         Returns the licenses applied to the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of licenses applied to the FilterLists.
+            dict: A dictionary containing a list of licenses applied to the FilterLists.
         """
         endpoint = "licenses"
         return mr.make_request(self.base_url+endpoint)
         
     def get_lists(self):
         """
         Returns the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the FilterLists.
+            dict: A dictionary containing the FilterLists.
         """
         endpoint = "lists"
         return mr.make_request(self.base_url+endpoint)
         
     def get_list_by_id(self, list_id):
         """
         Returns details of a specific FilterList matching the given id.
         
         Args:
-        - list_id (int): A unique numerical identifier for a FilterList.
+            list_id (int): A unique numerical identifier for a FilterList.
         
         Returns:
-        - dict: A dictionary containing details of the FilterList.
+            dict: A dictionary containing details of the FilterList.
         """
         endpoint = f"lists/{list_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_maintainers(self):
         """
         Returns the maintainers of the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the maintainers of the FilterLists.
+            dict: A dictionary containing the maintainers of the FilterLists.
         """
         endpoint = "maintainers"
         return mr.make_request(self.base_url+endpoint)
         
     def get_software(self):
         """
         Returns the software that subscribes to the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the software that subscribes to the FilterLists.
+            dict: A dictionary containing the software that subscribes to the FilterLists.
         """
         endpoint = "software"
         return mr.make_request(self.base_url+endpoint)
         
     def get_syntaxes(self):
         """
         Returns the syntaxes of the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the syntaxes of the FilterLists.
+            dict: A dictionary containing the syntaxes of the FilterLists.
         """
         endpoint = "syntaxes"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tags(self):
         """
         Returns the tags of the FilterLists.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the tags of the FilterLists.
+            dict: A dictionary containing the tags of the FilterLists.
         """
         endpoint = "tags"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/developer_tools/microlink.py` & `nokey-0.7.4/nokey/developer_tools/microlink.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,87 +2,87 @@
 from .. helperFuncs import make_request as mr
 
 class Microlink:
     """
     A class for interacting with the Microlink API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     
     def __init__(self, use_caching=False, cache_name="microlink_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.microlink.io"
         self.about = "Microlink API provides a powerful API for automating any browser action. Free use is limited to 50 requests a day."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Microlink API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://microlink.io/docs/api/getting-started/overview"
         
     def get_metadata_for_target_url(self, url):
         """
         Returns metadata for the target URL.
         
         Args:
-        - url (str): The target URL.
+            url (str): The target URL.
         
         Returns:
-        - dict: A dictionary containing metadata for the target URL.
+            dict: A dictionary containing metadata for the target URL.
         """
         params = {'url': url}
         return mr.make_request_with_params(self.base_url, params)
         
     def get_screenshot_of_target_url(self, url):
         """
         Returns the URL for a screenshot of the target URL.
         
         Args:
-        - url (str): The target URL.
+            url (str): The target URL.
         
         Returns:
-        - string: The URL for the screenshot of the target URL.
+            string: The URL for the screenshot of the target URL.
         """
         params = {'url': url, "screenshot": True}
         metadata = mr.make_request_with_params(self.base_url, params)
         return metadata["data"]["screenshot"]["url"]
         
     def get_pdf_of_target_url(self, url):
         """
         Returns the URL for a pdf of the target URL.
         
         Args:
-        - url (str): The target URL.
+            url (str): The target URL.
         
         Returns:
-        - string: The URL for the pdf of the target URL.
+            string: The URL for the pdf of the target URL.
         """
         params = {'url': url, "pdf": True}
         metadata = mr.make_request_with_params(self.base_url, params)
         return metadata["data"]["pdf"]["url"]
         
     def get_color_palette_for_target_url(self, url):
         """
         Returns metadata containing the predominant color pallette for each image detected over the target URL.
         
         Args:
-        - url (str): The target URL.
+            url (str): The target URL.
         
         Returns:
-        - dict: A dictionary of metadata containing the predominant color pallette for each image detected over the target URL.
+            dict: A dictionary of metadata containing the predominant color pallette for each image detected over the target URL.
         """
         params = {'url': url, "palette": True}
         metadata = mr.make_request_with_params(self.base_url, params)
         return metadata
```

### Comparing `nokey-0.7.3/nokey/developer_tools/url_haus.py` & `nokey-0.7.4/nokey/developer_tools/url_haus.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,186 +5,186 @@
 
 
 class URLHaus:
     """
     A class to interact with the URLHaus API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="urlhaus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://urlhaus-api.abuse.ch/v1/"
         self.about = "URLhaus is a project operated by abuse.ch. The purpose of the project is to collect, track and share malware URLs, helping network administrators and security analysts to protect their network and customers from cyber threats."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the URLHaus API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://urlhaus-api.abuse.ch/"
         
     def get_recent_urls(self, limit=None):
         """
         Returns a list of recent URLs added to URLHaus.
         
         Args:
-        - limit (int): Optional limit of URLs returned. Defaults to None.
+            limit (int): Optional limit of URLs returned. Defaults to None.
         
         Returns:
-        - dict: A dictionary containing a list of recent URLs added to URLHaus.
+            dict: A dictionary containing a list of recent URLs added to URLHaus.
         """
         if limit is not None:
             endpoint = f"urls/recent/limit/{limit}"
         else:
             endpoint = "urls/recent"
         return mr.make_request(self.base_url+endpoint)
         
     def get_recent_payloads(self, limit=None):
         """
         Returns a list of recent payloads seen by URLHaus.
         
         Args:
-        - limit (int): Optional limit of payloads returned. Defaults to None.
+            limit (int): Optional limit of payloads returned. Defaults to None.
         
         Returns:
-        - dict: A dictionary containing a list of recent payloads seen by URLHaus.
+            dict: A dictionary containing a list of recent payloads seen by URLHaus.
         """
         if limit is not None:
             endpoint = f"payloads/recent/limit/{limit}"
         else:
             endpoint = "payloads/recent"
         return mr.make_request(self.base_url+endpoint)
         
     def get_info_about_url(self, url):
         """
         Returns any information URLHaus may have about a specific URL.
         
         Args:
-        - url (str): The URL in question.
+            url (str): The URL in question.
         
         Returns:
-        - dict: A dictionary containing information about a specific URL.
+            dict: A dictionary containing information about a specific URL.
         """
         payload = {"url": f"{url}"}
         endpoint = "url/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def get_info_about_url_by_id(self, urlID):
         """
         Returns any information URLHaus may have about a specific URL.
         
         Args:
-        - urlID (int): The id of the URL in question.
+            urlID (int): The id of the URL in question.
         
         Returns:
-        - dict: A dictionary containing information about a specific URL.
+            dict: A dictionary containing information about a specific URL.
         """
         payload = {"urlid": f"{urlID}"}
         endpoint = "urlid/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def get_info_about_host(self, host):
         """
         Returns any information URLHaus may have about a specific host.
         
         Args:
-        - host (str): The IPv4 address, domain name, or hostname in question.
+            host (str): The IPv4 address, domain name, or hostname in question.
         
         Returns:
-        - dict: A dictionary containing information about a specific host.
+            dict: A dictionary containing information about a specific host.
         """
         payload = {"host": f"{host}"}
         endpoint = "host/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def get_info_about_payload(self, p_load):
         """
         Returns any information URLHaus has about a specific payload (malware sample).
         
         Args:
-        - p_load (str): The MD5 hash or SHA256 hash of the payload (malware sample).
+            p_load (str): The MD5 hash or SHA256 hash of the payload (malware sample).
         
         Returns:
-        - dict: A dictionary containing information about a specific payload.
+            dict: A dictionary containing information about a specific payload.
         """
         payload = {"payload": f"{p_load}"}
         endpoint = "payload/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def get_info_about_tag(self, tag):
         """
         Returns any information URLHaus has about a specific tag.
         
         Args:
-        - tag (str): The tag to query.
+            tag (str): The tag to query.
         
         Returns:
-        - dict: A dictionary containing information about a specific tag.
+            dict: A dictionary containing information about a specific tag.
         """
         payload = {"tag": f"{tag}"}
         endpoint = "tag/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def get_info_about_signature(self, signature):
         """
         Returns any information URLHaus has about a specific signature.
         
         Args:
-        - signature (str): The signature to query.
+            signature (str): The signature to query.
         
         Returns:
-        - dict: A dictionary containing information about a specific signature.
+            dict: A dictionary containing information about a specific signature.
         """
         payload = {"signature": f"{signature}"}
         endpoint = "signature/"
         response = requests.post(self.base_url+endpoint, payload)
         if response.status_code == 200:
             return response.json()
         else:
             return f"Error: {response.status_code}"
             
     def download_malware_sample(self, sha256):
         """
         Downloads a zip file containing the malware sample (payload).
     
         Args:
-        - base_url (str): The base URL of the API.
-        - sha256 (str): The SHA256 hash identifying the malware sample (payload) to be downloaded.
+            base_url (str): The base URL of the API.
+            sha256 (str): The SHA256 hash identifying the malware sample (payload) to be downloaded.
     
         Returns:
-        - str: Path to the downloaded ZIP file if successful, error message otherwise.
+            - str: Path to the downloaded ZIP file if successful, error message otherwise.
         """
         # Define the endpoint and construct the URL
         endpoint = f"download/{sha256}"
         url = self.base_url + endpoint
 
         # Send the GET request
         response = requests.get(url)
```

### Comparing `nokey-0.7.3/nokey/developer_tools/url_shortener.py` & `nokey-0.7.4/nokey/developer_tools/url_shortener.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 
 @throttle_class(rate_limit=200, period=3600)
 class UrlShortener:
     """
     A class for interacting with the URL Shortener API.
     
     Attributes:
-    - base_url: The base URL of the URL Shortener API.
-    - about: A short description of the API.
+        base_url: The base URL of the URL Shortener API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="url_shortener_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://is.gd/create.php?"
         self.about = "This URL Shortener API (from is.gd) is a URL shortener service."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the URL Shortener API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs
+            string: The URL for the API docs
         """
         return "https://is.gd/apishorteningreference.php?"
         
     def shorten_url(self, url, shorturl=None):
         """
         Returns the shortened URL for the given parameters.
         
         Args:
-        - url (str): The original URL to be shortened.
-        - shorturl (str): Optional parameter for a desired short URL if available (case sensitive). Must be between 5 and 30 characters. Defaults to None.
+            url (str): The original URL to be shortened.
+            shorturl (str): Optional parameter for a desired short URL if available (case sensitive). Must be between 5 and 30 characters. Defaults to None.
         
         Returns:
-        - dict: Dictionary containing the shortened URL.
+            dict: Dictionary containing the shortened URL.
         """
         if shorturl is not None:
             if len(shorturl) < 31 and len(shorturl) > 4:
                 endpoint = f"format=json&url={url}&shorturl={shorturl}"
             else:
                 print("Chosen shortened URL must be between 5 and 30 characters")
                 return ""
```

### Comparing `nokey-0.7.3/nokey/education/university_domains_and_names.py` & `nokey-0.7.4/nokey/education/university_domains_and_names.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 from .. helperFuncs import make_request as mr
 
 class UniversityDomainsAndNames:
     """
     A class to interact with the University Domains and Names API.
     
     Attributes:
-    - base_url: The base url for the University Domains and Names API.
-    - about: A short description of the API.
+        base_url: The base url for the University Domains and Names API.
+        about: A short description of the API.
     """
     
     def __init__(self, use_caching=False, cache_name="university_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://universities.hipolabs.com/search?"
         self.about = "This API accesses a list of universities and their domain names."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the url for the University Domains and Names API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://github.com/Hipo/university-domains-list"
         
     def get_university_name_and_domain(self, name, country, offset=None, limit=None):
         """
         Returns university names and domains for the given parameters.
         
         Args:
-        - name (str): Whole or partial name of university in question.
-        - country (str): Country of university in question.
-        - offset (int): Optional pagination parameter to limit search. Defaults to None.
-        - limit (int): Optional pagination parameter to limit number of results. Defaults to None.
+            name (str): Whole or partial name of university in question.
+            country (str): Country of university in question.
+            offset (int): Optional pagination parameter to limit search. Defaults to None.
+            limit (int): Optional pagination parameter to limit number of results. Defaults to None.
         
         Returns:
-        - dict: List containing universities matching parameters with their respective domains.
+            dict: List containing universities matching parameters with their respective domains.
         """
         if offset is not None and limit is not None:
             endpoint = f"name={name}&country={country}&offset={offset}&limit={limit}"
         elif offset is not None:
             endpoint = f"name={name}&country={country}&offset={offset}"
         elif limit is not None:
             endpoint = f"name={name}&country={country}&limit={limit}"
@@ -53,18 +53,18 @@
         return mr.make_request(self.base_url+endpoint)
         
     def update_list(self):
         """
         Forces a refresh of the API, since the API won't automatically update the dataset if it changes.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: An updated, refreshed list of the university dataset.
+            dict: An updated, refreshed list of the university dataset.
         """
         endpoint = "update"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/finance_and_crypto/coinmap.py` & `nokey-0.7.4/nokey/finance_and_crypto/coinmap.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,61 +4,69 @@
 from .. helperFuncs import make_request as mr
 
 class Coinmap:
     """
     A class for interacting with the Coinmap API.
     
     Attributes:
-    - base_url: The base URL of the Coinmap API.
-    - about: A short description of the API.
+        base_url: The base URL of the Coinmap API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="coinmap_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://coinmap.org/api/v1/"
         self.about = "The CoinMap API is a free resource to access data about thousands of crypto merchants, ATMs, grocery stores, shops, cafes, and other venues. This API is really simple to use since it has a flat data structure, doesn't require authorization, and a well-described data format."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Coinmap API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://coinmap.org/api/"
         
-    def get_venues(self, min_lat: Optional[float] = None, max_lat: Optional[float] = None, min_lon: Optional[float] = None,
-                   max_lon: Optional[float] = None, query: Optional[str] = None, category: Optional[str] = None,
-                   owner: Optional[str] = None, upvoter: Optional[str] = None, before: Optional[date] = None,
-                   after: Optional[date] = None, promoted: Optional[bool] = None, limit: Optional[int] = None,
-                   offset: Optional[int] = None):
+    def get_venues(self, min_lat: Optional[float] = None, 
+                        max_lat: Optional[float] = None, 
+                        min_lon: Optional[float] = None,
+                        max_lon: Optional[float] = None, 
+                        query: Optional[str] = None, 
+                        category: Optional[str] = None,
+                        owner: Optional[str] = None, 
+                        upvoter: Optional[str] = None, 
+                        before: Optional[date] = None,
+                        after: Optional[date] = None, 
+                        promoted: Optional[bool] = None, 
+                        limit: Optional[int] = None,
+                        offset: Optional[int] = None):
         """
         Returns a list of venues with crypto ATMs.
         
         Args:
-        - min_lat (float): Minimum latitude (>=)
-        - max_lat (float): Maximum latitude (<=)
-        - min_lon (float): Minimum longitude (>=)
-        - max_lon (float): Maximum longitude (<=)
-        - query (str): Substring search in venue names
-        - category (str): Filter category
-        - owner (str): Venue owner (userhash)
-        - upvoter (str): User who upvoted the venue (userhash)
-        - before (date): Only show venues created before YYYY-MM-DD
-        - after (date): Only show venues created after YYYY-MM-DD
-        - promoted (bool): Show promoted venues (unset = both)
-        - limit (int): Limit number of results
-        - offset (int): Skip first N results
+            min_lat (float): Minimum latitude (>=)
+            max_lat (float): Maximum latitude (<=)
+            min_lon (float): Minimum longitude (>=)
+            max_lon (float): Maximum longitude (<=)
+            query (str): Substring search in venue names
+            category (str): Filter category
+            owner (str): Venue owner (userhash)
+            upvoter (str): User who upvoted the venue (userhash)
+            before (date): Only show venues created before YYYY-MM-DD
+            after (date): Only show venues created after YYYY-MM-DD
+            promoted (bool): Show promoted venues (unset = both)
+            limit (int): Limit number of results
+            offset (int): Skip first N results
         
         Returns:
-        - dict: A dictionary containing a list of venues with crypto ATMs.
+            dict: A dictionary containing a list of venues with crypto ATMs.
         """
         endpoint = "venues"
         params = {}
 
         if min_lat is not None:
             params['lat1'] = min_lat
         if max_lat is not None:
@@ -89,84 +97,84 @@
         return mr.make_request_with_params(self.base_url + endpoint, params=params)
         
     def get_venue_by_id(self, venue_id):
         """
         Returns a venue matching the given id.
         
         Args:
-        - venue_id (str): A unique number identifying a specific venue.
+            venue_id (str): A unique number identifying a specific venue.
         
         Returns:
-        - dict: A dictionary containing information about the venue matching the given id.
+            dict: A dictionary containing information about the venue matching the given id.
         """
         endpoint = f"venues/{venue_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comments_by_venue_id(self, venue_id):
         """
         Returns a list of comments about the venue matching the given id.
         
         Args:
-        - venue_id (str): A unique number identifying a specific venue.
+            venue_id (str): A unique number identifying a specific venue.
         
         Returns:
-        - dict: A dictionary containing a list of comments about the venue matching the given id.
+            dict: A dictionary containing a list of comments about the venue matching the given id.
         """
         endpoint = f"venues/{venue_id}/comments"
         return mr.make_request(self.base_url+endpoint)
         
     def get_ratings_by_venue_id(self, venue_id):
         """
         Returns ratings about the venue matching the given id.
         
         Args:
-        - venue_id (str): A unique number identifying a specific venue.
+            venue_id (str): A unique number identifying a specific venue.
         
         Returns:
-        - dict: A dictionary containing ratings about the venue matching the given id.
+            dict: A dictionary containing ratings about the venue matching the given id.
         """
         endpoint = f"venues/{venue_id}/ratings"
         return mr.make_request(self.base_url+endpoint)
         
     def get_atm_operators(self):
         """
         Returns a list of ATM operators.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of ATM operators.
+            dict: A dictionary containing a list of ATM operators.
         """
         endpoint = "atm-operators"
         return mr.make_request(self.base_url+endpoint)
         
     def get_coins(self):
         """
         Returns a list of coins.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a list of coins.
+            dict: A dictionary containing a list of coins.
         """
         endpoint = "coins"
         return mr.make_request(self.base_url+endpoint)
 
 # LISTED IN THE DOCS AS A VALID ENDPOINT, BUT IT THROWS UP AN ERROR. POSSIBLY DEPRECATED.    
 #    def get_atm_providers(self):
 #        """
 #        Returns a list of ATM providers.
 #        
 #        Args:
-#        - None
+#            None
 #        
 #        Returns:
-#        - dict: A dictionary containing a list of ATM providers.
+#            dict: A dictionary containing a list of ATM providers.
 #        """
 #        endpoint = "providers"
 #        return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.7.4/nokey/finance_and_crypto/exchange_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 from .. helperFuncs import make_request as mr
 
 class ExchangeAPI:
     """
     A class for interacting with Exchange API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="exchange_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@"
         self.about = "ExchangeAPI is a free currency exchange rates API with 150+ currencies and no rate limits."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the ExchangeAPI documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://github.com/fawazahmed0/exchange-api"
         
     def get_available_currencies(self, minified_version=False):
         """
         Returns all the available currencies in the API.
         
         Args:
-        - minified_version (bool): An optional parameter for getting a minified version of the currency list. Default is false.
+            minified_version (bool): An optional parameter for getting a minified version of the currency list. Default is false.
         
         Returns:
-        - dict: A dictionary containing a list of the available currencies.
+            dict: A dictionary containing a list of the available currencies.
         """
         if minified_version:
             endpoint = "latest/v1/currencies.min.json"
             print(endpoint)
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = "latest/v1/currencies.json"
             return mr.make_request(self.base_url+endpoint)
             
     def get_rates_from_base(self, currency_code, date="latest", minified_version=False):
         """
         Returns exchange rates list for the given currency code on the given date.
         
         Args:
-        - currency_code (str): The code for the base currency used to get exchange rates.
-        - date (str): Date for the exchange rates. Default is latest, but other values must be in YYYY-MM-DD format.
-        - minified_version (bool): An optional parameter for getting a minified version of the currency list. Default is false.
+            currency_code (str): The code for the base currency used to get exchange rates.
+            date (str): Date for the exchange rates. Default is latest, but other values must be in YYYY-MM-DD format.
+            minified_version (bool): An optional parameter for getting a minified version of the currency list. Default is false.
         
         Returns:
-        - dict: A dictionary containing a list of exchange rates.
+            dict: A dictionary containing a list of exchange rates.
         """
         if minified_version:
             endpoint = f"{date}/v1/currencies/{currency_code.lower()}.min.json"
             print(endpoint)
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"{date}/v1/currencies/{currency_code.lower()}.json"
```

### Comparing `nokey-0.7.3/nokey/finance_and_crypto/wallstreet_bets.py` & `nokey-0.7.4/nokey/finance_and_crypto/wallstreet_bets.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,42 +3,41 @@
 
 
 class WallstreetBets:
     """
     A class to interact with the Wallstreet Bets API.
     
     Attributes:
-    - base_url: The base URL of the Wallstreet Bets API.
-    - about: A short description of the API.
+        base_url: The base URL of the Wallstreet Bets API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="wallstree_bets_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://tradestie.com/api/v1/apps/reddit"
         self.about = "This API gets the top 50 stocks discussed on the Reddit subreddit, Wallstreetbets"
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Wallstreet Bets API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        -string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://tradestie.com/apps/reddit/api/"       
     
     def get_stock_sentiment_from_reddit(self):
         """
         Returns top 50 stocks discussed on Reddit subeddit - Wallstreetbets.
 
         Args:
-        - None
+            None
 
         Returns:
-        - list: List of dictionaries containing information about subreddit comments of top 50 stocks.
+            list: List of dictionaries containing information about subreddit comments of top 50 stocks.
         """
-        endpoint = None
         return mr.make_request(self.base_url)
```

### Comparing `nokey-0.7.3/nokey/food/fruityvice.py` & `nokey-0.7.4/nokey/food/fruityvice.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,100 +2,100 @@
 from .. helperFuncs import make_request as mr
 
 class Fruityvice:
     """
     A class to interact with the Fruityvice API.
     
     Attributes:
-    - base_url: The base url of the Fruityvice API.
-    - about: A short description of the API.
+        base_url: The base url of the Fruityvice API.
+        about: A short description of the API.
     """
     
     def __init__(self, use_caching=False, cache_name="fruityvice_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.fruityvice.com/api/fruit/"
         self.about = "Fruityvice is an API that provides information on fruits and their nutritional value."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the url for the Fruityvice API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://www.fruityvice.com/doc/index.html"
         
     def get_all_fruit(self):
         """
         Returns all the fruit listed in the Fruityvice API.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: Dictionary containing all the fruit listed in the API.
+            dict: Dictionary containing all the fruit listed in the API.
         """
         endpoint = "all"
         return mr.make_request(self.base_url+endpoint)
         
     def get_fruit_by_nutrition(self, nutrition, minVal=0, maxVal=1000):
         """
         Returns a fruit with its information based on a minimum and maximum range of values for the specified nutritional component.
         
         Args:
-        - nutrition (str): A nutritional component. Possible values are carbohydrates, protein, fat, calories, and sugar.
-        - minVal (float): The minimum value of the range specified for nutritional component (per 100g of the fruit). Defaults to its minimum possible value, which is 0.
-        - maxVal (float): The maximum value of the range specified for nutritional component (per 100g of the fruit). Defaults to its maximum possible value, which is 1000.
+            nutrition (str): A nutritional component. Possible values are carbohydrates, protein, fat, calories, and sugar.
+            minVal (float): The minimum value of the range specified for nutritional component (per 100g of the fruit). Defaults to its minimum possible value, which is 0.
+            maxVal (float): The maximum value of the range specified for nutritional component (per 100g of the fruit). Defaults to its maximum possible value, which is 1000.
         
         Returns:
-        - dict: Dictionary containing information on the fruit matching the specified values.
+            dict: Dictionary containing information on the fruit matching the specified values.
         """
         endpoint = f"{nutrition}?min={minVal}&max={maxVal}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_fruit_by_family(self, family):
         """
         Returns fruit matching the given family.
         
         Args:
-        - family (str): The name of a fruit family.
+            family (str): The name of a fruit family.
         
         Returns:
-        -dict: Dictionary containing fruit of the given family.
+            dict: Dictionary containing fruit of the given family.
         """
         endpoint = f"family/{family}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_fruit_by_genus(self, genus):
         """
         Returns fruit matching the given genus.
         
         Args:
-        - genus (str): The name of a fruit genus.
+            genus (str): The name of a fruit genus.
         
         Returns:
-        -dict: Dictionary containing fruit of the given genus.
+            dict: Dictionary containing fruit of the given genus.
         """
         endpoint = f"genus/{genus}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_fruit_by_order(self, order):
         """
         Returns fruit matching the given order.
         
         Args:
-        - order (str): The name of a fruit order.
+            order (str): The name of a fruit order.
         
         Returns:
-        -dict: Dictionary containing fruit of the given order.
+            dict: Dictionary containing fruit of the given order.
         """
         endpoint = f"order/{order}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/games/free_to_game.py` & `nokey-0.7.4/nokey/games/free_to_game.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,131 +2,131 @@
 from .. helperFuncs import make_request as mr
 
 class FreeToGame:
     """
     Class to interact with the Free To Game API.
     
     Attributes:
-    - base_url: The base URL of the Free To Game API.
-    - about: A short description of the API.
+        base_url: The base URL of the Free To Game API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="freetogame_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.freetogame.com/api/"
         self.about = "The Free To Game API is a way to access programmatically the best free-to-play games and free MMO games."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Free To Game API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        -string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://www.freetogame.com/api-doc"
         
     def get_all_live_games(self, sort_by=None):
         """
         Returns the live games listed in the API.
         
         Args:
-        - sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
+            sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
         
         Returns:
-        - dict: A dictionary containing all the live games listed in the API.
+            dict: A dictionary containing all the live games listed in the API.
         """
         if sort_by is not None:
             endpoint = f"games?sort-by={sort_by}"
         else:
             endpoint = "games"
         return mr.make_request(self.base_url+endpoint)
         
     def get_games_by_platform(self, platform, sort_by=None):
         """
         Returns a list of free games by platform.
         
         Args:
-        - platform (str): The platform on which the game is played. Supported values are pc, browser, or all.
-        - sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
+            platform (str): The platform on which the game is played. Supported values are pc, browser, or all.
+            sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
         
         Returns:
-        - dict: A dictionary containing the free games played on the given platform.
+            dict: A dictionary containing the free games played on the given platform.
         """
         if sort_by is not None:
             endpoint = f"games?platform={platform}&sort-by={sort_by}"
         else:
             endpoint = f"games?platform={platform}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_games_by_category(self, category, sort_by=None):
         """
         Returns a list of free games by category.
         
         Args:
-        - category (str): The category of the game. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
-        - sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
+            category (str): The category of the game. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
+            sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
         
         Returns:
-        - dict: A dictionary containing the free games matching the given category.
+            dict: A dictionary containing the free games matching the given category.
         """
         if sort_by is not None:
             endpoint = f"games?category={category}&sort-by={sort_by}"
         else:
             endpoint = f"games?category={category}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_games_by_platform_and_category(self, platform, category, sort_by=None):
         """
         Returns a list of free games by category.
         
         Args:
-        - platform (str): The platform on which the game is played. Supported values are pc, browser, or all.
-        - category (str): The category of the game. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
-        - sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
+            platform (str): The platform on which the game is played. Supported values are pc, browser, or all.
+            category (str): The category of the game. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
+            sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
         
         Returns:
-        - dict: A dictionary containing the free games matching the given category.
+            dict: A dictionary containing the free games matching the given category.
         """
         if sort_by is not None:
             endpoint = f"games?platform={platform}&category={category}&sort-by={sort_by}"
         else:
             endpoint = f"games?platform={platform}&category={category}"
         return mr.make_request(self.base_url+endpoint)
         
     def filter_games(self, tag, platform="all", sort_by=None):
         """
         Returns a list of free games by category.
         
         Args:
-        - tag (str): The filter tags, representing the categories of the filtered games, period delimited, no spaces. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
-        - platform (str): Optional parameter representing the platform on which the games are played. Default is all, but other supported values are browser and pc.
-        - sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
+            tag (str): The filter tags, representing the categories of the filtered games, period delimited, no spaces. Supported values are mmorpg, shooter, strategy, moba, racing, sports, social, sandbox, open-world, survival, pvp, pve, pixel, voxel, zombie, turn-based, first-person, third-Person, top-down, tank, space, sailing, side-scroller, superhero, permadeath, card, battle-royale, mmo, mmofps, mmotps, 3d, 2d, anime, fantasy, sci-fi, fighting, action-rpg, action, military, martial-arts, flight, low-spec, tower-defense, horror, mmorts.
+            platform (str): Optional parameter representing the platform on which the games are played. Default is all, but other supported values are browser and pc.
+            sort_by (str): Optional parameter by which to sort games if desired. Defaults to None, but supported values are release-date, popularity, alphabetical or relevance.
         
         Returns:
-        - dict: A dictionary containing the free games matching the given category.
+            dict: A dictionary containing the free games matching the given category.
         """
         if sort_by is not None:
             endpoint = f"filter?tag={tag}&platform={platform}&sort-by={sort_by}"
         else:
             endpoint = f"filter?tag={tag}&platform={platform}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_game_by_id(self, gameID):
         """
         Returns information for a single game matching the id.
         
         Args:
-        - gameID (int): A number representing the unique id of the game as listed in the API.
+            gameID (int): A number representing the unique id of the game as listed in the API.
         
         Returns:
-        - dict: A dictionary containing information for the game matching the given id.
+            dict: A dictionary containing information for the game matching the given id.
         """
         endpoint = f"game?id={gameID}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/games/open_trivia_db.py` & `nokey-0.7.4/nokey/games/open_trivia_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,58 +2,58 @@
 from .. helperFuncs import make_request as mr
 
 class OpenTriviaDB:
     """
     A class for interacting with the Open Trivia Database API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="open_trivia_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://opentdb.com/api.php?"
         self.about = "The Open Trivia Database provides a completely free JSON API to retrieve trivia questions for use in programming projects."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Open Trivia Database API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://opentdb.com/api_config.php"
         
     def get_random_trivia_questions(self, amount):
         """
         Returns the specified amount of random trivia questions of various difficulties and subjects, and the answers to those questions.
         
         Args:
-        - amount (int): The number of trivia desired.
+            amount (int): The number of trivia desired.
         
         Returns:
-        - dict: A dictionary containing the specified amount of trivia questions along with relevant data and the answers.
+            dict: A dictionary containing the specified amount of trivia questions along with relevant data and the answers.
         """
         endpoint = f"amount={amount}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_specified_trivia_questions(self, amount, category=None, difficulty=None, q_type=None):
         """
         Returns the specified amount of trivial questions matching the given parameters, along with relevant data and answers to the questions.
         
         Args:
-        - amount (int): The number of trivia questions to return.
-        - category (int): The category of trivia questions desired. Defaults to None, in which case any categories will be returned.
-        - difficulty (str): The difficulty level of the trivia questions. Defaults to None, in which case each question can be any difficulty level. Supported values are easy, medium, and hard.
-        - q_type (str): The type of questions. Defaults to None, in which case the types are random. Supported values are boolean (True or False) and multiple (Multiple Choice).
+            amount (int): The number of trivia questions to return.
+            category (int): The category of trivia questions desired. Defaults to None, in which case any categories will be returned.
+            difficulty (str): The difficulty level of the trivia questions. Defaults to None, in which case each question can be any difficulty level. Supported values are easy, medium, and hard.
+            q_type (str): The type of questions. Defaults to None, in which case the types are random. Supported values are boolean (True or False) and multiple (Multiple Choice).
         """
         category_dict = {"general knowledge": 9, 
                          "books": 10,
                          "film": 11,
                          "music": 12,
                          "musicals and theatres": 13,
                          "television": 14,
```

### Comparing `nokey-0.7.3/nokey/games/shadify.py` & `nokey-0.7.4/nokey/games/shadify.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,104 +2,104 @@
 from .. helperFuncs import make_request as mr
 
 class Shadify:
     """
     A class for interacting with the Shadify API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="shadify_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://shadify.dev/api/"
         self.about = "Shadify is a powerful REST API service provides a collection of different puzzle types, like crosswords, Sudoku, word search and so on. The API allows users to generate data for puzzles, check the correctness of solutions, and configure various parameters to change the difficulty of the puzzles."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Shadify API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://shadify.dev/introduction.html"
         
     # SUDOKU
     def about_sudoku(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Sudoku is a popular number puzzle game. The essence of the game is to fill free cells with numbers from 1 to 9 so that in each row, each column and each small 3×3 square each digit occurs only once."
     
     def generate_random_sudoku(self, fill=30):
         """
         Returns a random sudoku puzzle, both the finished ("grid") and the unfinished ("task") versions.
         
         Args:
-        - fill (int): A number from 0 to 50 that corresponds to the field fill level (as a percentage). Default is 30.
+            fill (int): A number from 0 to 50 that corresponds to the field fill level (as a percentage). Default is 30.
         
         Returns:
-        - dict: A dictionary containing two grids: the unfinished and finished versions of the puzzle.
+            dict: A dictionary containing two grids: the unfinished and finished versions of the puzzle.
         """
         if fill > 50:
             print("Fill value cannot exceed 50.")
             exit()
         endpoint = f"sudoku/generator?fill={fill}"
         return mr.make_request(self.base_url+endpoint)
         
     def check_sudoku(self, puzzle_grid):
         """
         Returns whether or not the provided sudoku grid is correct or not.
         
         Args:
-        - puzzle_grid (array): A two-dimensional grid (list of lists), where each list is a row in the sudoku grid.
+            puzzle_grid (array): A two-dimensional grid (list of lists), where each list is a row in the sudoku grid.
         
         Returns:
-        - dict: A dictionary containing whether or not the given puzzle is correctly solved, as well as which row contains incorrect values.
+            dict: A dictionary containing whether or not the given puzzle is correctly solved, as well as which row contains incorrect values.
         """
         payload = {
                     "task": puzzle_grid
         }
         endpoint = "sudoku/verifier"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=payload)
         
     # TAKUZU
     def about_takuzu(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Takuzu (a.k.a. Binairo) is an entertaining puzzle game with simple rules. All you have to do is to fill a square field of a certain size with two digits (or colors) while following three simple rules: 1) Each column and each row must be unique. 2) Each row and each column must have an equal number of tiles of each digit. 3) No more than two tiles with the same digit in a row (110001 is wrong, 110010 is right)."
         
     def generate_random_takuzu(self, size=8, fill=33):
         """
         Returns a random takuzu puzzle, both the finished ("field") and the unfinished ("task") versions.
         
         Args:
-        - size (int): An even number from 4 to 12, which specifies the size of the field. Default is 8.
-        - fill (int): A number from 0 to 100 that corresponds to the field fill level (as a percentage). Default is 33.
+            size (int): An even number from 4 to 12, which specifies the size of the field. Default is 8.
+            fill (int): A number from 0 to 100 that corresponds to the field fill level (as a percentage). Default is 33.
         
         Returns:
-        - dict: A dictionary containing two grids: the unfinished and finished versions of the puzzle, as well as the size of the grid.
+            dict: A dictionary containing two grids: the unfinished and finished versions of the puzzle, as well as the size of the grid.
         """
         if (size > 12 or size < 4 or size % 2 != 0) and fill > 100:
             print("Size must be an even number between 4 and 12, inclusive; and fill cannot exceed 100.")
             exit()
         if size > 12 or size < 4 or size % 2 != 0:
             print("Size must be an even number between 4 and 12, inclusive.")
             exit()
@@ -110,63 +110,63 @@
         return mr.make_request(self.base_url+endpoint)
         
     def check_takuzu(self, puzzle_grid):
         """
         Returns whether or not the provided takuzu grid is correct or not.
         
         Args:
-        - puzzle_grid (array): A two-dimensional grid (list of lists), where each list is a row in the takuzu grid.
+            puzzle_grid (array): A two-dimensional grid (list of lists), where each list is a row in the takuzu grid.
         
         Returns:
-        - dict: A dictionary containing whether or not the given puzzle is correctly solved, as well as which row contains incorrect values.
+            dict: A dictionary containing whether or not the given puzzle is correctly solved, as well as which row contains incorrect values.
         """
         payload = {
                     "task": puzzle_grid
         }
         endpoint = "takuzu/verifier"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=payload)
         
     # SET (I know nothing about this game or how to make it work, so read the documentation or Wikipedia to learn how it works.)
     def about_set(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Set (card game) – a fascinating card game. The game deck consists of 81 cards, each with one, two, or three of the same symbol (rhombus, oval, or wave) of the same color (red, green, or purple) and texture (shaded, shaded, or outline only). The essence of the game is to find a set - a set of three cards that meets certain conditions."
         
     def get_all_set_cards(self, possible_sets=True):
         """
         Always returns the same array of 81 objects. Each object corresponds to one of the cards.
         
         Args:
-        - possible_sets (bool): A true/false string that enables/disables the search for possible sets in the current layout. The list of possible sets is not necessary for the game and acts only as a hint and evidence that sets exist in the current layout.
+            possible_sets (bool): A true/false string that enables/disables the search for possible sets in the current layout. The list of possible sets is not necessary for the game and acts only as a hint and evidence that sets exist in the current layout.
         
         Returns:
-        - dict: A dictionary containing 
+            dict: A dictionary containing 
         """
         endpoint = f"set/start?possible-sets={possible_sets}"
         return mr.make_request(self.base_url+endpoint)
         
     def load_set_state(self, state, possible_sets=True, action=None, cards=None):
         """
         Always returns the same array of 81 objects. Each object corresponds to one of the cards.
         
         Args:
-        - A string of hyphenated, no spaced numbers representing the state of the cards.
-        - possible_sets (bool): A true/false string that enables/disables the search for possible sets in the current layout. The list of possible sets is not necessary for the game and acts only as a hint and evidence that sets exist in the current layout.
-        - action (str): Optional. The add/remove string, which allows you to perform the appropriate action with the current game state. The add string adds 3 random cards from the current freeCards array to the current layout (available only if the layout size does not exceed 20 cards). The remove string removes the specified combination of three cards from the current layout. To do this you must use the cards parameter. Default is None.
-        - cards (str): Required if action=remove. A string of the form 1-2-3, where each number corresponds to the unique identifier of one of the cards that make up the set. Default is None.
+            state (str): A string of hyphenated, no spaced numbers representing the state of the cards.
+            possible_sets (bool): A true/false string that enables/disables the search for possible sets in the current layout. The list of possible sets is not necessary for the game and acts only as a hint and evidence that sets exist in the current layout.
+            action (str): Optional. The add/remove string, which allows you to perform the appropriate action with the current game state. The add string adds 3 random cards from the current freeCards array to the current layout (available only if the layout size does not exceed 20 cards). The remove string removes the specified combination of three cards from the current layout. To do this you must use the cards parameter. Default is None.
+            cards (str): Required if action=remove. A string of the form 1-2-3, where each number corresponds to the unique identifier of one of the cards that make up the set. Default is None.
         
         Returns:
-        - dict: A dictionary containing 
+            dict: A dictionary containing 
         """
         if action == "remove" and cards is not None:
             endpoint = f"set/{state}?possible-sets={possible_sets}&action={action}&cards={cards}"
         if action == "remove" and cards is None:
             print("If value of action is 'removed,' cards cannot be None.")
             exit()
         if action == "add":
@@ -177,158 +177,158 @@
         
     # MATH
     def about_math(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "A module for generating random mathematical expressions. Great for creating various simulators, where you'll have to wiggle your brain."
         
     def generate_addition(self, min_first=1, max_first=99, min_second=1, max_second=99):
         """
         Returns a generated addition expression.
         
         Args:
-        - min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
-        - max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
-        - min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
-        - max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.   
+            min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
+            max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
+            min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
+            max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.   
         
         Returns:
-        - dict: A dictionary containing the generated expression.
+            dict: A dictionary containing the generated expression.
         """
         endpoint = f"math/add?min-first={min_first}&max-first={max_first}&min-second={min_second}&max-second={max_second}"
         return mr.make_request(self.base_url+endpoint)
         
     def generate_subtraction(self, min_first=1, max_first=99, min_second=1, max_second=99, negative=0):
         """
         Returns a generated subtraction expression.
         
         Args:
-        - min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
-        - max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
-        - min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
-        - max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.
-        - negative (int): Optional. The number 0/1 which enables/disables the possibility of generating a result with a negative value for expressions with subtraction. Initially, when generating an expression with subtraction, the first number is always greater than the second number. To change this behavior, use this parameter. Default is 0.   
+            min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
+            max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
+            min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
+            max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.
+            negative (int): Optional. The number 0/1 which enables/disables the possibility of generating a result with a negative value for expressions with subtraction. Initially, when generating an expression with subtraction, the first number is always greater than the second number. To change this behavior, use this parameter. Default is 0.   
         
         Returns:
-        - dict: A dictionary containing the generated expression.
+            dict: A dictionary containing the generated expression.
         """
         endpoint = f"math/sub?min-first={min_first}&max-first={max_first}&min-second={min_second}&max-second={max_second}&negative={negative}"
         return mr.make_request(self.base_url+endpoint)
         
     def generate_multiplication(self, min_first=1, max_first=99, min_second=1, max_second=99):
         """
         Returns a generated multiplication expression.
         
         Args:
-        - min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
-        - max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
-        - min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
-        - max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.
+            min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
+            max_first (int): Optional. Maximum value of the first number in the expression. Default is 99.
+            min_second (int): Optional. Minimum value of the second number in the expression. Default is 1.
+            max_second (int): Optional. Maximum value of the second number in the expression. Default is 99.
         
         Returns:
-        - dict: A dictionary containing the generated expression.
+            dict: A dictionary containing the generated expression.
         """
         endpoint = f"math/mul?min-first={min_first}&max-first={max_first}&min-second={min_second}&max-second={max_second}"
         return mr.make_request(self.base_url+endpoint)
         
     def generate_division(self, min_first=1, max_first=99):
         """
         Returns a generated division expression.
         
         Args:
-        - min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
-        - max_first (int): Optional. Maximum value of the first number in the expression. Default is 99. 
+            min_first (int): Optional. Minimum value of the first number in the expression. Default is 1.
+            max_first (int): Optional. Maximum value of the first number in the expression. Default is 99. 
         
         Returns:
-        - dict: A dictionary containing the generated expression.
+            dict: A dictionary containing the generated expression.
         """
         endpoint = f"math/div?min-first={min_first}&max-first={max_first}"
         return mr.make_request(self.base_url+endpoint)
         
     def generate_quadratic_equation(self, min_a=1, max_a=20, min_b=1, max_b=40, min_c=1, max_c=20):
         """
         Returns a generated quadratic equation.
         
         Args:
-        - min_a (int): Minimum value of coefficient a. Default is 1.
-        - max_a (int): Maximum value of coefficient a. Default is 20.
-        - min_b (int): Minimum value of coefficient b. Default is 1.
-        - max_b (int): Maximum value of coefficient b. Default is 40.
-        - min_c (int): Minimum value of coefficient c. Default is 1.
-        - max_c (int): Maximum value of coefficient c. Default is 20.
+            min_a (int): Minimum value of coefficient a. Default is 1.
+            max_a (int): Maximum value of coefficient a. Default is 20.
+            min_b (int): Minimum value of coefficient b. Default is 1.
+            max_b (int): Maximum value of coefficient b. Default is 40.
+            min_c (int): Minimum value of coefficient c. Default is 1.
+            max_c (int): Maximum value of coefficient c. Default is 20.
        
         Returns:
-        - dict: A dictionary containing the generated equation.
+            dict: A dictionary containing the generated equation.
         """
         endpoint = f"math/quad?min-a={min_a}&max-a={max_a}&min-b={min_b}&max-b={max_b}&min-c={min_c}&max-c={max_c}"
         return mr.make_request(self.base_url+endpoint)
         
     
     # SCHULTE TABLES
     def about_schulte(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Schulte Tables – tables with randomly arranged objects (usually numbers or letters) used to test and develop quickness of finding these objects in a certain order (usually in ascending order for numbers and alphabetical order for letters). Exercises with tables can improve peripheral visual perception, which will have a positive impact on the skill of speed reading."
         
     def generate_random_schulte_table(self, size=5, mode="number"):
         """
         Returns a random schulte table.
         
         Args:
-        - size (int): The size of the generated table. The available range is from 1 to 15. Default is 5.
-        - mode (str) The number / alphabet string, which defines the generated values for the table: numbers or letters. If alphabet is selected, the size parameter will always be 5. Default is number
+            size (int): The size of the generated table. The available range is from 1 to 15. Default is 5.
+            mode (str) The number / alphabet string, which defines the generated values for the table: numbers or letters. If alphabet is selected, the size parameter will always be 5. Default is number
         
         Returns:
-        - dict: A dictionary containing a grid representing the schulte table.
+            dict: A dictionary containing a grid representing the schulte table.
         """
         if size < 1 or size > 15:
             print("Size must be between 1 and 15, inclusive.")
             exit()
         endpoint = f"schulte/generator?size={size}&mode={mode}"
         return mr.make_request(self.base_url+endpoint)  
         
     # MINESWEEPER
     def about_minesweeper(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Minesweeper – a computer puzzle game in which the playing field is divided into adjacent cells, some of which are mined. The number of mined cells is known. The goal of the game is to open all the cells that do not contain mines. This game has become quite popular among Windows users, since it was pre-installed by default on older versions of that OS."
 
     def generate_random_minesweeper_field(self, start, width=9, height=9, mines=12):
         """
         Returns a randomly generated minesweeper grid.
         
         Args:
-        - start (str): A string of the form 1-2, which sets the starting position of the player. There will never be mines in and around this position. The first number is the X coordinate (from 1 to the value of the widht parameter), the second number is the Y coordinate (from 1 to the value of the height parameter).
-        - width (int): The number that sets the width of the generated field. The total number of cells in the field must not exceed 1000. Default is 9.
-        - height (int): The number that sets the height of the generated field. The total number of cells in the field must not exceed 1000. Default is 9.
-        - mines (int): The number that sets the number of mines on the field. The number of mines must not exceed 25% of the total number of cells on the field. Default is 12.
+            start (str): A string of the form 1-2, which sets the starting position of the player. There will never be mines in and around this position. The first number is the X coordinate (from 1 to the value of the widht parameter), the second number is the Y coordinate (from 1 to the value of the height parameter).
+            width (int): The number that sets the width of the generated field. The total number of cells in the field must not exceed 1000. Default is 9.
+            height (int): The number that sets the height of the generated field. The total number of cells in the field must not exceed 1000. Default is 9.
+            mines (int): The number that sets the number of mines on the field. The number of mines must not exceed 25% of the total number of cells on the field. Default is 12.
         
         Returns:
-        - dict: A dictionary containing the minesweeper board grid and other data.
+            dict: A dictionary containing the minesweeper board grid and other data.
         """
         if width * height > 1000:
             print(f"The width and height given would result in {width*height} cells, but total cells must not exceed 1000. Adjust dimensions accordingly.")
             exit()
         if mines > .25 * width * height:
             print(f"Number of mines given would be {mines/(width*height)} of total cells, but number of mines may not exceed .25 of total cells. Adjust number of mines accordingly.")
             exit()
@@ -337,31 +337,31 @@
         
     # WORDSEARCH
     def about_wordsearch(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Word search is a puzzle consisting of letters of words placed in a square or rectangular grid. The aim of the puzzle is to find and mark all the words hidden in the grid. The words can be placed horizontally, vertically or diagonally."
         
     def generate_random_wordsearch_grid(self, width=9, height=9):
         """
         Returns a randomly generated wordsearch grid.
         
         Args:
-        - width (int): A number from 5 to 20 that specifies the width of the grid. The total number of cells in the field must not exceed 256. Default is 9.
-        - height (int): A number from 5 to 20 that specifies the width of the grid. The total number of cells in the field must not exceed 256. Default is 9.
+            width (int): A number from 5 to 20 that specifies the width of the grid. The total number of cells in the field must not exceed 256. Default is 9.
+            height (int): A number from 5 to 20 that specifies the width of the grid. The total number of cells in the field must not exceed 256. Default is 9.
         
         Returns:
-        - dict: Returns a dictionary containing the wordsearch grid and the key.
+            dict: Returns a dictionary containing the wordsearch grid and the key.
         """
         if width < 5 or width > 20:
             print("Value of width must be between 5 and 20, inclusive.")
             exit()
         if height < 5 or height > 20:
             print("Value of height must be between 5 and 20, inclusive.")
             exit()
@@ -373,57 +373,57 @@
         
     # ANAGRAMS
     def about_anagram(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Anagrams is a whole type of puzzles associated with composing all possible words from a given set of letters. This module implements the simplest variation of anagrams: a random word is given, the letters of which should be used to compose as many other words as possible."
         
     def generate_random_anagram(self):
         """
         Returns a word as the task and the possible words that can be composed from the word.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing a task word and a list of words that can be composed from this word.
+            dict: A dictionary containing a task word and a list of words that can be composed from this word.
         """
         endpoint = "anagram/generator"
         return mr.make_request(self.base_url+endpoint)
         
     # COUNTRIES
     def about_countries(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Countries module allows you to generate quizes such as guess the capital or guess the country from an image of the flag. It is a simple and useful module for creating applications to test and practice knowledge of all countries."
         
     def generate_capital_quiz(self, variants=4, amount=1):
         """
         Returns a country capital quiz and answer the the quiz.
         
         Args:
-        - variants (int): Optional. A number from 2 to 6 corresponding to the number of different options from which you have to choose the correct capital of the given country. Default is 4.
-        - amount (int): Optional. A number from 1 to 20 which is responsible for the number of quizzes returned. The use of this parameter ensures that among all quizzes received, all will be unique. Default is 1.
+            variants (int): Optional. A number from 2 to 6 corresponding to the number of different options from which you have to choose the correct capital of the given country. Default is 4.
+            amount (int): Optional. A number from 1 to 20 which is responsible for the number of quizzes returned. The use of this parameter ensures that among all quizzes received, all will be unique. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a country name, a link to its flag, possible answers for its capital, and correct answer.
+            dict: A dictionary containing a country name, a link to its flag, possible answers for its capital, and correct answer.
         """
         if variants < 2 or variants > 6:
             print("Value of variants must be between 2 and 6, inclusive. Please adjust value accordingly.")
             exit()
         if amount < 1 or amount > 20:
             print("Value of amount must be between 1 and 20, inclusive. Please adjust value accordingly.")
             exit()
@@ -431,19 +431,19 @@
         return mr.make_request(self.base_url+endpoint)
         
     def generate_country_quiz(self, variants=4, amount=1):
         """
         Returns a country capital quiz and answer the the quiz.
         
         Args:
-        - variants (int): Optional. A number from 2 to 6 corresponding to the number of different options from which you have to choose the the correct country of the given flag image. Default is 4.
-        - amount (int): Optional. A number from 1 to 20 which is responsible for the number of quizzes returned. The use of this parameter ensures that among all quizzes received, all will be unique. Default is 1.
+            variants (int): Optional. A number from 2 to 6 corresponding to the number of different options from which you have to choose the the correct country of the given flag image. Default is 4.
+            amount (int): Optional. A number from 1 to 20 which is responsible for the number of quizzes returned. The use of this parameter ensures that among all quizzes received, all will be unique. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a link to a country's flag, possible answers for the country, and correct answer.
+            dict: A dictionary containing a link to a country's flag, possible answers for the country, and correct answer.
         """
         if variants < 2 or variants > 6:
             print("Value of variants must be between 2 and 6, inclusive. Please adjust value accordingly.")
             exit()
         if amount < 1 or amount > 20:
             print("Value of amount must be between 1 and 20, inclusive. Please adjust value accordingly.")
             exit()
@@ -452,32 +452,32 @@
         
     # CAMP
     def about_camp(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Camp (aka Tents and trees, Tents) is a logic puzzle with simple rules and challenging solutions. The rules of Camp are simple: 1) Pair each tree with a tent adjacent horizontally or vertically. This should be a 1 to 1 relation. 2) Tents never touch each other even diagonally. 3) The clues outside the grid indicate the number of tents on that row/column."
     
     def generate_random_camp_task(self, width=7, height=7, solution=True):
         """
         Returns a camp game grid and the solution.
         
         Args:
-        - width (int): Optional. A number from 5 to 15 which corresponds to the width of the generated field. Default is 7.
-        - height (int): Optional. A number from 5 to 15 which corresponds to the height of the generated field. Default is 7.
-        - solution (bool): Optional. The true/false value that specifies whether the solution should be sent with the task or not. Default is True.
+            width (int): Optional. A number from 5 to 15 which corresponds to the width of the generated field. Default is 7.
+            height (int): Optional. A number from 5 to 15 which corresponds to the height of the generated field. Default is 7.
+            solution (bool): Optional. The true/false value that specifies whether the solution should be sent with the task or not. Default is True.
         
         Returns:
-        - dict: A dictionary containing the camp grid task and the solution if solution is True.
+            dict: A dictionary containing the camp grid task and the solution if solution is True.
         """
         if width < 5 or width > 15:
             print("Value of width must be between 5 and 15, inclusive. Please adjust value accordingly.")
             exit()
         if height < 5 or height > 15:
             print("Value of height must be between 5 and 15, inclusive. Please adjust value accordingly.")
             exit()
@@ -485,20 +485,20 @@
         return mr.make_request(self.base_url+endpoint)
         
     def check_camp_task(self, row_tents, column_tents, solution):
         """
         Checks the given camp task grid and returns whether or not it is correct.
         
         Args:
-        - row_tents (list): A list containing the row tents values.
-        - column_tents (list). A list containing the column tents values.
-        - solution (array): A two dimensional array containing the solution grid.
+            row_tents (list): A list containing the row tents values.
+            column_tents (list). A list containing the column tents values.
+            solution (array): A two dimensional array containing the solution grid.
         
         Returns:
-        - dict: A dictionary containing whether or not the solution is valid, where the error occurs if it is not, and a message.
+            dict: A dictionary containing whether or not the solution is valid, where the error occurs if it is not, and a message.
         """
         payload = {
                 "rowTents": row_tents,
                 "columnTents": column_tents,
                 "solution": solution
         }
         endpoint = "camp/verifier/"
@@ -506,32 +506,32 @@
         
     # KUROMASU
     def about_kuromasu(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Kuromasu is a puzzle played on a rectangular grid. Some of these cells have numbers in them. Each cell may be either black or white. The object is to determine what type each cell is. The following rules determine which cells are which: 1) Each number on the board represents the number of white cells that can be seen from that cell, including itself. A cell can be seen from another cell if both cells are within the same row or column, and there are no black cells between them in that row or column. 2) Numbered cells must not be black. 3) No two black cells must be horizontally or vertically adjacent. 4) All the white cells must be connected horizontally or vertically."
     
     def generate_random_kuromasu_task(self, width=5, height=5, fill=30):
         """
         Returns a kuromasu task grid and the solution.
         
         Args:
-        - width (int): Optional. A number from 4 to 15 which corresponds to the width of the generated field. Default is 5.
-        - height (int): Optional. A number from 4 to 15 which corresponds to the height of the generated field. Default is 5.
-        - fill (int): Optional. A number from 10 to 50 which corresponds to the % level of filling the task with ready cells.
+            width (int): Optional. A number from 4 to 15 which corresponds to the width of the generated field. Default is 5.
+            height (int): Optional. A number from 4 to 15 which corresponds to the height of the generated field. Default is 5.
+            fill (int): Optional. A number from 10 to 50 which corresponds to the % level of filling the task with ready cells.
         
         Returns:
-        - dict: A dictionary containing the kuromasu grid task and the solution.
+            dict: A dictionary containing the kuromasu grid task and the solution.
         """
         if width < 4 or width > 15:
             print("Value of width must be between 4 and 15, inclusive. Please adjust value accordingly.")
             exit()
         if height < 4 or height > 15:
             print("Value of height must be between 4 and 15, inclusive. Please adjust value accordingly.")
             exit()
@@ -541,50 +541,50 @@
         return mr.make_request(self.base_url+endpoint)
         
     def check_kuromasu_task(self, solution):
         """
         Checks the given kuromasu task grid and returns whether or not it is correct.
         
         Args:
-        - solution (array): A two dimensional array containing the solution grid.
+            solution (array): A two dimensional array containing the solution grid.
         
         Returns:
-        - dict: A dictionary containing whether or not the solution is valid, where the error occurs if it is not.
+            dict: A dictionary containing whether or not the solution is valid, where the error occurs if it is not.
         """
         payload = {
                 "solution": solution
         }
         endpoint = "kuromasu/verifier/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=payload)
         
     # MEMORY
     def about_memory(self):
         """
         Returns a short description of the game.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: A short description of the game.
+            string: A short description of the game.
         """
         return "Memory is a puzzle that's great for practicing memorization. You are given a field with a random set of elements, and each element in the field occur several times (usually 2 or 3). You have some time to remember the position of all the elements on the field, and then all of them are hidden and your task is to open pairs of identical elements one by one trying to make as few mistakes as possible."
   
     def generate_random_memory_grid(self, width=6, height=4, pair_size=3, show_positions=True):
         """
         Returns a memory grid and pair positions.
         
         Args:
-        - width (int). Optional. A number corresponding to the width of the generated grid. The total number of cells in the grid must not exceed 52 multiplied by the pair-size. Default is 6.
-        - height (int): Optional. A number corresponding to the height of the generated grid. The total number of cells in the grid must not exceed 52 multiplied by the pair-size. Default is 4.
-        - pair_size (int): Optional. A number corresponding to the size of a pair of identical elements. The value must be a multiple of the total number of cells in the grid. Available values: 2, 3, 4. Default is 3.
-        - show_positions (bool): Optional. A true/false value that determines whether to send position information for each pair of elements. Default is True.
+            width (int). Optional. A number corresponding to the width of the generated grid. The total number of cells in the grid must not exceed 52 multiplied by the pair-size. Default is 6.
+            height (int): Optional. A number corresponding to the height of the generated grid. The total number of cells in the grid must not exceed 52 multiplied by the pair-size. Default is 4.
+            pair_size (int): Optional. A number corresponding to the size of a pair of identical elements. The value must be a multiple of the total number of cells in the grid. Available values: 2, 3, 4. Default is 3.
+            show_positions (bool): Optional. A true/false value that determines whether to send position information for each pair of elements. Default is True.
         
         Returns:
-        - dict: A dictionary containing a memory grid and pair positions.
+            dict: A dictionary containing a memory grid and pair positions.
         """
         if width * height > 52 * pair_size:
             print(f"The total number of cells in the grid are {width*height}, but total cells must not exceed 52 times the pair_size. Please adjust dimensions accordingly.")
             exit()
         endpoint = f"memory/generator?width={width}&height={height}&pair-size={pair_size}&show-positions={show_positions}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/geolocation/ip_api.py` & `nokey-0.7.4/nokey/geolocation/ip_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 @throttle_class(rate_limit=45, period=60)
 class IP_API:
     """
     A class to interact with the IP API.
     
     Attributes:
-    - base_url: The base URL of IP API.
-    - about: A short description of the API.
+        base_url: The base URL of IP API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="ip_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://ip-api.com/json/" 
         self.about = "The IP API is a fast, reliable, and free IP geolocation API."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://ip-api.com/docs"
     
     def get_location_info_by_ip_address(self, ip):
         """
         Returns geolocation info (country, state, coordinates, etc.) by IP address.
 
         Args:
-        - ip (str): IPv4/IPv6 address or domain name.
+            ip (str): IPv4/IPv6 address or domain name.
 
         Returns:
-        - dict: Location information based on given IP address or domain name.
+            dict: Location information based on given IP address or domain name.
         """
         endpoint = f"{ip}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/geolocation/zippopotamus.py` & `nokey-0.7.4/nokey/geolocation/zippopotamus.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 from .. helperFuncs import make_request as mr
 
 class Zippopotomus:
     """
     A class to interact with the Zippopotomus API.
     
     Attributes:
-    - base_url: The basee URL of the API.
-    - about: A short description of the API.
+        base_url: The basee URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="zippopotomus_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://api.zippopotam.us/"
         self.about = "Zippopotamus is an open source project that is focused on converting zip codes into valid geographical locations."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Zippopotomus API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://www.zippopotam.us/"
         
     def get_info_by_zipcode(self, country, zipcode):
         """
         Returns information on a given zipcode in a given country.
         
         Args:
-        - country (str): The country code as defined in the API docs. See docs for supported countries. 
-        - zipcode (int): The zipcode in question. See docs for range and format of zipcodes by country.
+            country (str): The country code as defined in the API docs. See docs for supported countries. 
+            zipcode (int): The zipcode in question. See docs for range and format of zipcodes by country.
         
         Returns:
-        - dict: A dictionary containing information about the given zipcode in the given country.
+            dict: A dictionary containing information about the given zipcode in the given country.
         """
         endpoint = f"{country}/{zipcode}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_zipcode_by_city(self, country, state, city):
         """
         Returns the zipcode(s) of the city matching the parameters.
         
         Args:
-        - country (str): The country code as defined in the API docs.
-        - state (str): The state code.
-        - city (str): The city in question.
+            country (str): The country code as defined in the API docs.
+            state (str): The state code.
+            city (str): The city in question.
         
         Returns:
-        - dict: A dictionary containing the zipcode of the given location.
+            dict: A dictionary containing the zipcode of the given location.
         """
         endpoint = f"{country}/{state}/{city}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/government/federal_register.py` & `nokey-0.7.4/nokey/government/federal_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,92 +2,92 @@
 from .. helperFuncs import make_request as mr
 
 class FederalRegister:
     """
     A class for interacting with the Federal Register API.
     
     Attributes:
-    base_url: The base URL of the API.
-    about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="federal_register_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://www.federalregister.gov/api/v1/"
         self.about = "FederalRegister.gov provides multiple public API endpoints. These can be used to access information in the Federal Register, the daily journal of the US government."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Federal Register API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://www.federalregister.gov/developers/documentation/api/v1"
         
     def get_fed_reg_document(self, document_num):
         """
         Returns a Federal Register document of the given number.
         
         Args:
-        - document_num (str): The unique number for the document.
+            document_num (str): The unique number for the document.
         
         Returns:
-        - dict: A dictionary containing the document matching the given number.
+            dict: A dictionary containing the document matching the given number.
         """
         endpoint = f"documents/{document_num}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_multiple_fed_reg_documents(self, document_nums):
         """
         Returns multiple Federal Register documents of the given numbers.
         
         Args:
-        - document_nums (str): A string of unspaced, comma-separated document numbers.
+            document_nums (str): A string of unspaced, comma-separated document numbers.
         
         Returns:
-        - dict: A dictionary containing the documents matching the given numbers.
+            dict: A dictionary containing the documents matching the given numbers.
         """
         endpoint = f"documents/{document_nums}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def search_all_documents(self, search_term, per_page=20, doc_type=None):
         """
         Returns the Federal Register documents published since 1994 matching the given parameters.
         
         Args:
-        - search_term (str): The term by which to search the documents.
-        - per_page (int): The number of documents to return at once; default is 20; 1000 maximum.
-        - doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
+            search_term (str): The term by which to search the documents.
+            per_page (int): The number of documents to return at once; default is 20; 1000 maximum.
+            doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
         
         Returns:
-        - dict: A dictionary containing the documents published since 1994 matching the given values.
+            dict: A dictionary containing the documents published since 1994 matching the given values.
         """
         if doc_type is not None:
             endpoint = f"documents.json?per_page={per_page}&conditions[term]={search_term}&conditions[type][]={doc_type.upper()}"
             return mr.make_request(self.base_url+endpoint)
         else:            
             endpoint = f"documents.json?per_page={per_page}&conditions[term]={search_term}"
             return mr.make_request(self.base_url+endpoint)
         
     def get_document_counts_by_facet(self, facet, search_term=None, doc_type=None):
         """
         Returns counts of matching Federal Register documents grouped by a facet.
         
         Args:
-        - facet (str): The facet by which to group the documents. Supported values are daily, weekly, monthly, quarterly, yearly, agency, topic, section, type, and subtype.
-        - search_term (str): Option search query term. Defaults to None.
-        - doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
+            facet (str): The facet by which to group the documents. Supported values are daily, weekly, monthly, quarterly, yearly, agency, topic, section, type, and subtype.
+            search_term (str): Option search query term. Defaults to None.
+            doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
         
         Returns:
-        - dict: Returns a dictionary of document counts for the given parameters.
+            dict: Returns a dictionary of document counts for the given parameters.
         """
         if search_term is not None and doc_type is None:
             endpoint = f"documents/facets/{facet}?conditions[term]={search_term}"
             return mr.make_request(self.base_url+endpoint)
         elif doc_type is not None and search_term is None:
             endpoint = f"documents/facets/{facet}?conditions[type][]={doc_type.upper()}"
             return mr.make_request(self.base_url+endpoint)
@@ -96,73 +96,73 @@
             return mr.make_request(self.base_url+endpoint)
             
     def get_document_toc_by_date(self, pub_date):
         """
         Returns the document table of contents based on print edition.
         
         Args:
-        - pub_date (str): The exact publication date (YYYY-MM-DD).
+            pub_date (str): The exact publication date (YYYY-MM-DD).
         
         Returns:
-        - dict: A dictionary containing the document table of contents that matches the given date.
+            dict: A dictionary containing the document table of contents that matches the given date.
         """
         endpoint = f"issues/{pub_date}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_public_inspection_document(self, document_num):
         """
         Returns a single public inspection document matching the given number.
         
         Args:
-        - document_num (str): The number matching the public inspection document.
+            document_num (str): The number matching the public inspection document.
         
         Returns:
-        - dict: A dictionary containing a single public inspection document matching the given number.
+            dict: A dictionary containing a single public inspection document matching the given number.
         """
         endpoint = f"public-inspection-documents/{document_num}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_multiple_public_inspection_documents(self, document_nums):
         """
         Returns the public inspection documents matching the given numbers.
         
         Args:
-        - document_nums (str): The numbers matching the public inspection documents, separated by commas, no spaces.
+            document_nums (str): The numbers matching the public inspection documents, separated by commas, no spaces.
         
         Returns:
-        - dict: A dictionary containing the public inspection documents matching the given numbers.
+            dict: A dictionary containing the public inspection documents matching the given numbers.
         """
         endpoint = f"public-inspection-documents/{document_nums}.json"
         return mr.make_request(self.base_url+endpoint)
         
     def get_current_public_inspection_documents(self):
         """
         Returns all the public inspection documents that are currently on public inspection.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing all the public inspection documents that are currently on public inspection.
+            dict: A dictionary containing all the public inspection documents that are currently on public inspection.
         """
         endpoint = "public-inspection-documents/current.json"
         return mr.make_request(self.base_url+endpoint)
         
     def search_all_public_inspection_documents(self, pub_date, per_page=20, search_term=None, doc_type=None):
         """
         Returns the Federal Register documents published since 1994 matching the given parameters.
         
         Args:
-        - pub_date (str): Public inspection issue date (YYYY-MM-DD).
-        - per_page (int): The number of documents to return at once; default is 20; 1000 maximum.
-        - search_term (str): The term by which to search the documents.
-        - doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
+            pub_date (str): Public inspection issue date (YYYY-MM-DD).
+            per_page (int): The number of documents to return at once; default is 20; 1000 maximum.
+            search_term (str): The term by which to search the documents.
+            doc_type (str): Additional optional search by document type. Supported values are rule (final rule), prorule (proposed rule), notice (notice), and presdocu (presidential document)
         
         Returns:
-        - dict: A dictionary containing the documents published since 1994 matching the given values.
+            dict: A dictionary containing the documents published since 1994 matching the given values.
         """
         if search_term is not None and doc_type is None:
             endpoint = f"public-inspection-documents.json?per_page={per_page}&conditions[available_on]={pub_date}&conditions[term]={search_term}"
             return mr.make_request(self.base_url+endpoint)
         elif doc_type is not None and search_term is None:
             endpoint = f"public-inspection-documents.json?per_page={per_page}&conditions[available_on]={pub_date}&conditions[type][]={doc_type.upper()}"
             return mr.make_request(self.base_url+endpoint)
@@ -175,70 +175,70 @@
             return mr.make_request(self.base_url+endpoint)
             
     def get_agencies_details(self):
         """
         Returns all agency details.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing all agency details.
+            dict: A dictionary containing all agency details.
         """
         endpoint = "agencies"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agency_by_slug(self, slug):
         """
         Returns a particular agency's details.
         
         Args:
-        - slug (str): The Federal Register slug for the agency. See Federal Register API docs for extensive list of possible values.
+            slug (str): The Federal Register slug for the agency. See Federal Register API docs for extensive list of possible values.
         
         Returns:
-        - dict: A dictionary containing a particular agency's details.
+            dict: A dictionary containing a particular agency's details.
         """
         endpoint = f"agencies/{slug}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_image_variants_by_id(self, image_id):
         """
         Returns the available image variants and their metadata for a single image identifier.
         
         Args:
-        - image_id (str): The Federal Register image identifier.
+            image_id (str): The Federal Register image identifier.
         
         Returns:
-        - dict: A dictionary containing the available image variants and their metadata for a single image identifier.
+            dict: A dictionary containing the available image variants and their metadata for a single image identifier.
         """
         endpoint = f"images/{image_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_suggested_searches_by_section(self, section):
         """
         Returns all suggested searches or limit by FederalRegister.gov section.
         
         Args:
-        - section (str): The Federal Register slug for the section. Supported values are business-and-industry, environment, health-and-public-welfare, money, science-and-technology, and world.
+            section (str): The Federal Register slug for the section. Supported values are business-and-industry, environment, health-and-public-welfare, money, science-and-technology, and world.
         
         Returns:
-        - dict: A dictionary containing all the suggested searches or limit by Federal.Register.gov section.
+            dict: A dictionary containing all the suggested searches or limit by Federal.Register.gov section.
         """
         endpoint = f"suggested_searches?conditions[sections]={section}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_suggested_search_by_slug(self, slug):
         """
         Returns a particular suggested search.
         
         Args:
-        - slug (str): The Federal Register slug for the suggested search. See Federal Register API docs for extensive list of possible values.
+            slug (str): The Federal Register slug for the suggested search. See Federal Register API docs for extensive list of possible values.
         
         Returns:
-        - dict: A dictionary containing a particular suggested search.
+            dict: A dictionary containing a particular suggested search.
         """
         endpoint = f"suggested_searches/{slug}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/government/usa_spending.py` & `nokey-0.7.4/nokey/government/usa_spending.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,375 +5,375 @@
 current = dt.datetime.now().year
 
 class USAspending:
     """
     A class for interacting with the USA Spending API.
     
     Attributes:
-    - base_url: The base URL for the API.
-    - about: A short description of the API.
+        base_url: The base URL for the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="usa_spending_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.usaspending.gov/api/v2/"
         self.about = "USAspending is the official open data source of federal spending information, including information about federal awards such as contracts, grants, and loans."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the USAspending API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://api.usaspending.gov/docs/"
         
     def get_agency_overview_info(self, toptier_agency_code, fiscal_year=current):
         """
         Returns agency overview information for USAspending.gov's Agency Details page for agencies that have ever awarded.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing the agency overview information.
+            dict: A dictionary containing the agency overview information.
         """
         endpoint = f"agency/{toptier_agency_code}?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agency_summary_info(self, toptier_agency_code, fiscal_year=current, agency_type="awarding"):
         """
         Returns agency summary information, specifically the number of transactions and award obligations for the sub agency section of USAspending.gov's Agency Details page.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
         
         Returns:
-        - dict: A dictionary containing the agency summary information.
+            dict: A dictionary containing the agency summary information.
         """
         endpoint = f"agency/{toptier_agency_code}/awards?fiscal_year={fiscal_year}&agency_type={agency_type}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_new_awards_count_for_agency(self, toptier_agency_code, fiscal_year=current, agency_type="awarding"):
         """
         Returns a count of New Awards for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
         
         Returns:
-        - dict: A dictionary containing the count.
+            dict: A dictionary containing the count.
         """
         endpoint = f"agency/{toptier_agency_code}/awards/new/count?fiscal_year={fiscal_year}&agency_type={agency_type}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_awards_type_count(self, group="all", fiscal_year=current, order="desc", limit=1, page=1):
         """
         Returns a count of Awards types for agencies in a single fiscal year.
         
         Args:
-        - group (str): Optional parameter. Use cfo to get results where CFO designated agencies are returned. Otherwise the default is all.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): The number of items to return. Default is 1.
-        - page (int): Pagination parameter. Default is 1.
+            group (str): Optional parameter. Use cfo to get results where CFO designated agencies are returned. Otherwise the default is all.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): The number of items to return. Default is 1.
+            page (int): Pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing the count.
+            dict: A dictionary containing the count.
         """
         endpoint = f"agency/awards/count?group={group}&fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_budget_functions_for_agency(self, toptier_agency_code, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Budget Functions and Budget Subfunctions for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Budget Functions and Subfunctions.
+            dict: A dictionary containing a list of Budget Functions and Subfunctions.
         """
         if Filter is not None:
             endpoint = f"agency/{toptier_agency_code}/budget_function?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/{toptier_agency_code}/budget_function?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         
     def get_budget_function_count_for_agency(self, toptier_agency_code, fiscal_year=current):
         """
         Returns the count of Budget Functions for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing the count.
+            dict: A dictionary containing the count.
         """
         endpoint = f"agency/{toptier_agency_code}/budget_function/count?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_budgetary_resources_for_agency(self, toptier_agency_code):
         """
         Returns budgetary resources and obligations for the agency and fiscal year requested.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
         
         Returns:
-        - dict: A dictionary containing a list of budgetary resources and obligations.
+            dict: A dictionary containing a list of budgetary resources and obligations.
         """
         endpoint = f"agency/{toptier_agency_code}/budgetary_resources"
         return mr.make_request(self.base_url+endpoint)
         
     def get_federal_accounts_for_agency(self, toptier_agency_code, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Federal Accounts and Treasury Accounts for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Federal Accounts and Treasury Accounts.
+            dict: A dictionary containing a list of Federal Accounts and Treasury Accounts.
         """
         if Filter is not None:
             endpoint = f"agency/{toptier_agency_code}/federal_account?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/{toptier_agency_code}/federal_account?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
              
     def get_federal_accounts_count_for_agency(self, toptier_agency_code, fiscal_year=current):
         """
         Returns the count of Federal Accounts and Treasury Accounts for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing the count of Federal Accounts and Treasury Accounts.
+            dict: A dictionary containing the count of Federal Accounts and Treasury Accounts.
         """
         endpoint = f"agency/{toptier_agency_code}/federal_account/count?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_object_classes_for_agency(self, toptier_agency_code, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Object Classes for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Objects Classes.
+            dict: A dictionary containing a list of Objects Classes.
         """
         if Filter is not None:
             endpoint = f"agency/{toptier_agency_code}/object_class?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/{toptier_agency_code}/object_class?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
                
     def get_object_classes_count_for_agency(self, toptier_agency_code, fiscal_year=current):
         """
         Returns the count of Object Classes for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing the count of Object Classes.
+            dict: A dictionary containing the count of Object Classes.
         """
         endpoint = f"agency/{toptier_agency_code}/object_class/count?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_obligations_by_award_category_for_agency(self, toptier_agency_code, fiscal_year=current):
         """
         Returns a breakdown of obligations by award category within a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing a breakdown of obligations by award category.
+            dict: A dictionary containing a breakdown of obligations by award category.
         """
         endpoint = f"agency/{toptier_agency_code}/obligations_by_award_category?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_program_activity_for_agency(self, toptier_agency_code, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Program Activity categories for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Program Activity categories.
+            dict: A dictionary containing a list of Program Activity categories.
         """
         if Filter is not None:
             endpoint = f"agency/{toptier_agency_code}/program_activity?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/{toptier_agency_code}/program_activity?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
               
     def get_program_activity_count_for_agency(self, toptier_agency_code, fiscal_year=current):
         """
         Returns the count of Program Activity categories for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing the count of Program Activity categories.
+            dict: A dictionary containing the count of Program Activity categories.
         """
         endpoint = f"agency/{toptier_agency_code}/program_activity/count?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sub_agencies_for_agency(self, toptier_agency_code, fiscal_year=current, agency_type="awarding", order="desc", limit=10, page=1):
         """
         Returns a list of sub-agencies and offices with obligated amounts, transaction counts and new award counts for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of sub-agencies and offices.
+            dict: A dictionary containing a list of sub-agencies and offices.
         """
         endpoint = f"agency/{toptier_agency_code}/sub_agency?fiscal_year={fiscal_year}&agency_type={agency_type}&order={order}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_sub_agency_count_for_agency(self, toptier_agency_code, fiscal_year=current, agency_type="awarding"):
         """
         Returns the number of sub-agencies and offices for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
         
         Returns:
-        - dict: A dictionary containing a number of sub-agencies and offices.
+            dict: A dictionary containing a number of sub-agencies and offices.
         """
         endpoint = f"agency/{toptier_agency_code}/sub_agency/count?fiscal_year={fiscal_year}&agency_type={agency_type}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_federal_accounts_by_bureau_for_agency(self, toptier_agency_code, bureau_slug, fiscal_year=current, agency_type="awarding", order="desc", limit=10, page=1):
         """
         Returns a list of federal_accounts by bureau for the agency in a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - bureau_slug (str): The slug for the bureau.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            bureau_slug (str): The slug for the bureau.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of federal accounts by bureau.
+            dict: A dictionary containing a list of federal accounts by bureau.
         """
         endpoint = f"agency/{toptier_agency_code}/sub_components/{bureau_slug}?fiscal_year={fiscal_year}&agency_type={agency_type}&order={order}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_subcomponents_for_agency(self, toptier_agency_code, fiscal_year=current, agency_type="awarding", order="desc", limit=10, page=1):
         """
         Returns a list of Sub-Components in the Agency's appropriations for a single fiscal year.
         
         Args:
-        - toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            toptier_agency_code (str): A numerical code (in string form, due to the use of leading zeros) identifying the agency.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            agency_type (str): Optional. Determines if the data being returned is derived from the awarding agency or the funding agency. Defaults to awarding, but other option is funding.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Sub-Components.
+            dict: A dictionary containing a list of Sub-Components.
         """
         endpoint = f"agency/{toptier_agency_code}/sub_components?fiscal_year={fiscal_year}&agency_type={agency_type}&order={order}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_object_classes_for_tas(self, tas, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Object Classes for the specified Treasury Account Symbol (tas).
         
         Args:
-        - tas (str): The treasury account symbol (tas) of a treasury account. This endpoint supports TAS codes with 0 or 1 slashes in the code.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            tas (str): The treasury account symbol (tas) of a treasury account. This endpoint supports TAS codes with 0 or 1 slashes in the code.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Object Classes.
+            dict: A dictionary containing a list of Object Classes.
         """
         if Filter is not None:
             endpoint = f"agency/treasury_account/{tas}/object_class?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/treasury_account/{tas}/object_class?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
     
         
     def get_program_activities_for_tas(self, tas, fiscal_year=current, Filter=None, order="desc", limit=10, page=1):
         """
         Returns a list of Program Activities for the specified Treasury Account Symbol (tas).
         
         Args:
-        - tas (str): The treasury account symbol (tas) of a treasury account. This endpoint supports TAS codes with 0 or 1 slashes in the code.
-        - fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
-        - Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
-        - limit (int): Optional parameter to limit number of items. Default is 10.
-        - page (int): Optional pagination parameter. Default is 1.
+            tas (str): The treasury account symbol (tas) of a treasury account. This endpoint supports TAS codes with 0 or 1 slashes in the code.
+            fiscal_year (int): The fiscal year. Optional parameter, defaults to the current year.
+            Filter (str): Optional. This will filter the Budget Function by their name to those matching the text.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order (default).
+            limit (int): Optional parameter to limit number of items. Default is 10.
+            page (int): Optional pagination parameter. Default is 1.
         
         Returns:
-        - dict: A dictionary containing a list of Program Activities.
+            dict: A dictionary containing a list of Program Activities.
         """
         if Filter is not None:
             endpoint = f"agency/treasury_account/{tas}/program_activity?fiscal_year={fiscal_year}&filter={Filter}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
         else:
             endpoint = f"agency/treasury_account/{tas}/program_activity?fiscal_year={fiscal_year}&order={order}&limit={limit}&page={page}"
             return mr.make_request(self.base_url+endpoint)
@@ -381,548 +381,548 @@
        
     ### Autocomplete functions       
     def tas_autocomplete_a(self, Filter, limit=10):
         """
         Returns the list of potential Availability Type Codes narrowed by other components supplied in the Treasury Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Availability Type Codes.
+            dict: A dictionary containing list of potential Availability Type Codes.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/a"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_aid(self, Filter, limit=10):
         """
         Returns the list of potential Agency Identifiers narrowed by other components supplied in the Treasury Account or Federal Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Agency Identifiers.
+            dict: A dictionary containing list of potential Agency Identifiers.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/aid"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_ata(self, Filter, limit=10):
         """
         Returns the list of potential Allocation Transfer Agency Identifiers narrowed by other components supplied in the Treasury Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Transfer Agency Identifiers.
+            dict: A dictionary containing list of potential Transfer Agency Identifiers.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/ata"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_bpoa(self, Filter, limit=10):
         """
         Returns the list of potential Beginning Period of Availabilities narrowed by other components supplied in the Treasury Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Beginning Period of Availabilities.
+            dict: A dictionary containing list of potential Beginning Period of Availabilities.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/bpoa"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_epoa(self, Filter, limit=10):
         """
         Returns the list of potential Ending Period of Availabilities narrowed by other components supplied in the Treasury Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Ending Period of Availabilities.
+            dict: A dictionary containing list of potential Ending Period of Availabilities.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/epoa"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_main(self, Filter, limit=10):
         """
         Returns the list of potential Main Account Codes narrowed by other components supplied in the Treasury Account or Federal Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Main Account Codes.
+            dict: A dictionary containing list of potential Main Account Codes.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/main"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def tas_autocomplete_sub(self, Filter, limit=10):
         """
         Returns the list of potential Sub Account Codes narrowed by other components supplied in the Treasury Account filter.
         
         Args:
-        - Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
-        - limit (int): Optional. Maximum number of results to return. Default is 10.
+            Filter (dict): The component filters to be used in the data. Each component listed may be omitted, null, or a string value. If omitted, no filtering will be performed on that component. If null, the filter will include account numbers missing that component. If a string, the filter will perform an exact match on account numbers where that component matches the string provided. Possible values are ata (optional, string, nullable) Allocation Transfer Agency Identifier (3 characters). TAS only; aid (optional, string, nullable) Agency Identifier (3 characters); bpoa (optional, string, nullable) Beginning Period of Availability (4 characters). TAS only; epoa (optional, string, nullable) Ending Period of Availability (4 characters). TAS only; a (optional, string, nullable) Availability Type Code (1 character). Will either be 'X' or null. TAS only; main (optional, string, nullable) Main Account Code (4 characters); and sub (optional, string, nullable) Sub Account Code (3 characters). TAS only.
+            limit (int): Optional. Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of potential Sub Account Codes.
+            dict: A dictionary containing list of potential Sub Account Codes.
         """
         data = {"filters": Filter, "limit": limit}
         endpoint = "autocomplete/accounts/sub"
         return mr.make_request_with_post_and_data(self.base_url+endpoint, data=data)
         
     def awarding_agency_and_office_autocomplete(self, search_text, limit=None):
         """
         Returns a list of rewarding agencies matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Optional. Maximum number of results to return. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Optional. Maximum number of results to return. Default is None.
         
         Returns:
-        - dict: A dictionary containing list of rewarding agencies.
+            dict: A dictionary containing list of rewarding agencies.
         """
         data = {"search_text": search_text}
         if limit is not None:
             data["limit"] = limit
         endpoint = "autocomplete/awarding_agency_office/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def funding_agency_autocomplete(self, search_text, limit=None):
         """
         Returns a list of funding agencies matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Optional. Maximum number of results to return. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Optional. Maximum number of results to return. Default is None.
         
         Returns:
-        - dict: A dictionary containing list of funding agencies.
+            dict: A dictionary containing list of funding agencies.
         """
         data = {"search_text": search_text}
         if limit is not None:
             data["limit"] = limit
         endpoint = "autocomplete/funding_agency_office/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def cfda_autocomplete(self, search_text, limit=None):
         """
         Returns a list of cfda programs matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Optional. Maximum number of results to return. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Optional. Maximum number of results to return. Default is None.
         
         Returns:
-        - dict: A dictionary containing list of cfda programs.
+            dict: A dictionary containing list of cfda programs.
         """
         data = {"search_text": search_text}
         if limit is not None:
             data["limit"] = limit
         endpoint = "autocomplete/cfda/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def city_autocomplete(self, search_text, limit, country_code, scope, state_code=None):
         """
         Returns a list of city names matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Maximum number of results to return. Required.
-        - country_code (str): Country code part of a filter object. 
-        - scope (str): Scope of the search, part of a filter object. Possible values are primary_place_of_performance and recipient_location.
-        - state_code (str): Optional state code part of a filter object. 
+            search_text (str): Text for search query.
+            limit (int): Maximum number of results to return. Required.
+            country_code (str): Country code part of a filter object. 
+            scope (str): Scope of the search, part of a filter object. Possible values are primary_place_of_performance and recipient_location.
+            state_code (str): Optional state code part of a filter object. 
         
         Returns:
-        - dict: A dictionary containing list of city names.
+            dict: A dictionary containing list of city names.
         """
         if state_code is not None:
             data = {"search_text": search_text, "limit": limit, "filter": {"country_code": country_code, "scope": scope, "state_code": state_code}}
         else:
             data = {"search_text": search_text, "limit": limit, "filter": {"country_code": country_code, "scope": scope}}
         endpoint = "autocomplete/city/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def recipient_autocomplete(self, search_text, limit=10, recipient_levels=None):
         """
         Returns a list of recipients matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Maximum number of results to return. Default is 10, and maximum is 500.
-        - recipient_levels (array): Optional. Array of strings identifying the recipient levels. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Maximum number of results to return. Default is 10, and maximum is 500.
+            recipient_levels (array): Optional. Array of strings identifying the recipient levels. Default is None.
         
         Returns:
-        - dict: A dictionary containing list of recipients.
+            dict: A dictionary containing list of recipients.
         """
         data = {"search_text": search_text, "limit": limit}
         if recipient_levels is not None:
             data["recipient_levels"] = recipient_levels
         endpoint = "autocomplete/recipient/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def glossary_autocomplete(self, search_text, limit=None):
         """
         Returns glossary autocomplete data for submitted text snippet.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Optional. Maximum number of results to return. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Optional. Maximum number of results to return. Default is None.
         
         Returns:
-        - dict: A dictionary containing glossary autocomplete data.
+            dict: A dictionary containing glossary autocomplete data.
         """
         data = {"search_text": search_text}
         if limit is not None:
             data["limit"] = limit
         endpoint = "autocomplete/glossary/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def naics_autocomplete(self, search_text, limit=10):
         """
         Returns a list of naics objects matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Maximum number of results to return. Default is 10.
+            search_text (str): Text for search query.
+            limit (int): Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of naics objects.
+            dict: A dictionary containing list of naics objects.
         """
         data = {"search_text": search_text, "limit": limit}
         endpoint = "autocomplete/naics/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def psc_autocomplete(self, search_text, limit=None):
         """
         Returns a list of product or service (psc) codes matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Optional. Maximum number of results to return. Default is None.
+            search_text (str): Text for search query.
+            limit (int): Optional. Maximum number of results to return. Default is None.
         
         Returns:
-        - dict: A dictionary containing list of product or service (psc) codes.
+            dict: A dictionary containing list of product or service (psc) codes.
         """
         data = {"search_text": search_text}
         if limit is not None:
             data["limit"] = limit
         endpoint = "autocomplete/psc/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def location_autocomplete(self, search_text, limit=10):
         """
         Returns a list of locations matching the specified search text.
         
         Args:
-        - search_text (str): Text for search query.
-        - limit (int): Maximum number of results to return. Default is 10.
+            search_text (str): Text for search query.
+            limit (int): Maximum number of results to return. Default is 10.
         
         Returns:
-        - dict: A dictionary containing list of locations.
+            dict: A dictionary containing list of locations.
         """
         data = {"search_text": search_text, "limit": limit}
         endpoint = "autocomplete/location/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     ### Award-related functions
     def get_recipient_award_spending(self, awarding_agency_id, fiscal_year, limit=10, page=1):
         """
         Returns all award spending by recipient for a given agency id and fiscal year.
         
         Args:
-        - awarding_agency_id (int): Internal award id of the recipient.
-        - fiscal_year (int): The fiscal year for the search.
-        - limit (int): Number of items to return. Defaults to 10.
-        - page (int): Pagination parameter. Defaults to first page.
+            awarding_agency_id (int): Internal award id of the recipient.
+            fiscal_year (int): The fiscal year for the search.
+            limit (int): Number of items to return. Defaults to 10.
+            page (int): Pagination parameter. Defaults to first page.
         
         Returns:
-        - dict: Dictionary containing all award spending by recipient.
+            dict: Dictionary containing all award spending by recipient.
         """
         enpoint = f"award_spending/recipient/?fiscal_year={fiscal_year}&awarding_agency_id={awarding_agency_id}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+enpoint)
         
     def get_award_data(self, award_id):
         """
         Returns a list of data that is associated with the award profile page.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
+            award_id (str): Unique identifier matching the award.
         
         Returns:
-        - dict: Dictionary containing a list of data associated with an award.
+            dict: Dictionary containing a list of data associated with an award.
         """
         enpoint = f"awards/{award_id}"
         return mr.make_request(self.base_url+enpoint)
         
     def get_award_accounts(self, award_id, page=1, limit=None, order="desc", sort="federal_account"):
         """
         Returns a list of federal accounts under a given award.
         
         Args:
-        - award_id (str): Unique matching the award.
-        - page (int): Optional pagination parameter. Defaults to first page.
-        - limit (int): Number of items to return. Defaults to None.
-        - order (str): Ordering of the data. Defaults to desc (descending), and other option is asc (ascending).
-        - sort (str): The field to sort on. Default is federal_account, but other options are account_title, agency, and total_transaction_obligated_amount.
+            award_id (str): Unique matching the award.
+            page (int): Optional pagination parameter. Defaults to first page.
+            limit (int): Number of items to return. Defaults to None.
+            order (str): Ordering of the data. Defaults to desc (descending), and other option is asc (ascending).
+            sort (str): The field to sort on. Default is federal_account, but other options are account_title, agency, and total_transaction_obligated_amount.
         
         Returns:
-        - dict: Dictionary containing a list of federal accounts under a given award.
+            dict: Dictionary containing a list of federal accounts under a given award.
         """
         data = {"sort": sort, "order": order, "award_id": award_id, "page": page}
         if limit is not None:
             data["limit"] = limit
         enpoint = "awards/accounts/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def get_federal_accounts_count_by_award(self, award_id):
         """
         Returns the number of federal accounts associated with the given award.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
+            award_id (str): Unique identifier matching the award.
         
         Returns:
-        - dict: Dictionary containing the number of federal accounts associated with the given award.
+            dict: Dictionary containing the number of federal accounts associated with the given award.
         """
         enpoint = f"awards/count/federal_account/{award_id}"
         return mr.make_request(self.base_url+enpoint)
         
     def get_subawards_for_award(self, award_id):
         """
         Returns the number of subawards associated with the given award.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
+            award_id (str): Unique identifier matching the award.
         
         Returns:
-        - dict: Dictionary containing the number of subawards associated with the given award.
+            dict: Dictionary containing the number of subawards associated with the given award.
         """
         enpoint = f"awards/count/subaward/{award_id}"
         return mr.make_request(self.base_url+enpoint)
         
     def get_award_transactions_count(self, award_id):
         """
         Returns the number of transactions associated with the given award.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
+            award_id (str): Unique identifier matching the award.
         
         Returns:
-        - dict: Dictionary containing the number of transactions associated with the given award.
+            dict: Dictionary containing the number of transactions associated with the given award.
         """
         enpoint = f"awards/count/transaction/{award_id}"
         return mr.make_request(self.base_url+enpoint)
         
     def get_award_funding_data(self, award_id, page=1, limit=10, order="desc", sort="reporting_fiscal_date"):
         """
         Returns federal account, awarding agencies, funding agencies, and transaction obligated amount information for a requested award.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
-        - page (int): Optional pagination parameter. Defaults to first page.
-        - limit (int): Number of items to return. Defaults to 10.
-        - order (str): Ordering of the data. Defaults to desc (descending), and other option is asc (ascending).
-        - sort (str): The field to sort on. Default is reporting_fiscal_date, but other options are account_title, awarding_agency_name, disaster_emergency_fund_code, federal_account, funding_agency_name, gross_outlay_amount, object_class, program_activity, and transaction_obligated_amount.
+            award_id (str): Unique identifier matching the award.
+            page (int): Optional pagination parameter. Defaults to first page.
+            limit (int): Number of items to return. Defaults to 10.
+            order (str): Ordering of the data. Defaults to desc (descending), and other option is asc (ascending).
+            sort (str): The field to sort on. Default is reporting_fiscal_date, but other options are account_title, awarding_agency_name, disaster_emergency_fund_code, federal_account, funding_agency_name, gross_outlay_amount, object_class, program_activity, and transaction_obligated_amount.
         
         Returns:
-        - dict: Dictionary containing a list of data for a given award.
+            dict: Dictionary containing a list of data for a given award.
         """
         data = {"sort": sort, "order": order, "award_id": award_id, "page": page, "limit": limit}
         enpoint = "awards/funding/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def get_award_funding_obligations_and_count(self, award_id):
         """
         Returns the total transaction obligations and count of awarding agencies, funding agencies, and federal accounts for an award.
         
         Args:
-        - award_id (str): Unique identifier matching the award.
+            award_id (str): Unique identifier matching the award.
        
         Returns:
-        - dict: Dictionary containing a list of total transaction obligations and count of awarding agencies, funding agencies, and federal accounts for an award.
+            dict: Dictionary containing a list of total transaction obligations and count of awarding agencies, funding agencies, and federal accounts for an award.
         """
         data = {"award_id": award_id}
         enpoint = "awards/funding_rollup/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def get_award_last_updated(self):
         """
         Returns the last updated date for the award data.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: Dictionary containing the last updated date for the award data.
+            dict: Dictionary containing the last updated date for the award data.
         """
         enpoint = "awards/last_updated"
         return mr.make_request(self.base_url+enpoint)
     
     ### Budget functions    
     def get_budget_functions(self):
         """
         Returns a list of all Budget Functions ordered by their title.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: Dictionary containing a list of all Budget Functions ordered by their title.
+            dict: Dictionary containing a list of all Budget Functions ordered by their title.
         """
         enpoint = "budget_functions/list_budget_functions"
         return mr.make_request(self.base_url+enpoint)
         
     def get_budget_subfunctions(self, budget_function=None):
         """
         Returns a list of all Budget Subfunctions that can be filtered by Budget Function, ordered by their title.
         
         Args:
-        - budget_function (int): Number matching the budget function.
+            budget_function (int): Number matching the budget function.
        
         Returns:
-        - dict: Dictionary containing a list of Budget Subfunctions.
+            dict: Dictionary containing a list of Budget Subfunctions.
         """
         if budget_function is not None:
             data = {"budget_function": budget_function}
         else:
             data = {}
         enpoint = "budget_functions/list_budget_subfunctions/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     ### Download functions
     def bulk_award_download(self, filters, file_format="csv"):
         """
         Returns a ZIP file of award data for download.
         
         Args:
-        - filters (dict): A dictionary of filter options for the downloaded data. See the endpoint docs for the format of this filter object.
-        - file_format (str): Format of the file to be downloaded. Default is csv, but other options are tsv and pstxt.
+            filters (dict): A dictionary of filter options for the downloaded data. See the endpoint docs for the format of this filter object.
+            file_format (str): Format of the file to be downloaded. Default is csv, but other options are tsv and pstxt.
        
         Returns:
-        - dict: Dictionary containing the data regarding ZIP file for download.
+            dict: Dictionary containing the data regarding ZIP file for download.
         """
         data = {"filters": filters, "file_format": file_format}
         enpoint = "bulk_download/awards/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def list_agencies(self, agencies_type, agency=None):
         """
         Returns one of three result set flavors. For "account_agencies" requests it returns a list of all toptier agencies with at least one DABS submission. For "award_agencies" requests it returns a list of all user selectable flagged toptier agencies with at least one subtier agency. For specific agency requests it returns a list of all user selectable flagged subtier agencies.
         
         Args:
-        - agencies_type (str): Type of agency desired. Possible options are account_agencies and award_agencies.
-        - agency (int): Agency identifier number.
+            agencies_type (str): Type of agency desired. Possible options are account_agencies and award_agencies.
+            agency (int): Agency identifier number.
        
         Returns:
-        - dict: Dictionary containing a list of selected agency information.
+            dict: Dictionary containing a list of selected agency information.
         """
         data = {"type": agencies_type}
         if agency is not None:
             data["agency"] = agency
         enpoint = "bulk_download/list_agencies/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def list_monthly_files(self, agency, fiscal_year, file_type):
         """
         Returns a list of the current versions of generated archive files for a given fiscal year and agency.
         
         Args:
-        - agency (str or int): Agency database ID or all.
-        - fiscal_year (int): Fiscal year.
-        - file_type (str): Optional parameter for archive file type. Possible values are assistance and contracts. Defaults to None.
+            agency (str or int): Agency database ID or all.
+            fiscal_year (int): Fiscal year.
+            file_type (str): Optional parameter for archive file type. Possible values are assistance and contracts. Defaults to None.
        
         Returns:
-        - dict: Dictionary containing a list of current versions of generated archive files.
+            dict: Dictionary containing a list of current versions of generated archive files.
         """
         data = {"agency": agency, "fiscal_year": fiscal_year, "type": file_type}
         enpoint = "bulk_download/list_monthly_files/"
         return mr.make_request_with_post_and_json(self.base_url+enpoint, json=data)
         
     def get_download_status(self, file_name):
         """
         Returns the current status of a download job.
         
         Args:
-        - file_name (str): The full name of the file downloaded. Taken from the file_name field of a download endpoint response.
+            file_name (str): The full name of the file downloaded. Taken from the file_name field of a download endpoint response.
         
         Returns:
-        - dict: Dictionary containing the current status of a download job.
+            dict: Dictionary containing the current status of a download job.
         """
         enpoint = f"bulk_download/status?file_name={file_name}"
         return mr.make_request(self.base_url+enpoint)
         
     ### Emergency and disaster related functions
     def get_count_agencies_receiving_def(self, def_codes):
         """
         Returns a count for agencies which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
         
         Returns:
-        - dict: A dictionary containing a count of agencies which received disaster/emergency funding.
+            dict: A dictionary containing a count of agencies which received disaster/emergency funding.
         """
         data = {"filter": {"def_codes": def_codes}}
         endpoint = "disaster/agency/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_agencies_awarding_def_loans(self, def_codes, award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Agencies awarding loans from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Agencies awarding loans from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Agencies awarding loans from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order}
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/agency/loans/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_agencies_receiving_def_funding(self, def_codes, spending_type="total", award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Agencies receiving funding from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Agencies receiving funding from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Agencies receiving funding from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -930,25 +930,25 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_aggregated_def_spending(self, def_codes, spending_type="total", award_type_codes=None, award_type=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - award_type (str): When provided, it will return results limiting to the award type (Assistance or Procurment) based on Financial Account data. This is mutually exclusive from award_type_codes. Possible values are procurement and assistance.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            award_type (str): When provided, it will return results limiting to the award type (Assistance or Procurment) based on Financial Account data. This is mutually exclusive from award_type_codes. Possible values are procurement and assistance.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -958,25 +958,25 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_aggregated_def_spending_count(self, def_codes, spending_type="total", award_type_codes=None, award_type=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns the count of account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - award_type (str): When provided, it will return results limiting to the award type (Assistance or Procurment) based on Financial Account data. This is mutually exclusive from award_type_codes. Possible values are procurement and assistance.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            award_type (str): When provided, it will return results limiting to the award type (Assistance or Procurment) based on Financial Account data. This is mutually exclusive from award_type_codes. Possible values are procurement and assistance.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing the count of account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of account data obligation and outlay spending aggregations of all (File D) Awards which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -986,64 +986,64 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_cfda_receiving_def_count(self, def_codes, award_type_codes=None):
         """
         Returns the count of CFDA programs which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11. Defaults to None here, but in the API it defaults to all the codes.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11. Defaults to None here, but in the API it defaults to all the codes.
         
         Returns:
-        - dict: A dictionary containing the count of CFDA programs which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of CFDA programs which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes}}
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/cfda/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_def_loans_for_cfda(self, def_codes, award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the CFDA Programs' loans from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the CFDA Programs' loans from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the CFDA Programs' loans from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order}
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/cfda/loans/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_cfda_programs_receiving_def_funding(self, def_codes, spending_type="total", award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the cfda programs receiving funding from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the cfda programs receiving funding from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the cfda programs receiving funding from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -1051,75 +1051,75 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_defc_receiving_def_count(self, def_codes):
         """
         Returns the count of DEFC which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
          
         Returns:
-        - dict: A dictionary containing the count of DEFC which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of DEFC which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes}}
         endpoint = "disaster/def_code/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_federal_accounts_receiving_def_count(self, def_codes):
         """
         Returns the count of Federal Accounts and TAS which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
          
         Returns:
-        - dict: A dictionary containing the count of Federal Accounts and TAS which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of Federal Accounts and TAS which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes}}
         endpoint = "disaster/federal_account/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_def_loans_for_federal_accounts(self, def_codes, award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Federal Accounts awarding loans from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Federal Accounts awarding loans from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Federal Accounts awarding loans from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order}
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/federal_account/loans/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_federal_accounts_receiving_def_funding(self, def_codes, spending_type="total", award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Federal Accounts and TAS receiving funding from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Federal Accounts and TAS receiving funding from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Federal Accounts and TAS receiving funding from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -1127,61 +1127,61 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_object_classes_receiving_def_count(self, def_codes):
         """
         Returns the count of Object Classes which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
          
         Returns:
-        - dict: A dictionary containing the count of Object Classes which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of Object Classes which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes}}
         endpoint = "disaster/object_class/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_def_loans_for_object_classes(self, def_codes, award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Object Classes' loans from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Object Classes' loans from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Object Classes' loans from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order}
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/object_class/loans/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_object_classes_receiving_def_funding(self, def_codes, spending_type="total", award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the Object Classes receiving funding from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the Object Classes receiving funding from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the Object Classes receiving funding from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -1189,64 +1189,64 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_recipients_receiving_def_count(self, def_codes, award_type_codes=None):
         """
         Returns the count of Recipients which received disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
         
         Returns:
-        - dict: A dictionary containing the count of Recipients which received disaster/emergency funding per the requested filters.
+            dict: A dictionary containing the count of Recipients which received disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes}}
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/recipient/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_def_loans_for_recipients(self, def_codes, award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the recipient loans from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            award_type_codes (list): Optional. Only accepts loan award type 07 or 08 in the array, since this endpoint is specific to loans. Defaults to None.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the recipient loans from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the recipient loans from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order}
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
         endpoint = "disaster/recipient/loans/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_recipients_receiving_def_funding(self, def_codes, spending_type="total", award_type_codes=None, limit=10, page=1, sort="id", order="desc"):
         """
         Returns insights on the recipients receiving funding from disaster/emergency funding per the requested filters.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - spending_type (str): Spending type. Defaults to total, but other option is award.
-        - award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - limit (int): Page size of results. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
-        - sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            spending_type (str): Spending type. Defaults to total, but other option is award.
+            award_type_codes (list): Optional. Only to be used if spending type is award. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            limit (int): Page size of results. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            order (str): Order of returned data. Defaults to desc (descending), with asc (ascending) as other option.
+            sort (str): Optional parameter indicating what returns values should be sorted by. Default is id, but other options are code, description, award_count, face_value_of_loan, obligation, and outlay.
         
         Returns:
-        - dict: A dictionary containing insights on the recipients receiving funding from disaster/emergency funding per the requested filters.
+            dict: A dictionary containing insights on the recipients receiving funding from disaster/emergency funding per the requested filters.
         """
         data = {"filter": {"def_codes": def_codes},
                 "pagination": {"limit": limit, "page": page, "sort": sort, "order": order},
                 "spending_type": spending_type
                 }
         if award_type_codes is not None:
             data["filter"]["award_type_codes"] = award_type_codes
@@ -1254,22 +1254,22 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_def_spending_by_geography(self, def_codes, geo_layer, spendng_type, geo_layer_filters=None, scope="recipient_location"):
         """
         Returns geographical spending information from emergency/disaster funding based on recipient location.
         
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
-        - geo_layer (str): Sets the type of shape codes in the response. Possible values are state, county, and district.
-        - spending_type (str): Possible values are obligation, outlay, and face_value_of_loan.
-        - geo_layer_filters (list): Optional. Allows the API to only request data for what is currently in view in the map.. Defaults to None.
-        - scope (str): Optional. When fetching awards, use the primary place of performance or recipient location. Defaults to recipient_location, but other values is place_of_performance.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V.
+            geo_layer (str): Sets the type of shape codes in the response. Possible values are state, county, and district.
+            spending_type (str): Possible values are obligation, outlay, and face_value_of_loan.
+            geo_layer_filters (list): Optional. Allows the API to only request data for what is currently in view in the map.. Defaults to None.
+            scope (str): Optional. When fetching awards, use the primary place of performance or recipient location. Defaults to recipient_location, but other values is place_of_performance.
         
         Returns:
-        - dict: A dictionary containing geographical spending information from emergency/disaster funding based on recipient location.
+            dict: A dictionary containing geographical spending information from emergency/disaster funding based on recipient location.
         """
         data = {"filter": {"def_codes": def_codes},
                 "geo_layer": geo_layer,
                 "scope": scope,
                 "spending_type": spendng_type
         }
         if geo_layer_filters is not None:
@@ -1279,26 +1279,26 @@
         
     ### More download functions
     def download_account(self, account_level, submission_types, fiscal_year, agency=None, federal_account=None, quarter=None, period=None, def_codes=None, file_format="csv"):
         """
         Generate files and return metadata using filters on custom account.
             
         Args:
-        - account_level (str): Used to filter for a specific type of file. Specific values are treasury_account and federal_account.
-        - submission_types (list): Possible values are account_balances, object_class_program_activity, and award_financial.
-        - fiscal_year (int): Fiscal year.
-        - agency (str): Optional. The agency on which to filter. This field expects an internal toptier agency identifier also known as the toptier_agency_id. Defaults to None.
-        - federal_account (str): Optional. An internal id. Defaults to None.
-        - quarter (int): Either quarter or period is required. Do not supply both. Note that both monthly and quarterly submissions will be included in the resulting download file even if only quarter is provided. Possible values are 1, 2, 3, and 4.
-        - period (int): Either quarter or period is required. Do not supply both. Agencies cannot submit data for period 1 so it is disallowed as a query filter. Note that both monthly and quarterly submissions will be included in the resulting download file even if only period is provided. Possible values are 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, and 12.
-        - def_codes (list): Option search parameter by def codes.
-        - file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
+            account_level (str): Used to filter for a specific type of file. Specific values are treasury_account and federal_account.
+            submission_types (list): Possible values are account_balances, object_class_program_activity, and award_financial.
+            fiscal_year (int): Fiscal year.
+            agency (str): Optional. The agency on which to filter. This field expects an internal toptier agency identifier also known as the toptier_agency_id. Defaults to None.
+            federal_account (str): Optional. An internal id. Defaults to None.
+            quarter (int): Either quarter or period is required. Do not supply both. Note that both monthly and quarterly submissions will be included in the resulting download file even if only quarter is provided. Possible values are 1, 2, 3, and 4.
+            period (int): Either quarter or period is required. Do not supply both. Agencies cannot submit data for period 1 so it is disallowed as a query filter. Note that both monthly and quarterly submissions will be included in the resulting download file even if only period is provided. Possible values are 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, and 12.
+            def_codes (list): Option search parameter by def codes.
+            file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
             
         Returns:
-        - dict: A dictionary containing information on the download job.
+            dict: A dictionary containing information on the download job.
         """
         data = {"account_level": account_level,
                 "file_format": file_format,
                 "filters": {
                     "fy": fiscal_year,
                     "submission_types": submission_types
                     }
@@ -1323,36 +1323,36 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
             
     def download_assistance_data(self, award_id, file_format="csv"):
         """
         Creates a new download job for the requested award and returns a link to a zipped file containing contract award data.
             
         Args:
-        - award_id (str): Unique identifier for the award.
-        - file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
+            award_id (str): Unique identifier for the award.
+            file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
             
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"award_id": award_id, "file_format": file_format}
         endpoint = "download/assistance/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
             
     def download_award_data_advanced(self, filters, columns=None, file_format="csv", limit=None):
         """
         Creates a download job for the award data matching the search filters.
         
         Args:
-        - filters (dict): An advanced json object for filtering results. Must contain ar least one filter entry. See this endpoint's docs for information on format of this filtering object.
-        - columns (list): A list of the column names desired. Default is None.
-        - file_format (str): Default is csv, but other options are tsv and pstxt.
-        - limit (int): Optional. Number of items in file. Default is None.
+            filters (dict): An advanced json object for filtering results. Must contain ar least one filter entry. See this endpoint's docs for information on format of this filtering object.
+            columns (list): A list of the column names desired. Default is None.
+            file_format (str): Default is csv, but other options are tsv and pstxt.
+            limit (int): Optional. Number of items in file. Default is None.
         
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"filters": filters,
                 "file_format": file_format
         }
         if columns is not None:
             data["columns"] = columns
         if limit is not None:
@@ -1361,100 +1361,100 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def download_contract_data(self, award_id, file_format="csv"):
         """
         Creates a new download job for the requested award and returns a link to a zipped file containing award contract data.
             
         Args:
-        - award_id (str): Unique identifier for the award.
-        - file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
+            award_id (str): Unique identifier for the award.
+            file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
             
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"award_id": award_id, "file_format": file_format}
         endpoint = "download/contract/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def download_transaction_count(self, filters):
         """
         Returns the number of transactions that would be included in a download request for the given filter set.
             
         Args:
-        - filters (dict): Advanced json filter object. See this endpoint's docs for information on the format of this json object.
+            filters (dict): Advanced json filter object. See this endpoint's docs for information on the format of this json object.
             
         Returns:
-        - dict: A dictionary containing a number of transactions.
+            dict: A dictionary containing a number of transactions.
         """
         data = filters
         endpoint = "download/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
        
     def download_def_data(self, def_codes, file_format="csv"):
         """
         Creates a new download job for the requested COVID-19 related account and award. Returns a link to a zipped file containing the generated data files.
             
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V, but it must be either one of these or all of them.
-        - file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V, but it must be either one of these or all of them.
+            file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
             
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"filters": {"def_codes": def_codes}, "file_format": file_format}
         endpoint = "download/disaster/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def download_def_recipient_data(self, def_codes, award_type_codes=None, query=None):
         """
         Returns information to download a zip file of recipient disaster data. Specifically, only COVID-19 at the moment
             
         Args:
-        - def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V, but it must be either one of these or all of them.
-        - award_type_codes (list): Optional. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
-        - query (str): Search query term.
+            def_codes (list): A list of Disaster Emergency Fund (def) codes (strings). Possible values are L, M, N, O, P, U, and V, but it must be either one of these or all of them.
+            award_type_codes (list): Optional. Possible values are 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, A, B, C, D, IDV_A, IDV_B_A, IDV_B_B, IDV_B_C, IDV_B, IDV_C, IDV_D, IDV_E, and -1.
+            query (str): Search query term.
             
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"filters": {"def_codes": def_codes}}
         if award_type_codes is not None:
             data["filters"]["award_type_codes"] = award_type_codes
         if query is not None:
             data["filters"]["query"] = query
         endpoint = "download/disaster/recipients/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def download_idv_data(self, award_id, file_format="csv"):
         """
         Creates a new download job for the requested award and returns a link to a zipped file containing IDV data.
             
         Args:
-        - award_id (str): Unique identifier for the award.
-        - file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
+            award_id (str): Unique identifier for the award.
+            file_format (str): Optional. Defaults to csv, but other values are tsv and pstxt.
             
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"award_id": award_id, "file_format": file_format}
         endpoint = "download/idv/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def download_transactions_data_advanced(self, filters, columns=None, file_format="csv", limit=None):
         """
         Creates a download job for the transaction data matching the search filters.
         
         Args:
-        - filters (dict): An advanced json object for filtering results. Must contain ar least one filter entry. See this endpoint's docs for information on format of this filtering object.
-        - columns (list): A list of the column names desired. Default is None.
-        - file_format (str): Default is csv, but other options are tsv and pstxt.
-        - limit (int): Optional. Number of items in file. Default is None.
+            filters (dict): An advanced json object for filtering results. Must contain ar least one filter entry. See this endpoint's docs for information on format of this filtering object.
+            columns (list): A list of the column names desired. Default is None.
+            file_format (str): Default is csv, but other options are tsv and pstxt.
+            limit (int): Optional. Number of items in file. Default is None.
         
         Returns:
-        - dict: A dictionary containing information about the download job.
+            dict: A dictionary containing information about the download job.
         """
         data = {"filters": filters,
                 "file_format": file_format
         }
         if columns is not None:
             data["columns"] = columns
         if limit is not None:
@@ -1464,65 +1464,65 @@
         
     ### Other functions 
     def get_federal_account(self, account_number, fiscal_year=current):
         """
         Returns the agency identifier, account code, title, and database id for the given federal account.
         
         Args:
-        - account_number (str): The Federal Account symbol comprised of Agency Code and Main Account Code. A unique identifier for federal accounts.
-        - fiscal_year (str): Desired fiscal year. Defaults to current year.
+            account_number (str): The Federal Account symbol comprised of Agency Code and Main Account Code. A unique identifier for federal accounts.
+            fiscal_year (str): Desired fiscal year. Defaults to current year.
         
         Returns:
-        - dict: A dictionary containing the agency identifier, account code, title, and database id for the given federal account.
+            dict: A dictionary containing the agency identifier, account code, title, and database id for the given federal account.
         """
         endpoint = f"federal_accounts/{account_number}/?fiscal_year={fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_spending_data_by_object_class(self, federal_account_id):
         """
         Returns object classes that the specified federal account has allotted money toward.
         
         Args:
-        - federal_account_id (int): Database id for a federal account.
+            federal_account_id (int): Database id for a federal account.
         
         Returns:
-        - dict: A dictionary containing the data matching the parameter.
+            dict: A dictionary containing the data matching the parameter.
         """
         endpoint = f"federal_accounts/{federal_account_id}/available_object_classes"
         return mr.make_request(self.base_url+endpoint)
         
     def get_fiscal_year_snapshot_for_federal_account(self, federal_account_id, fiscal_year=current):
         """
         Returns budget information for a federal account for the year provided based on account's internal ID.
         
         Args:
-        - federal_account_id (int): Database id for a federal account.
-        - fiscal_year (int): The fiscal year. Defaults to the current year.
+            federal_account_id (int): Database id for a federal account.
+            fiscal_year (int): The fiscal year. Defaults to the current year.
         
         Returns:
-        - dict: A dictionary containing budget information for a federal account for the year provided based on account's internal ID
+            dict: A dictionary containing budget information for a federal account for the year provided based on account's internal ID
         """
         endpoint = f"federal_accounts/{federal_account_id}/fiscal_year_snapshot/{fiscal_year}"
         return mr.make_request(self.base_url+endpoint)
         
     def search_federal_accounts(self, fiscal_year=str(current), agency_identifier=None, sort_direction="desc", sort_field="budgetary_resources", limit=50, page=1, keyword=None):
         """
         Returns a list of federal accounts, their number, name, managing agency, and budgetary resources matching the search parameters.
         
         Args:
-        - fiscal_year (str): The desired fiscal year, entered as a string. If none is given, default is previous year.
-        - agency_identifier (str): Agency id. Optional. Defaults to None.
-        - sort_direction (str): The direction in which to sort. Defaults to desc, but other option is asc.
-        - sort_field (str): The field on which to sort. Default is budgetary_resources, but other options are account_number, account_name, and managing_agency.
-        - limit (int): Number of results to include per page. Defaults to 50.
-        - page (int): The page to return. Defaults to first page.
-        - keyword (str): Optional search term. Default is None.
+            fiscal_year (str): The desired fiscal year, entered as a string. If none is given, default is previous year.
+            agency_identifier (str): Agency id. Optional. Defaults to None.
+            sort_direction (str): The direction in which to sort. Defaults to desc, but other option is asc.
+            sort_field (str): The field on which to sort. Default is budgetary_resources, but other options are account_number, account_name, and managing_agency.
+            limit (int): Number of results to include per page. Defaults to 50.
+            page (int): The page to return. Defaults to first page.
+            keyword (str): Optional search term. Default is None.
         
         Returns:
-        - dict: A dictionary containing a list of federal accounts, their number, name, managing agency, and budgetary resources matching the search parameters.
+            dict: A dictionary containing a list of federal accounts, their number, name, managing agency, and budgetary resources matching the search parameters.
         """
         data = {"filters": {"fy": fiscal_year},
                 "sort": {
                     "direction": sort_direction,
                     "field": sort_field
                     },
                 "limit": limit,
@@ -1536,82 +1536,82 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_federal_account_by_obligation(self, fiscal_year, funding_agency_id, limit=10, page=1):
         """
         Returns the amount that the specific agency has obligated to various federal accounts in a given fiscal year.
         
         Args:
-        - fiscal_year (int): The desired fiscal year.
-        - funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
-        - limit (int): Maximum number of results to return.
-        - page (int): Optional pagination parameter. Defaults to first page.
+            fiscal_year (int): The desired fiscal year.
+            funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
+            limit (int): Maximum number of results to return.
+            page (int): Optional pagination parameter. Defaults to first page.
         
         Returns:
-        - dict: A dictionary containing the amount that the specific agency has obligated to various federal accounts in a given fiscal year.
+            dict: A dictionary containing the amount that the specific agency has obligated to various federal accounts in a given fiscal year.
         """
         endpoint = f"federal_obligations/?fiscal_year={fiscal_year}&funding_agency_id={funding_agency_id}&limit={limit}&page={page}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_financial_balances(self, fiscal_year, funding_agency_id):
         """
         Returns aggregated balances for a specific government agency in a given fiscal year.
         
         Args:
-        - fiscal_year (int): The desired fiscal year.
-        - funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
+            fiscal_year (int): The desired fiscal year.
+            funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
           
         Returns:
-        - dict: A dictionary containing financial balance data.
+            dict: A dictionary containing financial balance data.
         """
         endpoint = f"financial_balances/agencies/?fiscal_year={fiscal_year}&funding_agency_id={funding_agency_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_financial_spending_by_object_class(self, fiscal_year, funding_agency_id):
         """
         Returns the total amount that a specific agency has obligated to major object classes in a given fiscal year.
         
         Args:
-        - fiscal_year (int): The desired fiscal year.
-        - funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
+            fiscal_year (int): The desired fiscal year.
+            funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
           
         Returns:
-        - dict: A dictionary containing financial spending data.
+            dict: A dictionary containing financial spending data.
         """
         endpoint = f"financial_spending/major_object_class/?fiscal_year={fiscal_year}&funding_agency_id={funding_agency_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_financial_spending_for_minor_object_class(self, fiscal_year, funding_agency_id, major_object_class_code):
         """
         Returns the total amount that a specific agency has obligated to minor object classes within a specific major object class in a given fiscal year.
         
         Args:
-        - fiscal_year (int): The desired fiscal year.
-        - funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
-        - major_object_class_code (int): The major object class code returned in /api/v2/financial_spending/major_object_class/.
+            fiscal_year (int): The desired fiscal year.
+            funding_agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
+            major_object_class_code (int): The major object class code returned in /api/v2/financial_spending/major_object_class/.
           
         Returns:
-        - dict: A dictionary containing financial spending data.
+            dict: A dictionary containing financial spending data.
         """
         endpoint = f"financial_spending/major_object_class/?fiscal_year={fiscal_year}&funding_agency_id={funding_agency_id}&major_object_class_code={major_object_class_code}"
         return mr.make_request(self.base_url+endpoint)
         
     ### IDV functions  
     def get_federal_accounts_under_idv(self, award_id, page=1, limit=10, order="desc", sort="total_transaction_obligated_amount"):
         """
         Returns a list of federal accounts under a given IDV.
         
         Args:
-        - award_id (str): IDV (Indefinite Delivery Vehicle) to return accounts for.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Optional. Number of items to return. Default is 10.
-        - order (str): Order in which to return data. Default is desc, and other option is asc.
-        - sort (str): Sorting parameter. Default is total_transaction_obligated_amount, but other options are federal_account, agency, and account_title.
+            award_id (str): IDV (Indefinite Delivery Vehicle) to return accounts for.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Optional. Number of items to return. Default is 10.
+            order (str): Order in which to return data. Default is desc, and other option is asc.
+            sort (str): Sorting parameter. Default is total_transaction_obligated_amount, but other options are federal_account, agency, and account_title.
         
         Returns:
-        - dict: A dictionary containing a list of federal accounts.
+            dict: A dictionary containing a list of federal accounts.
         """
         data = {"limit": limit,
                 "sort": sort,
                 "order": order,
                 "award_id": award_id,
                 "page": page
         }
@@ -1619,57 +1619,57 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_idv_activity(self, award_id, page=1, limit=10, hide_edge_cases="false"):
         """
         Returns a list of child and grandchild awards for a given IDV.
         
         Args:
-        - award_id (str): IDV (Indefinite Delivery Vehicle) to return accounts for.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Optional. Number of items to return. Default is 10.
-        - hide_edge_cases (str): Choose whether or not to hide awards that have no/negative obligated amounts and/or no/negative awarded amounts and/or no end date. Default is false and true is other option.
+            award_id (str): IDV (Indefinite Delivery Vehicle) to return accounts for.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Optional. Number of items to return. Default is 10.
+            hide_edge_cases (str): Choose whether or not to hide awards that have no/negative obligated amounts and/or no/negative awarded amounts and/or no end date. Default is false and true is other option.
         
         Returns:
-        - dict: A dictionary containing a list of awards.
+            dict: A dictionary containing a list of awards.
         """
         data = {"award_id": award_id,
                 "page": page,
                 "hide_edge_cases": hide_edge_cases,
                 "limit": limit
         }
         endpoint = "idvs/activity/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_idv_amounts(self, award_id):
         """
         Returns aggregated award counts and funding amounts for IDV contracts.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
            
         Returns:
-        - dict: A dictionary containing a list of award coints and funding amounts.
+            dict: A dictionary containing a list of award coints and funding amounts.
         """
         endpoint = f"idvs/amounts/{award_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_idv_awards(self, award_id, Type="child_idvs", page=1, limit=10, order="desc", sort="period_of_performance_start_date"):
         """
         Returns a list of child IDVs, child awards, or grandchild awards for IDV.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
-        - type (str): The type of related awards to return. Default is child_idvs, but other options are child_awards and grandchild_awards.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Optional. Number of items to return. Default is 10.
-        - order (str): Order in which to return data. Default is desc, and other option is asc.
-        - sort (str): Sorting parameter. Default is period_of_performance_start_date, but other options are piid, description, period_of_performance_current_end_date, last_date_to_order, funding_agency, awarding_agency, award_type, and obligated_amount.
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            type (str): The type of related awards to return. Default is child_idvs, but other options are child_awards and grandchild_awards.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Optional. Number of items to return. Default is 10.
+            order (str): Order in which to return data. Default is desc, and other option is asc.
+            sort (str): Sorting parameter. Default is period_of_performance_start_date, but other options are piid, description, period_of_performance_current_end_date, last_date_to_order, funding_agency, awarding_agency, award_type, and obligated_amount.
         
         Returns:
-        - dict: A dictionary containing a list of idv award data.
+            dict: A dictionary containing a list of idv award data.
         """
         data = {"award_id": award_id,
                 "type": Type,
                 "limit": limit,
                 "page": page,
                 "sort": sort,
                 "order": order,        
@@ -1678,40 +1678,40 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_idv_federal_account_count(self, award_id, piid=None):
         """
         Returns the number of federal accounts associated with the given IDV and it's children and grandchildren.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
-        - piid (str): Optional. Award ID to further refine results. All File C financial data for this award is returned if omitted. Defaults to None.
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            piid (str): Optional. Award ID to further refine results. All File C financial data for this award is returned if omitted. Defaults to None.
           
         Returns:
-        - dict: A dictionary containing a federal account count.
+            dict: A dictionary containing a federal account count.
         """
         if piid is not None:
             endpoint = f"idvs/count/federal_account/{award_id}/?piid={piid}"
         else:
             endpoint = f"idvs/count/federal_account/{award_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_idv_funding(self, award_id, piid=None, page=1, limit=10, order="desc", sort="reporting_fiscal_date"):
         """
         Returns a list of File C financial data for an IDV award's descendant contracts.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
-        - piid (str): Optional. Award ID to further refine results. All File C financial data for this award is returned if omitted. Defaults to None.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Optional. Number of items to return. Default is 10.
-        - order (str): Order in which to return data. Default is desc, and other option is asc.
-        - sort (str): Sorting parameter. Default is reporting_fiscal_date, but other options are account_title, disaster_emergency_fund_code, gross_outlay_amount, object_class, piid, program_activity, reporting_agency_name, and transaction_obligated_amount.
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            piid (str): Optional. Award ID to further refine results. All File C financial data for this award is returned if omitted. Defaults to None.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Optional. Number of items to return. Default is 10.
+            order (str): Order in which to return data. Default is desc, and other option is asc.
+            sort (str): Sorting parameter. Default is reporting_fiscal_date, but other options are account_title, disaster_emergency_fund_code, gross_outlay_amount, object_class, piid, program_activity, reporting_agency_name, and transaction_obligated_amount.
         
         Returns:
-        - dict: A dictionary containing a list of financial data.
+            dict: A dictionary containing a list of financial data.
         """
         data = {"award_id": award_id,
                 "page": page,
                 "sort": sort,
                 "order": order,
                 "limit": limit        
         }
@@ -1721,38 +1721,38 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_idv_funding_totals(self, award_id):
         """
         Returns award metadata summing the total transaction obligations and counting awarding agencies, funding agencies, and federal accounts for an IDV's children and grandchildren.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
           
         Returns:
-        - dict: A dictionary containing award metadata.
+            dict: A dictionary containing award metadata.
         """
         data = {"award_id": award_id}
         endpoint = "idvs/funding_rollup/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     ### Recipient functions
     def search_recipients(self, order="desc", sort="amount", limit=50, page=1, keyword=None, award_type="all"):
         """
         Returns a list of recipients, their level, DUNS, UEI, and amount.
         
         Args:
-        - order (str): The direction results are sorted by. asc for ascending, desc for descending. Default is desc.
-        - sort (str): The field results are sorted by. Default is amount, but other values are name and duns.
-        - limit (int): Number of results per page. Default is 50. Max is 1000.
-        - page (int): Pagination parameter. Defaults to first page.
-        - keyword (str): The keyword results are filtered by. Searches on name, UEI, or DUNS.        
-        - award_type (str): The award type results are filtered by. Default is all, but other options are contracts, grants, loans, direct_payments, and other_financial_assistance.
+            order (str): The direction results are sorted by. asc for ascending, desc for descending. Default is desc.
+            sort (str): The field results are sorted by. Default is amount, but other values are name and duns.
+            limit (int): Number of results per page. Default is 50. Max is 1000.
+            page (int): Pagination parameter. Defaults to first page.
+            keyword (str): The keyword results are filtered by. Searches on name, UEI, or DUNS.        
+            award_type (str): The award type results are filtered by. Default is all, but other options are contracts, grants, loans, direct_payments, and other_financial_assistance.
         
         Returns:
-        - dict: A dictionary containing a list of recipient data.
+            dict: A dictionary containing a list of recipient data.
         """
         data = {"order": order,
                 "sort": sort,
                 "limit": limit if limit <= 1000 else 1000,
                 "page": page,
                 "award_type": award_type       
         }
@@ -1762,331 +1762,331 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_child_recipients_by_duns_or_uei(self, duns_or_uei, year="latest"):
         """
         Returns a list of child recipients belonging to the given parent recipient DUNS or UEI.
         
         Args:
-        - duns_or_uei (str): Parent recipient's DUNS or UEI.
-        - year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
+            duns_or_uei (str): Parent recipient's DUNS or UEI.
+            year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
         
         Returns:
-        - dict: A dictionary containing a list of child recipients.
+            dict: A dictionary containing a list of child recipients.
         """
         endpoint = f"recipient/children/{duns_or_uei}/?year={year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_recipient_count(self, keyword=None, award_type="all"):
         """
         Returns the count of recipients given an award_type and keyword string.
         
         Args:
-        - keyword (str): The keyword results are filtered by. Searches on name, UEI, or DUNS.        
-        - award_type (str): The award type results are filtered by. Default is all, but other options are contracts, grants, loans, direct_payments, and other_financial_assistance.
+            keyword (str): The keyword results are filtered by. Searches on name, UEI, or DUNS.        
+            award_type (str): The award type results are filtered by. Default is all, but other options are contracts, grants, loans, direct_payments, and other_financial_assistance.
         
         Returns:
-        - dict: A dictionary containing a count of recipients.
+            dict: A dictionary containing a count of recipients.
         """
         data= {"award_type": award_type}
         if keyword is not None:
             data["keyword"] = keyword
         endpoint = "recipient/count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_recipient_overview(self, recipient_id, year="latest"):
         """
         Returns a high-level overview of a specific recipient, given its id.
         
         Args:
-        - recipient_id (str): A unique identifier for the recipient at a specific level (parent, child, or neither).
-        - year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
+            recipient_id (str): A unique identifier for the recipient at a specific level (parent, child, or neither).
+            year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
         
         Returns:
-        - dict: A dictionary containing an overview of recipient.
+            dict: A dictionary containing an overview of recipient.
         """
         endpoint = f"recipient/{recipient_id}/?year={year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_state_metadata(self, fips, year="latest"):
         """
         Returns a high-level overview of a specific state or territory, given its USAspending.gov id.
         
         Args:
-        - fips (str): The FIPS code for the state you want to view. You must include leading zeros.
-        - year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
+            fips (str): The FIPS code for the state you want to view. You must include leading zeros.
+            year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
         
         Returns:
-        - dict: A dictionary containing state metadata.
+            dict: A dictionary containing state metadata.
         """
         endpoint = f"recipient/state/{fips}?year={year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_states(self):
         """
         Returns a list of states and their amounts.
         
         Args:
-        - None
+            None
           
         Returns:
-        - dict: A dictionary containing a list of states.
+            dict: A dictionary containing a list of states.
         """
         endpoint = "recipient/state"
         return mr.make_request(self.base_url+endpoint)
         
     def get_state_award_breakdown(self, fips, year="latest"):
         """
         Returns the award amounts and totals, based on award type, of a specific state or territory, given its USAspending.gov id.
         
         Args:
-        - fips (str): The FIPS code for the state you want to view. You must include leading zeros.
-        - year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
+            fips (str): The FIPS code for the state you want to view. You must include leading zeros.
+            year (str): The fiscal year you would like data for. Use all to view all time or latest to view the latest 12 months. Default is latest.   
         
         Returns:
-        - dict: A dictionary containing amounts and totals of a state.
+            dict: A dictionary containing amounts and totals of a state.
         """
         endpoint = f"recipient/state/awards/{fips}/?year={year}"
         return mr.make_request(self.base_url+endpoint)
         
     ### Differences and discrepancies functions 
     def get_obligation_difference_data(self, toptier_code, fiscal_year, fiscal_period, page=1, limit=10, order="desc", sort="tas"):
         """
         Returns an overview of government agency obligation differences data.
         
         Args:
-        - toptier_code (str): The specific agency code.
-        - fiscal_year (int): The fiscal year.
-        - fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
-        - page (int): Optional pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Defaults to 10.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Default is desc.
-        - sort (str):  A data field that will be used to sort the response array. Default is tas, but other options are difference, file_a_obligation, and file_b_obligation.
+            toptier_code (str): The specific agency code.
+            fiscal_year (int): The fiscal year.
+            fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
+            page (int): Optional pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Defaults to 10.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Default is desc.
+            sort (str):  A data field that will be used to sort the response array. Default is tas, but other options are difference, file_a_obligation, and file_b_obligation.
         Returns:
-        - dict: A dictionary containing an overview of government agency obligation differences data.
+            dict: A dictionary containing an overview of government agency obligation differences data.
         """
         endpoint = f"reporting/agencies/{toptier_code}/differences/?fiscal_year={fiscal_year}&fiscal_period={fiscal_period}&page={page}&limit={limit}&order={order}&sort={sort}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tas_discrepancies_data(self, toptier_code, fiscal_year, fiscal_period, page=1, limit=10, order="desc", sort="amount"):
         """
         Returns an overview of government agency TAS discrepancies data.
         
         Args:
-        - toptier_code (str): The specific agency code.
-        - fiscal_year (int): The fiscal year.
-        - fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
-        - page (int): Optional pagination parameter. Defaults to first page.
-        - limit (int): Number of results per page. Defaults to 10.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Default is desc.
-        - sort (str):  A data field that will be used to sort the response array. Default is amount, but other option is tas.
+            toptier_code (str): The specific agency code.
+            fiscal_year (int): The fiscal year.
+            fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
+            page (int): Optional pagination parameter. Defaults to first page.
+            limit (int): Number of results per page. Defaults to 10.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Default is desc.
+            sort (str):  A data field that will be used to sort the response array. Default is amount, but other option is tas.
         Returns:
-        - dict: A dictionary containing an overview of government agency TAS discrepancies data.
+            dict: A dictionary containing an overview of government agency TAS discrepancies data.
         """
         endpoint = f"reporting/agencies/{toptier_code}/discrepancies/?fiscal_year={fiscal_year}&fiscal_period={fiscal_period}&page={page}&limit={limit}&order={order}&sort={sort}"
         return mr.make_request(self.base_url+endpoint)
         
     ### References functions
     def get_agency_overview_by_agency_id(self, agency_id):
         """
         Returns a high-level overview of a specific government agency, given its USAspending.gov id.
         
         Args:
-        - agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
+            agency_id (int): The unique USAspending.gov agency identifier. This ID is the agency_id value returned in the /api/v2/references/toptier_agencies/ endpoint.
           
         Returns:
-        - dict: A dictionary containing an agency overview.
+            dict: A dictionary containing an agency overview.
         """
         endpoint = f"references/agency/{agency_id}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_award_types(self):
         """
         Returns a grouping of award types.
         
         Args:
-        - None
+            None
           
         Returns:
-        - dict: A dictionary containing a grouping of award types.
+            dict: A dictionary containing a grouping of award types.
         """
         endpoint = "references/award_types"
         return mr.make_request(self.base_url+endpoint)
     
     # This doesn't seem to be working.  
 #    def get_opportunity_totals_for_all_cfdas(self):
 #        """
 #        Returns opportunity totals for a CFDA or all opportunity totals.
 #        
 #        Args:
-#        - None
+#            None
 #          
 #        Returns:
-#        - dict: A dictionary containing opportunity totals for a CFDA or all opportunity totals.
+#            dict: A dictionary containing opportunity totals for a CFDA or all opportunity totals.
 #        """
 #        endpoint = "references/cfda/totals"
 #        return mr.make_request(self.base_url+endpoint)
 
     def get_data_dictionary(self):
         """
         Returns data corresponding to the latest data dictionary csv file.
         
         Args:
-        - None
+            None
           
         Returns:
-        - dict: A dictionary containing data corresponding to the latest data dictionary csv file.
+            dict: A dictionary containing data corresponding to the latest data dictionary csv file.
         """
         endpoint = "references/data_dictionary"
         return mr.make_request(self.base_url+endpoint)
         
     def get_def_codes(self):
         """
         Returns a JSON object describing all Disaster and Emergency Funding (DEF) Codes.
         
         Args:
-        - None
+            None
           
         Returns:
-        - dict: A dictionary containing all Disaster and Emergency Funding (DEF) Codes
+            dict: A dictionary containing all Disaster and Emergency Funding (DEF) Codes
         """
         endpoint = "references/def_codes"
         return mr.make_request(self.base_url+endpoint)
         
     def get_filter_hash_for_url(self, filters):
         """
         Returns a hash for URL, based on selected filter criteria.
         
         Args:
-        - filters (dict): Advanced JSON filtering object. See this endpoint's docs for information on the format of this filtering object.
+            filters (dict): Advanced JSON filtering object. See this endpoint's docs for information on the format of this filtering object.
         
         Returns:
-        - dict: A dictionary containing a hash.
+            dict: A dictionary containing a hash.
         """
         data= {"filters": filters}
         endpoint = "references/filter/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_psc_search_tree_nodes(self, depth=0, Filter=None):
         """
         Returns the basic groupings of Product Service Codes.
         
         Args:
-        - depth (int): Defines how many levels of descendants to return under each node. For example, depth=0 will return a flat array, while depth=2 will populate the children array of each top level node with that node's children and grandchildren. The actual depth of each tree may be less than the value of depth if returned nodes have no children. Negative values are treated as infinite, returning all descendants. Default is 0.
-        - Filter (str):  Restricts results to nodes with a id or description matching the filter string. If depth is greater than zero, nodes will also appear the response if at least one child within depth matches the filter. Default is None.  
+            depth (int): Defines how many levels of descendants to return under each node. For example, depth=0 will return a flat array, while depth=2 will populate the children array of each top level node with that node's children and grandchildren. The actual depth of each tree may be less than the value of depth if returned nodes have no children. Negative values are treated as infinite, returning all descendants. Default is 0.
+            Filter (str):  Restricts results to nodes with a id or description matching the filter string. If depth is greater than zero, nodes will also appear the response if at least one child within depth matches the filter. Default is None.  
         
         Returns:
-        - dict: A dictionary containing the basic groupings of the psc codes.
+            dict: A dictionary containing the basic groupings of the psc codes.
         """
         if Filter is not None:
             endpoint = f"references/filter_tree/psc/?depth={depth}&filter={Filter}"
         else:
             endpoint = f"references/filter_tree/psc/?depth={depth}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tas_search_tree_nodes(self, depth=0, Filter=None):
         """
         Returns a list of toptier agencies that have at least one TAS affiliated with them.
         
         Args:
-        - depth (int): Defines how many levels of descendants to return under each node. For example, depth=0 will return a flat array, while depth=2 will populate the children array of each top level node with that node's children and grandchildren. The actual depth of each tree may be less than the value of depth if returned nodes have no children. Negative values are treated as infinite, returning all descendants. Default is 0.
-        - Filter (str):  Restricts results to nodes with a id or description matching the filter string. If depth is greater than zero, nodes will also appear the response if at least one child within depth matches the filter. Default is None.  
+            depth (int): Defines how many levels of descendants to return under each node. For example, depth=0 will return a flat array, while depth=2 will populate the children array of each top level node with that node's children and grandchildren. The actual depth of each tree may be less than the value of depth if returned nodes have no children. Negative values are treated as infinite, returning all descendants. Default is 0.
+            Filter (str):  Restricts results to nodes with a id or description matching the filter string. If depth is greater than zero, nodes will also appear the response if at least one child within depth matches the filter. Default is None.  
         
         Returns:
-        - dict: A dictionary containing a list of toptier agencies.
+            dict: A dictionary containing a list of toptier agencies.
         """
         if Filter is not None:
             endpoint = f"references/filter_tree/tas/?depth={depth}&filter={Filter}"
         else:
             endpoint = f"references/filter_tree/tas/?depth={depth}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_glossary(self, page=1, limit=10):
         """
         Returns a list of glossary data.
         
         Args:
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Defaults to 10.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Defaults to 10.
           
         Returns:
-        - dict: A dictionary containing a list of glossary data.
+            dict: A dictionary containing a list of glossary data.
         """
         endpoint = f"references/glossary/?page={page}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_filter_object_from_hash(self, Hash):
         """
         Accepts a hash generated by /api/v2/references/filter/ and returns an Advanced Search filter object.
         
         Args:
-        - hash (str): A hash.
+            hash (str): A hash.
         
         Returns:
-        - dict: A dictionary containing a filter object.
+            dict: A dictionary containing a filter object.
         """
         data= {"hash": Hash}
         endpoint = "references/hash/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_naics_codes(self, Filter=None):
         """
         Returns a list of Tier 1 NAICS codes, their descriptions, and a count of their Tier 3 grandchildren. If filter is provided then return parents/grandparents that match the search text.
         
         Args:
-        - Filter (str): Optional. This will filter the NAICS by their descriptions to those matching the text. Default is None.
+            Filter (str): Optional. This will filter the NAICS by their descriptions to those matching the text. Default is None.
         
         Returns:
-        - dict: A dictionary containing a list of naics codes.
+            dict: A dictionary containing a list of naics codes.
         """
         if Filter is not None:
             endpoint = f"references/naics/?filter={Filter}"
         else:
             endpoint = "references/naics"
         return mr.make_request(self.base_url+endpoint)
     
     def get_submission_periods(self, use_cache=False):
         """
         Returns a list of all fields in the "dabs_submission_window_schedule" table except 'id'.
         
         Args:
-        - use_cache (bool): Optional. Whether or not to use a cache when retrieving values. Defaults to false.
+            use_cache (bool): Optional. Whether or not to use a cache when retrieving values. Defaults to false.
         
         Returns:
-        - dict: A dictionary containing a list of all fields in the "dabs_submission_window_schedule" table except 'id'.
+            dict: A dictionary containing a list of all fields in the "dabs_submission_window_schedule" table except 'id'.
         """
         if use_cache:
             endpoint = f"references/submission_periods/?use_cache={use_cache}"
         else:
             endpoint = "references/submission_periods"
         return mr.make_request(self.base_url+endpoint)
         
     def get_toptier_agencies(self, sort="percentage_of_total_budget_authority", order="desc"):
         """
         Returns a list of toptier agencies, their budgetary resources, and and the percent of the total government budget authority this agency accounts for.
         
         Args:
-        - sort (str): A data field that will be used to sort the response array. Defaults to percentage_of_total_budget_authority.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
+            sort (str): A data field that will be used to sort the response array. Defaults to percentage_of_total_budget_authority.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
         
         Returns:
-        - dict: A dictionary containing a list of toptier agencies.
+            dict: A dictionary containing a list of toptier agencies.
         """
         endpoint = f"references/toptier_agencies/?sort={sort}&order={order}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_total_budgetary_resources(self, fiscal_year=None, fiscal_period=None):
         """
         Returns federal budgetary resources by fiscal year and fiscal period.
         
         Args:
-        - fiscal_year (int): Optional. The fiscal year to retrieve, 2017 or later. Defaults to None.
-        - fiscal_period (int): Optional. The fiscal period. If this optional parameter is provided then fiscal_year is a required parameter. If fiscal_period is provided without fiscal_year, a 400 error is returned. Valid values: 2-12 (2 = November ... 12 = September). For retrieving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6). If neither paramater is provided, the entire available history will be returned.
+            fiscal_year (int): Optional. The fiscal year to retrieve, 2017 or later. Defaults to None.
+            fiscal_period (int): Optional. The fiscal period. If this optional parameter is provided then fiscal_year is a required parameter. If fiscal_period is provided without fiscal_year, a 400 error is returned. Valid values: 2-12 (2 = November ... 12 = September). For retrieving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6). If neither paramater is provided, the entire available history will be returned.
         
         Returns:
-        - dict: A dictionary containing federal budgetary resources by fiscal year and fiscal period.
+            dict: A dictionary containing federal budgetary resources by fiscal year and fiscal period.
         """
         if fiscal_year is not None and fiscal_period is None:
             endpoint = f"references/total_budgetary_resources/?fiscal_year={fiscal_year}"
         if fiscal_year is not None and fiscal_period is not None:
             endpoint = f"references/total_budgetary_resources/?fiscal_year={fiscal_year}&fiscal_period={fiscal_period}"
         if fiscal_year is None and fiscal_period is not None:
             print("If fiscal_period parameter is passed, fiscal_year must be passed as well.")
@@ -2097,113 +2097,113 @@
         
     ### Reporting functions   
     def get_agency_overview_by_toptier_code(self, toptier_code, page=1, limit=10, order="desc", sort="current_total_budget_authority_amount"):
         """
         Returns an overview of government agency submission data. 
         
         Args:
-        - toptier_code (str): The specific agency's toptier code.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Defaults to 10.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
-        - sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are fiscal_period, fiscal_year, missing_tas_accounts_count, tas_accounts_total, obligation_difference, percent_of_total_budgetary_resources, recent_publication_date, recent_publication_date_certified, tas_obligation_not_in_gtas_total, unlinked_contract_award_count, and unlinked_assistance_award_count.
+            toptier_code (str): The specific agency's toptier code.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Defaults to 10.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
+            sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are fiscal_period, fiscal_year, missing_tas_accounts_count, tas_accounts_total, obligation_difference, percent_of_total_budgetary_resources, recent_publication_date, recent_publication_date_certified, tas_obligation_not_in_gtas_total, unlinked_contract_award_count, and unlinked_assistance_award_count.
           
         Returns:
-        - dict: A dictionary containing an overview of government agency submission data.
+            dict: A dictionary containing an overview of government agency submission data.
         """
         endpoint = f"reporting/agencies/{toptier_code}/overview/?page={page}&limit={limit}&order={order}&sort={sort}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agency_overview_by_year(self, fiscal_year, fiscal_period, Filter=None, page=1, limit=10, order="desc", sort="current_total_budget_authority_amount"):
         """
         Returns an overview of government agency submission data. 
         
         Args:
-        - fiscal_year (int): The fiscal year.
-        - fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
-        - Filter (str): The agency name or abbreviation to filter on (partial match, case insesitive). Defaults to None.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Defaults to 10.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
-        - sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are fiscal_period, fiscal_year, missing_tas_accounts_count, tas_accounts_total, obligation_difference, percent_of_total_budgetary_resources, recent_publication_date, recent_publication_date_certified, tas_obligation_not_in_gtas_total, unlinked_contract_award_count, and unlinked_assistance_award_count.
+            fiscal_year (int): The fiscal year.
+            fiscal_period (int): The fiscal period. Valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly data, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
+            Filter (str): The agency name or abbreviation to filter on (partial match, case insesitive). Defaults to None.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Defaults to 10.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
+            sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are fiscal_period, fiscal_year, missing_tas_accounts_count, tas_accounts_total, obligation_difference, percent_of_total_budgetary_resources, recent_publication_date, recent_publication_date_certified, tas_obligation_not_in_gtas_total, unlinked_contract_award_count, and unlinked_assistance_award_count.
           
         Returns:
-        - dict: A dictionary containing an overview of government agency submission data.
+            dict: A dictionary containing an overview of government agency submission data.
         """
         if Filter is not None:
             endpoint = f"reporting/agencies/overview/?fiscal_year={fiscal_year}&fiscal_period={fiscal_period}&filter={Filter}&page={page}&limit={limit}&order={order}&sort={sort}"
         else:
             endpoint = f"reporting/agencies/overview/?fiscal_year={fiscal_year}&fiscal_period={fiscal_period}&page={page}&limit={limit}&order={order}&sort={sort}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_agency_reporting_publish_dates(self, fiscal_year, Filter=None, page=1, limit=10, order="desc", sort="current_total_budget_authority_amount"):
         """
         Returns list of agency submission information, included published and certified dates for the fiscal year.
         
         Args:
-        - fiscal_year (int): The fiscal year.
-        - Filter (str): The agency name or abbreviation to filter on (partial match, case insesitive). Defaults to None.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Defaults to 10.
-        - order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
-        - sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are agency_name, abbreviation, toptier_code, and publication_date.
+            fiscal_year (int): The fiscal year.
+            Filter (str): The agency name or abbreviation to filter on (partial match, case insesitive). Defaults to None.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Defaults to 10.
+            order (str): The direction (asc or desc) that the sort field will be sorted in. Defaults to desc.
+            sort (str): A data field that will be used to sort the response array. Default is current_total_budget_authority_amount, but other options are agency_name, abbreviation, toptier_code, and publication_date.
           
         Returns:
-        - dict: A dictionary containing a list of agency submission information, included published and certified dates for the fiscal year.
+            dict: A dictionary containing a list of agency submission information, included published and certified dates for the fiscal year.
         """
         if Filter is not None:
             endpoint = f"reporting/agencies/publish_dates/?fiscal_year={fiscal_year}&filter={Filter}&page={page}&limit={limit}&order={order}&sort={sort}"
         else:
             endpoint = f"reporting/agencies/publish_dates/?fiscal_year={fiscal_year}&page={page}&limit={limit}&order={order}&sort={sort}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_reporting_publishing_dates_for_single_agency(self, toptier_code, fiscal_year, fiscal_period):
         """
         Returns the history of publication and certification dates for a single agency's submission. 
         
         Args:
-        - toptier_code (str): The specific agency's toptier code.
-        - fiscal_year (int): The fiscal year of the submission.
-        - fiscal_period (int): The fiscal period of the submission. valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly submissions, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
+            toptier_code (str): The specific agency's toptier code.
+            fiscal_year (int): The fiscal year of the submission.
+            fiscal_period (int): The fiscal period of the submission. valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly submissions, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
              
         Returns:
-        - dict: A dictionary containing a publishing and certification data for a single agency.
+            dict: A dictionary containing a publishing and certification data for a single agency.
         """        
         endpoint = f"reporting/agencies/{toptier_code}/{fiscal_year}/{fiscal_period}/submission_history"
         return mr.make_request(self.base_url+endpoint)
         
     def get_unlinked_awards_for_agency(self, toptier_code, fiscal_year, fiscal_period, Type):
         """
         Returns the number of unlinked and linked awards for the agency in the provided fiscal year and period.
         
         Args:
-        - toptier_code (str): The specific agency's toptier code.
-        - fiscal_year (int): The fiscal year of the submission.
-        - fiscal_period (int): The fiscal period of the submission. valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly submissions, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
-        - Type (str): Possible vales are assistance and procurement. 
+            toptier_code (str): The specific agency's toptier code.
+            fiscal_year (int): The fiscal year of the submission.
+            fiscal_period (int): The fiscal period of the submission. valid values: 2-12 (2 = November ... 12 = September) For retriving quarterly submissions, provide the period which equals 'quarter * 3' (e.g. Q2 = P6).
+            Type (str): Possible vales are assistance and procurement. 
         
         Returns:
-        - dict: A dictionary containing number of unlinked and linked awards.
+            dict: A dictionary containing number of unlinked and linked awards.
         """        
         endpoint = f"reporting/agencies/{toptier_code}/{fiscal_year}/{fiscal_period}/unlinked_awards/{Type}"
         return mr.make_request(self.base_url+endpoint)
         
     ### Search functions
     def get_new_awards_over_time(self, start_date, end_date, recipient_id, group="quarter"):
         """
         Returns the count of new awards grouped by time period in ascending order (earliest to most recent).
         
         Args:
-        - start_date (str): (YYYY-MM-DD) Currently limited to an earliest date of 2007-10-01 (FY2008). For data going back to 2000-10-01 (FY2001), use either the Custom Award Download feature on the website or one of our download or bulk_download API endpoints.
-        - end_date (str): (YYYY-MM-DD) Currently limited to an earliest date of 2007-10-01 (FY2008). For data going back to 2000-10-01 (FY2001), use either the Custom Award Download feature on the website or one of our download or bulk_download API endpoints.
-        - recipient_id (str): Optional. A hash of recipient UEI, DUNS, name, and level. A unique identifier for recipients. Defaults to None.
-        - group (str): How to group the data. Default is quarter, but other options are fiscal_year and month.
+            start_date (str): (YYYY-MM-DD) Currently limited to an earliest date of 2007-10-01 (FY2008). For data going back to 2000-10-01 (FY2001), use either the Custom Award Download feature on the website or one of our download or bulk_download API endpoints.
+            end_date (str): (YYYY-MM-DD) Currently limited to an earliest date of 2007-10-01 (FY2008). For data going back to 2000-10-01 (FY2001), use either the Custom Award Download feature on the website or one of our download or bulk_download API endpoints.
+            recipient_id (str): Optional. A hash of recipient UEI, DUNS, name, and level. A unique identifier for recipients. Defaults to None.
+            group (str): How to group the data. Default is quarter, but other options are fiscal_year and month.
         
         Returns:
-        - dict: A dictionary containing a count of new awards.
+            dict: A dictionary containing a count of new awards.
         """
         data = {
                   "group": group,
                   "filters": {
                       "recipient_id": recipient_id,
                       "time_period": [
                           {
@@ -2217,26 +2217,26 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_award(self, filters, fields, limit=10, order="desc", page=1, sort=None, subawards=False, last_record_unique_id=None, last_record_sort_value=None):
         """
         Returns the fields of the filtered awards.
          
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - fields (list): Spending by award fields to return. See this endpoint's docs for the available fields.
-        - limit (int): Number of items to return. Default is 10.
-        - order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order. Default is desc and other option is asc.
-        - page (int): Pagination parameter. Defaults to first page.
-        - sort (str): Optional parameter indicating what value results should be sorted by. Valid options are any of the fields in the JSON objects in the response. Defaults to the first field provided, but here it defaults to None.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
-        - last_record_unique_id (int): Optional. The unique id of the last record in the results set. Used in the experimental Elasticsearch API functionality. Defaults to None.
-        - last_record_sort_value (str): Optional. The value of the last record that is being sorted on. Used in the experimental Elasticsearch API functionality. Defaults to None.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            fields (list): Spending by award fields to return. See this endpoint's docs for the available fields.
+            limit (int): Number of items to return. Default is 10.
+            order (str): Indicates what direction results should be sorted by. Valid options include asc for ascending order or desc for descending order. Default is desc and other option is asc.
+            page (int): Pagination parameter. Defaults to first page.
+            sort (str): Optional parameter indicating what value results should be sorted by. Valid options are any of the fields in the JSON objects in the response. Defaults to the first field provided, but here it defaults to None.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            last_record_unique_id (int): Optional. The unique id of the last record in the results set. Used in the experimental Elasticsearch API functionality. Defaults to None.
+            last_record_sort_value (str): Optional. The value of the last record that is being sorted on. Used in the experimental Elasticsearch API functionality. Defaults to None.
         
         Returns:
-        - dict: A dictionary containing the fields of the filtered awards.
+            dict: A dictionary containing the fields of the filtered awards.
         """
         data = {
               "subawards": subawards,
               "limit": limit,
               "page": page,
               "order": order,
               "filters": filters,
@@ -2252,247 +2252,247 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_award_count(self, filters, subawards=False):
         """
         Returns the number of awards in each award type (Contracts, Loans, Direct Payments, Grants, Other and IDVs).
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a number of awards.
+            dict: A dictionary containing a number of awards.
         """
         data = {"filters": filters,
                 "subawards": subawards} 
         endpoint = "search/spending_by_award_count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_awarding_agency(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Awarding Agencies sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Awarding Agencies sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Awarding Agencies sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "awarding_agency",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/awarding_agency/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_awarding_subagency(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Awarding Subagencies sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Awarding Subagencies sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Awarding Subagencies sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "awarding_subagency",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/awarding_subagency/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_cfda(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of CFDA sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of CFDA sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of CFDA sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "cfda",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/cfda/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_country(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Countries sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Countries sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Countries sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "country",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/country/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_county(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Counties sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Counties sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Counties sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "county",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/county/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_district(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Congressional Districts sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Congressional Districts sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Congressional Districts sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "district",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/district/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_federal_account(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Federal Accounts sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Federal Accounts sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Federal Accounts sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "federal_account",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/federal_account/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_funding_agency(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Funding Agencies sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Funding Agencies sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Funding Agencies sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "funding_agency",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/funding_agency/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_funding_subagency(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of Funding Subagencies sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of Funding Subagencies sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of Funding Subagencies sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "funding_subagency",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/funding_subagency/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_naics(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of NAICS sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of NAICS sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of NAICS sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "naics",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/naics/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_psc(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of PSC sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of PSC sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of PSC sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "psc",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/psc/"
@@ -2500,64 +2500,64 @@
     
     # This enpoint doesn't seem to be working  
 #    def get_spending_by_recipient(self, filters, limit=10, page=1, subawards=False):
 #        """
 #        Returns a list of the top results of Recipients sorted by the total amounts in descending order.
 #        
 #        Args:
-#        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-#        - limit (int): Number of items to return. Default is 10.
-#        - page (int): Pagination parameter. Defaults to first page.
-#        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+#            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+#            limit (int): Number of items to return. Default is 10.
+#            page (int): Pagination parameter. Defaults to first page.
+#            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
 #          
 #        Returns:
-#        - dict: A dictionary containing a list of the top results of Recipients sorted by the total amounts in descending order.
+#            dict: A dictionary containing a list of the top results of Recipients sorted by the total amounts in descending order.
 #        """
 #        data = {"filters": filters,
 #                "category": "recipient",
 #                "subawards": subawards,
 #                "page": page,
 #                "limit": limit} 
 #        endpoint = "search/spending_by_category/recipient/"
 #        return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
 
     def get_spending_by_state_territory(self, filters, limit=10, page=1, subawards=False):
         """
         Returns a list of the top results of State Territories sorted by the total amounts in descending order.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - limit (int): Number of items to return. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            limit (int): Number of items to return. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of the top results of State Territories sorted by the total amounts in descending order.
+            dict: A dictionary containing a list of the top results of State Territories sorted by the total amounts in descending order.
         """
         data = {"filters": filters,
                 "category": "state_territory",
                 "subawards": subawards,
                 "page": page,
                 "limit": limit} 
         endpoint = "search/spending_by_category/state_territory/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_geography(self, filters, scope, geo_layer, geo_layer_filters=None, subawards=False):
         """
         Returns aggregated obligation amounts in different geographic areas. 
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - scope (str): When fetching transactions, use the primary place of performance or recipient location. Options are place_of_performance and recipient_location.
-        - geo_layer (str): Set the type of areas in the response. Options are state, county, district, and country.
-        - geo_layer_filters (list): Optional. List of U.S. state codes, U.S. county codes, U.S. Congressional districts, or ISO 3166-1 alpha-3 country codes to show results for.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            scope (str): When fetching transactions, use the primary place of performance or recipient location. Options are place_of_performance and recipient_location.
+            geo_layer (str): Set the type of areas in the response. Options are state, county, district, and country.
+            geo_layer_filters (list): Optional. List of U.S. state codes, U.S. county codes, U.S. Congressional districts, or ISO 3166-1 alpha-3 country codes to show results for.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing aggregated obligation amounts in different geographic areas.
+            dict: A dictionary containing aggregated obligation amounts in different geographic areas.
         """
         data = {"filters": filters,
                 "scope": scope,
                 "geo_layer": geo_layer,
                 "subawards": subawards} 
         if geo_layer_filters is not None:
             data["geo_layer_filters"] = geo_layer_filters
@@ -2565,23 +2565,23 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_transaction(self, filters, fields, limit=10, page=1, sort="Transaction Amount", order="desc"):
         """
         Returns transaction records which match the provided filters. 
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - fields (list): The field names to include in the response.
-        - limit (int): The number of results per page. Default is 10.
-        - page (int): Pagination parameter. Defaults to first page.
-        - sort (str): The field on which to order results in the response. Default is "Transaction Amount"
-        - order (str): The direction in which to order results. asc for ascending or desc for descending. Default is desc.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            fields (list): The field names to include in the response.
+            limit (int): The number of results per page. Default is 10.
+            page (int): Pagination parameter. Defaults to first page.
+            sort (str): The field on which to order results in the response. Default is "Transaction Amount"
+            order (str): The direction in which to order results. asc for ascending or desc for descending. Default is desc.
         
         Returns:
-        - dict: A dictionary containing transaction records which match the provided filters.   
+            dict: A dictionary containing transaction records which match the provided filters.   
         """
         data = {"filters": filters,
                 "fields": fields,
                 "limit": limit,
                 "page": page,
                 "sort": sort,
                 "order": order
@@ -2590,87 +2590,87 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_by_transaction_count(self, filters):
         """
         Returns counts of transaction records which match the provided filters. 
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
           
         Returns:
-        - dict: A dictionary containing counts transaction records which match the provided filters.   
+            dict: A dictionary containing counts transaction records which match the provided filters.   
         """
         data = {"filters": filters} 
         endpoint = "search/spending_by_transaction_count/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_spending_over_time(self, filters, group="fiscal_year", subawards=False):
         """
         Returns a list of aggregated award amounts grouped by time period in ascending order (earliest to most recent).   
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
-        - group (str): Default is fiscal_year, and other options are quarter and month.
-        - subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            group (str): Default is fiscal_year, and other options are quarter and month.
+            subawards (bool): True when you want to group by Subawards instead of Awards. Defaulted to False.
           
         Returns:
-        - dict: A dictionary containing a list of aggregated award amounts grouped by time period in ascending order (earliest to most recent).
+            dict: A dictionary containing a list of aggregated award amounts grouped by time period in ascending order (earliest to most recent).
         """
         data = {"group": group,
                 "filters": filters,
                 "subawards": subawards} 
         endpoint = "search/spending_over_time/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_transaction_spending_summary(self, filters):
         """
         Returns the high-level aggregations of the counts and dollar amounts for all transactions which match the keyword filter.
         
         Args:
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
           
         Returns:
-        - dict: A dictionary containing the high-level aggregations of the counts and dollar amounts for all transactions which match the keyword filter.
+            dict: A dictionary containing the high-level aggregations of the counts and dollar amounts for all transactions which match the keyword filter.
         """
         data = {"filters": filters} 
         endpoint = "search/transaction_spending_summary/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
     
     # Spending Explorer    
     def explore_spending(self, Type, filters):
         """
         Returns spending data information through various types of filters.
         
         Args:
-        - Type (str): Options are federal_account, object_class, recipient, award, budget_function, budget_subfunction, agency, and program_activity.   
-        - filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
+            Type (str): Options are federal_account, object_class, recipient, award, budget_function, budget_subfunction, agency, and program_activity.   
+            filters (dict): An advanced JSON search object. See this endpoint's docs for the format of this object.
           
         Returns:
-        - dict: A dictionary containing spending data information through various types of filters.
+            dict: A dictionary containing spending data information through various types of filters.
         """ 
         data = {"type": Type,
                 "filters": filters
                 } 
         endpoint = "spending/"
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
     
     # Subawards    
     def get_subawards(self, sort, page=1, limit=10, order="desc", award_id=None):
         """
         Returns a filtered set of subawards.
         
         Args:
-        - sort (str): Required sorting parameter. Options are subaward_number, id, description, action_date, amount, recipient_name.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Default is 10.
-        - order (str): Ordering parameter. Default is desc (descending) and other option is asc (ascending).
-        - award_id (str): Optional. Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            sort (str): Required sorting parameter. Options are subaward_number, id, description, action_date, amount, recipient_name.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Default is 10.
+            order (str): Ordering parameter. Default is desc (descending) and other option is asc (ascending).
+            award_id (str): Optional. Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
         
         Returns:
-        - dict: A dictionary containing a filtered set of subawards.
+            dict: A dictionary containing a filtered set of subawards.
         """ 
         data = {"sort": sort,
                 "page": page,
                 "limit": limit,
                 "order": order
                 } 
         if award_id is not None:
@@ -2679,22 +2679,22 @@
         return mr.make_request_with_post_and_json(self.base_url+endpoint, json=data)
         
     def get_transactions(self, award_id, sort="action_date", page=1, limit=10, order="desc"):
         """
         Returns a list of transactions, their amount, type, action date, action type, modification number, and description.
         
         Args:
-        - award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
-        - sort (str): The field results are sorted by. Default is action_date, but other options are modification_number, federal_action_obligation, face_value_loan_guarantee, original_loan_subsidy_cost, action_type_description, and description.
-        - page (int): Pagination parameter. Defaults to first page.
-        - limit (int): Number of items per page. Default is 10. Max is 5000.
-        - order (str): Ordering parameter. Default is desc (descending) and other option is asc (ascending).
+            award_id (str): Either a "generated" natural award id (string) or a database surrogate award id (number). Generated award identifiers are preferred as they are effectively permanent. Surrogate award ids are retained for backward compatibility but are deprecated.
+            sort (str): The field results are sorted by. Default is action_date, but other options are modification_number, federal_action_obligation, face_value_loan_guarantee, original_loan_subsidy_cost, action_type_description, and description.
+            page (int): Pagination parameter. Defaults to first page.
+            limit (int): Number of items per page. Default is 10. Max is 5000.
+            order (str): Ordering parameter. Default is desc (descending) and other option is asc (ascending).
          
         Returns:
-        - dict: A dictionary containing a list of transactions, their amount, type, action date, action type, modification number, and description.
+            dict: A dictionary containing a list of transactions, their amount, type, action date, action type, modification number, and description.
         """
         data = {"award_id": award_id,
                 "sort": sort,
                 "page": page,
                 "limit": limit,
                 "order": order
                 }
```

### Comparing `nokey-0.7.3/nokey/health/open_disease.py` & `nokey-0.7.4/nokey/health/open_disease.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 from .. helperFuncs import make_request as mr
 
 class OpenDisease:
     """
     A class for interacting with the Open Disease API.
     
     Attributes:
-    - base_url: The base URL for the API.
-    - about: A short description of the API.
+        base_url: The base URL for the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="open_disease_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://disease.sh/v3/"
         self.about = "Open Disease is a Third Party API for reliable global disease information, serving COVID and influenza data (Note: None of the data in this API seems to be up to date)"
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Open Disease API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://disease.sh/docs/"
         
     # COVID WORLDOMETERS
     def get_worldometers_global_covid_data(self, day=0, allow_null=False):
         """
         Returns global COVID-19 totals for today, yesterday and two days ago.
         
         Args:
-        - day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing global COVID-19 totals.
+            dict: A dictionary containing global COVID-19 totals.
         """
         if day == 0:
             endpoint = f"covid-19/all?allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
         elif day == 1:
             endpoint = f"covid-19/all?yesterday=true&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
@@ -54,20 +54,20 @@
             exit()
             
     def get_worldometers_covid_data_for_all_states(self, sort=None, day=0, allow_null=False):
         """
         Returns COVID-19 totals for the states.
         
         Args:
-        - sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
-        - day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
+            day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing state COVID-19 totals.
+            dict: A dictionary containing state COVID-19 totals.
         """
         if sort is not None:
             if day == 0:
                 endpoint = f"covid-19/states?sort={sort}&allowNull={str(allow_null).lower()}"
                 return mr.make_request(self.base_url+endpoint)
             elif day == 1:
                 endpoint = f"covid-19/states?sort={sort}&yesterday=true&allowNull={str(allow_null).lower()}"
@@ -87,20 +87,20 @@
                 exit()
                 
     def get_worldometers_covid_data_for_specific_states(self, states, day=0, allow_null=False):
         """
         Returns COVID-19 totals for the specified state(s).
         
         Args:
-        - states (str): State name or comma separated non-spaced names, spelled correctly.
-        - day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            states (str): State name or comma separated non-spaced names, spelled correctly.
+            day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for specified state(s).
+            dict: A dictionary containing COVID-19 totals for specified state(s).
         """
         if day == 0:
             endpoint = f"covid-19/states/{states}?allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
         elif day == 1:
             endpoint = f"covid-19/states/{states}?yesterday=true&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
@@ -109,20 +109,20 @@
             exit()
             
     def get_worldometers_covid_data_for_all_continents(self, sort=None, day=0, allow_null=False):
         """
         Returns COVID-19 totals for all the continents.
         
         Args:
-        - sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
-        - day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
+            day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for the continents.
+            dict: A dictionary containing COVID-19 totals for the continents.
         """
         if sort is not None:
             if day == 0:
                 endpoint = f"covid-19/continents?sort={sort}&allowNull={str(allow_null).lower()}"
                 return mr.make_request(self.base_url+endpoint)
             elif day == 1:
                 endpoint = f"covid-19/continents?sort={sort}&yesterday=true&allowNull={str(allow_null).lower()}"
@@ -148,21 +148,21 @@
                 exit()
                 
     def get_worldometers_covid_data_for_specific_continent(self, continent, day=0, strict=True, allow_null=False):
         """
         Returns COVID-19 totals for the specified continent.
         
         Args:
-        - continent (str): Name of the continent, spelled correctly.
-        - day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
-        - strict (bool): Setting to false gives you the ability to fuzzy search continents (i.e. Oman vs. rOMANia). Default is True.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            continent (str): Name of the continent, spelled correctly.
+            day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
+            strict (bool): Setting to false gives you the ability to fuzzy search continents (i.e. Oman vs. rOMANia). Default is True.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for specified continent.
+            dict: A dictionary containing COVID-19 totals for specified continent.
         """
         if day == 0:
             endpoint = f"covid-19/continents/{continent}?strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
         elif day == 1:
             endpoint = f"covid-19/continents/{continent}?yesterday=true&strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
@@ -174,20 +174,20 @@
             exit()
             
     def get_worldometers_covid_data_for_all_countries(self, sort=None, day=0, allow_null=False):
         """
         Returns COVID-19 totals for all the countries.
         
         Args:
-        - sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
-        - day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            sort (str): Provided a key (e.g. cases, todayCases, deaths, active), result will be sorted from greatest to least. See docs for possible fields to sort by. Default is None.
+            day (int): Which day's data to return. Supported values are 0 for today and 1 for yesterday. Default is 0, today.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for the countries.
+            dict: A dictionary containing COVID-19 totals for the countries.
         """
         if sort is not None:
             if day == 0:
                 endpoint = f"covid-19/countries?sort={sort}&allowNull={str(allow_null).lower()}"
                 return mr.make_request(self.base_url+endpoint)
             elif day == 1:
                 endpoint = f"covid-19/countries?sort={sort}&yesterday=true&allowNull={str(allow_null).lower()}"
@@ -213,21 +213,21 @@
                 exit()
                 
     def get_worldometers_covid_data_for_specific_country(self, country, day=0, strict=True, allow_null=False):
         """
         Returns COVID-19 totals for the specified country.
         
         Args:
-        - country (str): A country name, iso2, iso3, or country ID code
-        - day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
-        - strict (bool): Setting to false gives you the ability to fuzzy search countries (i.e. Oman vs. rOMANia). Default is True.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            country (str): A country name, iso2, iso3, or country ID code
+            day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
+            strict (bool): Setting to false gives you the ability to fuzzy search countries (i.e. Oman vs. rOMANia). Default is True.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for specified country.
+            dict: A dictionary containing COVID-19 totals for specified country.
         """
         if day == 0:
             endpoint = f"covid-19/countries/{country}?strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
         elif day == 1:
             endpoint = f"covid-19/countries/{country}?yesterday=true&strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
@@ -239,21 +239,21 @@
             exit()
             
     def get_worldometers_covid_data_for_specific_countries(self, countries, day=0, strict=True, allow_null=False):
         """
         Returns COVID-19 totals for the specified countries.
         
         Args:
-        - countries (str): Multiple country names, iso2s, iso3s, or country ID codes, separated by commas, non spaces.
-        - day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
-        - strict (bool): Setting to false gives you the ability to fuzzy search countries (i.e. Oman vs. rOMANia). Default is True.
-        - allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
+            countries (str): Multiple country names, iso2s, iso3s, or country ID codes, separated by commas, non spaces.
+            day (int): Which day's data to return. Supported values are 0 for today, 1 for yesterday, and 2 for the day before yesterday. Default is 0, today.
+            strict (bool): Setting to false gives you the ability to fuzzy search countries (i.e. Oman vs. rOMANia). Default is True.
+            allow_null (bool): True if, where the value is 0, null is instead retired. Default is False.
         
         Returns:
-        - dict: A dictionary containing COVID-19 totals for specified countries.
+            dict: A dictionary containing COVID-19 totals for specified countries.
         """
         if day == 0:
             endpoint = f"covid-19/countries/{countries}?strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
         elif day == 1:
             endpoint = f"covid-19/countries/{countries}?yesterday=true&strict={str(strict).lower()}&allowNull={str(allow_null).lower()}"
             return mr.make_request(self.base_url+endpoint)
@@ -268,385 +268,386 @@
     # JHUCSSE (Johns Hopkins University) COVID data
     # This data doesn't seem to be current. It seems to end at 3/9/23.
     def get_jhu_global_time_series_covid_data(self, last_days=30):
         """
         Returns COVID-19 time series data for all countries and all their provences.
         
         Args:
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_global_accumulated_covid_data(self, last_days=30):
         """
         Returns global accumulated COVID-19 time series data for all countries and all their provences.
         
         Args:
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing global accumulated COVID-19 time series data.
+            dict: A dictionary containing global accumulated COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/all?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_time_series_covid_data_for_country(self, country, last_days=30):
         """
         Returns COVID-19 time series data for a specific country.
         
         Args:
-        - country (str): A country name, iso2, iso3, or country ID code.
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            country (str): A country name, iso2, iso3, or country ID code.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/{country}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_time_series_covid_data_for_countries(self, countries, last_days=30):
         """
         Returns COVID-19 time series data for a specific countries.
         
         Args:
-        - country (str): Multiple country names, iso2s, iso3s, or country ID codes, in comma separated no spaced string.
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            country (str): Multiple country names, iso2s, iso3s, or country ID codes, in comma separated no spaced string.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/{countries}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_time_series_covid_data_for_province(self, province, country, last_days=30):
         """
         Returns COVID-19 time series data for a specific province in a country.
         
         Args:
-        - country (str): A country name, iso2, iso3, or country ID code.
-        - province (str): Province name. All available names can be found in the /v3/covid-19/historical/{query} endpoint.
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            country (str): A country name, iso2, iso3, or country ID code.
+            province (str): Province name. All available names can be found in the /v3/covid-19/historical/{query} endpoint.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/{country}/{province}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_time_series_covid_data_for_provinces(self, provinces, country, last_days=30):
         """
         Returns COVID-19 time series data for a specific set of provinces in a country.
         
         Args:
-        - country (str): A country name, iso2, iso3, or country ID code.
-        - province (str): Provinces spelled correctly separated by ',' or '|' delimiters, never both in the same query.
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            country (str): A country name, iso2, iso3, or country ID code.
+            province (str): Provinces spelled correctly separated by ',' or '|' delimiters, never both in the same query.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/{country}/{provinces}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_us_states_jhu(self):
         """
         Returns all possible US States and provinces to query the /historical/usacounties/{state} endpoint with.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing all US states and provinces.
+            list: A list containing all US states and provinces.
         """
         endpoint = "covid-19/historical/usacounties"
         return mr.make_request(self.base_url+endpoint)
         
     def get_jhu_time_series_covid_data_for_state(self, state, last_days=30):
         """
         Returns COVID-19 time series data for all counties in a specific state.
         
         Args:
-        - state (str): US state name, validated in the array returned from the /v3/covid-19/historical/usacounties endpoint.
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            state (str): US state name, validated in the array returned from the /v3/covid-19/historical/usacounties endpoint.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/historical/usacounties/{state.lower()}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     # NEW YORK TIMES (NYT) COVID DATA (This doesn't seem up to date. Last date seems to be 2/23/23)
     def get_nyt_time_series_covid_data_for_all_states(self, last_days=30):
         """
         Returns COVID-19 time series data for all states, with an entry for each day since the pandemic began.
         
         Args:
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/nyt/states/?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_nyt_time_series_covid_data_for_specific_states(self, states, last_days=30):
         """
         Returns COVID-19 time series data for specific state(s), with an entry for each day since the pandemic began.
         
         Args:
-        - states (str): State name(s), separated by commas (e.g. 'Illinois, California').
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            states (str): State name(s), separated by commas (e.g. 'Illinois, California').
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/nyt/states/{states}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_nyt_time_series_covid_data_for_all_us_counties(self, last_days=30):
         """
         Returns COVID-19 time series data for all available US counties, with an entry for each day since the pandemic began.
         
         Args:
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/nyt/counties/?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_nyt_time_series_covid_data_for_specific_us_counties(self, counties, last_days=30):
         """
         Returns COVID-19 time series data for specific state(s), with an entry for each day since the pandemic began.
         
         Args:
-        - states (str): County name(s), separated by commas (e.g. 'Alameda, Humboldt').
-        - last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
+            states (str): County name(s), separated by commas (e.g. 'Alameda, Humboldt').
+            last_days (int, str): Number of days' data to return. Use 'all' to return all data. Default is 30.
         
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = f"covid-19/nyt/counties/{counties}?lastdays={last_days}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_nyt_time_series_covid_data_for_entire_usa(self):
         """
         Returns COVID-19 time series data for entire USA, with an entry for each day since the pandemic began.
         
         Args:
-        - None 
+            None 
+            
         Returns:
-        - dict: A dictionary containing COVID-19 time series data.
+            dict: A dictionary containing COVID-19 time series data.
         """
         endpoint = "covid-19/nyt/usa"
         return mr.make_request(self.base_url+endpoint)
         
         
     # APPLE COVID-19 DATA (COVID-19 related mobility trend data from Apple). This data is also not current. It goes up to 4/12/22.
     def get_all_countries_apple(self):
         """
         Returns a list of supported country names.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing supported country names.
+            list: A list containing supported country names.
         """
         endpoint = "covid-19/apple/countries"
         return mr.make_request(self.base_url+endpoint)
         
     def get_apple_supported_subregions_for_country(self, country):
         """
         Returns a list of supported subregions in a country where data is available.
         
         Args:
-        - country (str): A valid country name from the /v3/covid-19/apple/countries endpoint
+            country (str): A valid country name from the /v3/covid-19/apple/countries endpoint
         
         Returns:
-        - dict: A dictionary containing a list of supported subregions.
+            dict: A dictionary containing a list of supported subregions.
         """
         endpoint = f"covid-19/apple/countries/{country}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_apple_mobility_data_for_subregions(self, country, subregions):
         """
         Returns a list of mobility data entries for subregion(s) every day since January 13th. Each entry has driving, transit, and walking data with an associated number of percentage change since January 13th. 
         
         Args:
-        - country (str): A valid country name from the /v3/covid-19/apple/countries endpoint.
-        - subregions (str): Valid subregion(s) from the /v3/covid-19/apple/countries/{country} endpoint, separated by with commas.
+            country (str): A valid country name from the /v3/covid-19/apple/countries endpoint.
+            subregions (str): Valid subregion(s) from the /v3/covid-19/apple/countries/{country} endpoint, separated by with commas.
         
         Returns:
-        - dict: A dictionary containing a list of mobility data.
+            dict: A dictionary containing a list of mobility data.
         """
         endpoint = f"covid-19/apple/countries/{country}/{subregions}"
         return mr.make_request(self.base_url+endpoint)
         
         
     # GOVERNMENT COVID-19 DATA. (Data not current. It stops at 12/1/23)
     def get_all_countries_gov(self):
         """
         Returns a list of supported country names for government specific data.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing supported country names.
+            list: A list containing supported country names.
         """
         endpoint = "covid-19/gov"
         return mr.make_request(self.base_url+endpoint)
         
     def get_gov_covid_data_for_country(self, country, allow_null=False):
         """
         Returns government supported data for a specific country.
         
         Args:
-        - country (str): A valid country name from the /v3/covid-19/gov endpoint.
-        - allow_null (bool): By default, if a value is missing, it is returned as 0. This allows nulls to be returned.
+            country (str): A valid country name from the /v3/covid-19/gov endpoint.
+            allow_null (bool): By default, if a value is missing, it is returned as 0. This allows nulls to be returned.
         
         Returns:
-        - dict: A dictionary containing a list of supported subregions.
+            dict: A dictionary containing a list of supported subregions.
         """
         endpoint = f"covid-19/gov/{country}?allowNull={str(allow_null).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
         
     # VACCINE TRIAL DATA (RAPS - Regulatory Affairs Professional Society) (The dates of the data are current, but the data itself is not)
     #This endpoint doesn't seem to be working.
 #    def get_raps_covid_vaccine_trial_data(self):
 #        """
 #        Returns vaccine trial data from RAPS.
 #        
 #        Args:
-#        - None
+#            None
 #        
 #        Returns:
-#        - dict: A dictionary containing vaccine trial data.
+#            dict: A dictionary containing vaccine trial data.
 #        """
 #        endpoint = "covid-19/vaccine"
 #        return mr.make_request(self.base_url+endpoint)
 
     def get_raps_total_covid_vaccines_administered(self, last_days=30, full_data=False):
         """
         Returns total global COVID-19 vaccine doses administered. Sourced from https://covid.ourworldindata.org.
         
         Args:
-        - last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
-        - full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
+            last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
+            full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
         
         Returns:
-        - dict: A dictionary containing vaccine administration data.
+            dict: A dictionary containing vaccine administration data.
         """
         endpoint = f"covid-19/vaccine/coverage?lastdays={last_days}&fullData={str(full_data).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_raps_covid_vaccines_administered_for_all_countries(self, last_days=30, full_data=False):
         """
         Returns Get COVID-19 vaccine doses administered for all countries that have reported rolling out vaccination. Sourced from https://covid.ourworldindata.org/
         
         Args:
-        - last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
-        - full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
+            last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
+            full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
         
         Returns:
-        - dict: A dictionary containing vaccine administration data.
+            dict: A dictionary containing vaccine administration data.
         """
         endpoint = f"covid-19/vaccine/coverage/countries?lastdays={last_days}&fullData={str(full_data).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_raps_covid_vaccines_administered_for_country(self, country, last_days=30, full_data=False):
         """
         Returns Get COVID-19 vaccine doses administered for any country that has reported rolling out vaccination. Sourced from https://covid.ourworldindata.org/
         
         Args:
-        - country (str): A valid country name, iso2, iso3.
-        - last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
-        - full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
+            country (str): A valid country name, iso2, iso3.
+            last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
+            full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
         
         Returns:
-        - dict: A dictionary containing vaccine administration data.
+            dict: A dictionary containing vaccine administration data.
         """
         endpoint = f"covid-19/vaccine/coverage/countries/{country}?lastdays={last_days}&fullData={str(full_data).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_raps_covid_vaccines_administered_for_all_states(self, last_days=30, full_data=False):
         """
         Returns Get COVID-19 vaccine doses administered for all states that have reported rolling out vaccination. Sourced from https://covid.ourworldindata.org/
         
         Args:
-        - last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
-        - full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
+            last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
+            full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
         
         Returns:
-        - dict: A dictionary containing vaccine administration data.
+            dict: A dictionary containing vaccine administration data.
         """
         endpoint = f"covid-19/vaccine/coverage/states?lastdays={last_days}&fullData={str(full_data).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_raps_covid_vaccines_administered_for_state(self, state, last_days=30, full_data=False):
         """
         Returns Get COVID-19 vaccine doses administered for any state that has reported rolling out vaccination. Sourced from https://covid.ourworldindata.org/
         
         Args:
-        - country (str): A valid state name
-        - last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
-        - full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
+            country (str): A valid state name
+            last_data (int, str): Number of days to return. Use 'all' for the full data set (e.g. 15, all, 24
+            full_data (bool): Flag indicating whether to return data type as simpleVaccineTimeline (false) or fullVaccineTimeline (true). 
         
         Returns:
-        - dict: A dictionary containing vaccine administration data.
+            dict: A dictionary containing vaccine administration data.
         """
         endpoint = f"covid-19/vaccine/coverage/states/{state}?lastdays={last_days}&fullData={str(full_data).lower()}"
         return mr.make_request(self.base_url+endpoint)
         
     # THERAPEUTICS (from RAPS)
     # This endpoint doesn't seem to be working.
 #    def get_covid_therapeutics_data(self):
 #        """
 #        Returns therapeutics trial data from RAPS (Regulatory Affairs Professional Society). Specifically published by Jeff Craven at https://www.raps.org/news-and-articles/news-articles/2020/3/covid-19-therapeutics-tracker.
 #        
 #        Args:
-#        - None
+#            None
 #        
 #        Returns:
-#        - dict: A dictionary containing therapeutics trial data.
+#            dict: A dictionary containing therapeutics trial data.
 #        """
 #        endpoint = "covid-19/therapeutics"
 #        return mr.make_request(self.base_url+endpoint)
 
     
     # VARIANTS (COVID-19 data from The European Surveillance System -TESSy, provided by [Austria, Belgium, Bulgaria, Croatia, Cyprus, Czechia, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Netherlands, Norway, Poland, Portugal, Romania, Slovakia, Slovenia, Spain and Sweden] https://www.ecdc.europa.eu and released by ECDC updated every week)
     def get_all_countries_ecdc(self):
         """
         Returns a list of supported country names.
         
         Args:
-        - None
+            None
         
         Returns:
-        - list: A list containing supported country names.
+            list: A list containing supported country names.
         """
         endpoint = "covid-19/variants/countries"
         return mr.make_request(self.base_url+endpoint)
         
     def get_ecdc_covid_variant_data_for_country(self, country):
         """
         Returns COVID-19 ECDC reported data for a specific country. 
         
         Args:
-        - country (str): A valid country name from the /v3/covid-19/variants/countries/ endpoint
+            country (str): A valid country name from the /v3/covid-19/variants/countries/ endpoint
         
         Returns:
-        - dict: A dictionary containing covid data.
+            dict: A dictionary containing covid data.
         """
         endpoint = f"covid-19/variants/countries/{country}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/helperFuncs/get_api_list.py` & `nokey-0.7.4/nokey/helperFuncs/get_api_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 def get_api_list():
     """
     Prints out the APIs in a visually pleasing format with headings for the categories 
     and the individual APIs under the respective headings.
 
     Args:
-    - None
+        None
     
     Returns:
-    - string: A list of the apis supported by the nokey package.
+        string: A list of the apis supported by the nokey package.
     """
 
     # ANSI escape codes for colors
     green_color = "\033[92m"  # Green
     blue_color = "\033[94m"   # Blue
     reset_color = "\033[0m"   # Reset color to default
```

### Comparing `nokey-0.7.3/nokey/helperFuncs/make_request.py` & `nokey-0.7.4/nokey/helperFuncs/make_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,79 +31,79 @@
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
 
 
-def make_request_with_params(url, params):
+def make_request_with_params(url, params, headers=None):
     """
     Make a request to an API if the API call requires params.
     
     Args:
-        - url (str): The url of the API.
-        - params (dict): The params to be included in the request.
+        url (str): The url of the API.
+        params (dict): The params to be included in the request.
     
     Returns:
-        - dict: A dictionary containing either the response data or an error message.
+        dict: A dictionary containing either the response data or an error message.
     """
     try:
-        response = requests.get(url, params)
+        response = requests.get(url, params, headers=headers)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
         return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
         
-def make_request_for_content(url):
+def make_request_for_content(url, headers=None):
     """
     Make a request to an API if the API call returns content other than in JSON format.
     
     Args:
-        - url (str): The url of the API.
+        url (str): The url of the API.
     
     Returns:
-        - string: Text in any format containing either the response data or an error message.
+        string: Text in any format containing either the response data or an error message.
     """
     try:
-        response = requests.get(url)
+        response = requests.get(url, headers=headers)
         return response.content
     except HTTPError as http_err:
         # Handle HTTP error
         return {"error": f"HTTP error occurred: {http_err}"}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
         
-def make_request_for_content_with_params(url, params):
+def make_request_for_content_with_params(url, params, headers=None):
     """
     Make a request to an API if the API call returns content other than in JSON format.
     
     Args:
-        - url (str): The url of the API.
+        url (str): The url of the API.
     
     Returns:
-        - string: Text in any format containing either the response data or an error message.
+        string: Text in any format containing either the response data or an error message.
     """
     try:
-        response = requests.get(url, params)
+        response = requests.get(url, params, headers=headers)
         return response.content
     except HTTPError as http_err:
         # Handle HTTP error
         return {"error": f"HTTP error occurred: {http_err}"}
     except Timeout:
         # Handle timeout error
         return {"error": "Request timed out."}
@@ -116,19 +116,19 @@
         
         
 def make_request_with_post_and_data(url, data):
     """
     Make a request to an API if the API using the POST method.
     
     Args:
-        - url (str): The url of the API.
-        - data (dict): The data to be included in the request.
+        url (str): The url of the API.
+        data (dict): The data to be included in the request.
     
     Returns:
-        - dict: A dictionary containing either the response data or an error message.
+        dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.post(url, data=data)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
         return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
@@ -143,19 +143,19 @@
         return {"error": f"An unexpected error occurred: {err}"}
         
 def make_request_with_post_and_json(url, json):
     """
     Make a request to an API if the API using the POST method.
     
     Args:
-        - url (str): The url of the API.
-        - data (dict): The data to be included in the request.
+        url (str): The url of the API.
+        data (dict): The data to be included in the request.
     
     Returns:
-        - dict: A dictionary containing either the response data or an error message.
+        dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.post(url, json=json)
         return response.json()
     except HTTPError as http_err:
         # Handle HTTP error
         return {"error": f"HTTP error occurred: {http_err}", "message": response.json()["message"] if "message" in response.json() else None}
@@ -178,8 +178,8 @@
         params_list (list of tuples): Each tuple contains (original_param_name, new_param_name).
     """
     for original_param_name, new_param_name in params_list:
         if new_param_name is not None:
             params[original_param_name] = new_param_name
         
       
-        
+
```

### Comparing `nokey-0.7.3/nokey/helperFuncs/nokey_apis.py` & `nokey-0.7.4/nokey/helperFuncs/nokey_apis.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.3/nokey/inspiration/dictum.py` & `nokey-0.7.4/nokey/inspiration/dictum.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,151 +2,151 @@
 from .. helperFuncs import make_request as mr
 
 class Dictum:
     """
     A class for interacting with the Dictum API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="dictum_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.fisenko.net/v1/"
         self.about = "Dictum API provides a programmatic way to access the most inspiring expressions of humanity."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Dictum API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        -string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://api.fisenko.net/swagger-ui/"
         
     def get_inspiring_authors(self, language="en", search_query=None, offset=0, limit=0):
         """
         Returns list of authors featured in the API based on the given parameters.
         
         Args:
-        - language (str): The language of the author. Default is en (English). Only other value supported is ru (Russian).
-        - search_query (str): The search query matching the author's name. Default is None.
-        - offset (int): The page offset for the list of authors. Default is 0.
-        - limit (int): The number of items.
+            language (str): The language of the author. Default is en (English). Only other value supported is ru (Russian).
+            search_query (str): The search query matching the author's name. Default is None.
+            offset (int): The page offset for the list of authors. Default is 0.
+            limit (int): The number of items.
         
         Returns:
-        - dict: A dictionary containing the authors matching the given parameters, along with the unique identifier for the author.
+            dict: A dictionary containing the authors matching the given parameters, along with the unique identifier for the author.
         """
         if search_query is not None:
             endpoint = f"authors/{language}?query={search_query}&offset={offset}&limit={limit}"
         else:
             endpoint = f"authors/{language}?&offset={offset}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_inspiring_author_by_id(self, authorID, language="en"):
         """
         Returns the author matching the unique identifier.
         
         Args:
-        - language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
-        - authorID (str): A unique hexadecimal string identifying a specific author in the API.
+            language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
+            authorID (str): A unique hexadecimal string identifying a specific author in the API.
         
         Returns:
-        - dict: A dictionary containing the author matching the given id.
+            dict: A dictionary containing the author matching the given id.
         """
         endpoint = f"authors/{language}/{authorID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_inspiring_quotes_by_author_id(self, authorID, language="en"):
         """
         Returns quotes from an author matching the unique identifier.
         
         Args:
-        - language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
-        - authorID (str): A unique hexadecimal string identifying a specific author in the API.
+            language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
+            authorID (str): A unique hexadecimal string identifying a specific author in the API.
         
         Returns:
-        - dict: A dictionary containing quotes from the author matching the given id.
+            dict: A dictionary containing quotes from the author matching the given id.
         """
         endpoint = f"authors/{language}/{authorID}/quotes"
         return mr.make_request(self.base_url+endpoint)
         
     def get_languages(self):
       """
       Returns a list of author languages used in the API.
       
       Args:
-      - None
+          None
       
       Returns:
-      - dict: A dictionary containing a list of languages (as of this time, only Russian and English)
+          dict: A dictionary containing a list of languages (as of this time, only Russian and English)
       """
       endpoint = "languages"
       return mr.make_request(self.base_url+endpoint)
       
     def get_inspiring_quotes(self, language="en", search_query=None, offset=0, limit=0):
         """
         Returns list of quotes matching the given parameters.
         
         Args:
-        - language (str): The language of the author. Default is en (English). Only other value supported is ru (Russian).
-        - search_query (str): The search query matching the quote. Default is None.
-        - offset (int): The page offset for the list of quotes. Default is 0.
-        - limit (int): The number of items.
+            language (str): The language of the author. Default is en (English). Only other value supported is ru (Russian).
+            search_query (str): The search query matching the quote. Default is None.
+            offset (int): The page offset for the list of quotes. Default is 0.
+            limit (int): The number of items.
         
         Returns:
-        - dict: A dictionary containing the quotes matching the given parameters, along with the unique identifier for the author.
+            dict: A dictionary containing the quotes matching the given parameters, along with the unique identifier for the author.
         """
         if search_query is not None:
             endpoint = f"quotes/{language}?query={search_query}&offset={offset}&limit={limit}"
         else:
             endpoint = f"quotes/{language}?&offset={offset}&limit={limit}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_random_quote(self, language="en"):
         """
         Returns a random quote.
         
         Args:
-        - language (str): Language of the quote. Defaults to en (English). Only other value supported is ru (Russian).
+            language (str): Language of the quote. Defaults to en (English). Only other value supported is ru (Russian).
         
         Returns:
-        - dict: A dictionary containing the random quote.
+            dict: A dictionary containing the random quote.
         """
         endpoint = f"quotes/{language}/random"
         return mr.make_request(self.base_url+endpoint)
         
     def get_inspiring_quote_by_quote_id(self, quoteID, language="en"):
         """
         Returns a quote  matching the unique identifier.
         
         Args:
-        - language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
-        - quoteID (str): A unique hexadecimal string identifying a specific quote in the API.
+            language (str): The language of the author. Defaults to en (English). Only other value supported is ru (Russian).
+            quoteID (str): A unique hexadecimal string identifying a specific quote in the API.
         
         Returns:
-        - dict: A dictionary containing a quote matching the given id.
+            dict: A dictionary containing a quote matching the given id.
         """
         endpoint = f"quotes/{language}/{quoteID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_number_of_quotes_and_authors(self, language="en"):
         """
         Returns the number of quotes and authors in the API for the given language.
         
         Args:
-        - language (str). The language of the quotes. Defaults to en (English). Only other value supported is ru (Russian).
+            language (str). The language of the quotes. Defaults to en (English). Only other value supported is ru (Russian).
         
         Returns:
-        - dict: Dictionary containing the number of authors and quotes for the given language.
+            dict: Dictionary containing the number of authors and quotes for the given language.
         """
         endpoint = f"statistics/{language}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/jokes/joke_api.py` & `nokey-0.7.4/nokey/jokes/joke_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,50 +4,50 @@
 
 @throttle_class(rate_limit=120, period=60)
 class JokeAPI:
     """
     A class to interact with the JokeAPI API.
     
     Attributes:
-    - base_url: Base URL for interacting with the API.
-    - about: A short description of the API.
+        base_url: Base URL for interacting with the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching="False", cache_name="joke_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://v2.jokeapi.dev/joke/"
         self.about = "JokeAPI is a REST API that serves uniformly and well formatted jokes. It can be used without any API token, membership, registration or payment. It supports a variety of filters that can be applied to get just the right jokes you need."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the JokeAPI documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The url for the API documentation.
+            string: The url for the API documentation.
         """
         return "https://sv443.net/jokeapi/v2/"
         
     def get_joke(self, category=None, lang=None, flags=None, joke_type=None, search_string=None, amount=None):
         """
         Returns joke(s) matching the given parameters.
     
         Args:
-        - category (str): Joke category. Defaults to Any. Possible non-default values are Programming, Misc, Dark, Pin, Spooky, and Christmas.
-        - lang (str): Language of the joke. Defaults to en (English). Possible other values are cs (Czech), de (German), es (Spanish), fr (French), and pt (Portuguese).
-        - flags (str): Optional flags to blacklist. Possible values are nsfw, religious, political, racist, sexist, and explicit.
-        - joke_type (str): Optional parameter for either single or twopart joke(s). Defaults to None.
-        - search_string (str): Optional search string contained in desired joke(s). Defaults to None.
-        - amount (int): Number of jokes returned. Defaults to 1.
+            category (str): Joke category. Defaults to Any. Possible non-default values are Programming, Misc, Dark, Pin, Spooky, and Christmas.
+            lang (str): Language of the joke. Defaults to en (English). Possible other values are cs (Czech), de (German), es (Spanish), fr (French), and pt (Portuguese).
+            flags (str): Optional flags to blacklist. Possible values are nsfw, religious, political, racist, sexist, and explicit.
+            joke_type (str): Optional parameter for either single or twopart joke(s). Defaults to None.
+            search_string (str): Optional search string contained in desired joke(s). Defaults to None.
+            amount (int): Number of jokes returned. Defaults to 1.
     
         Returns:
-        - dict: A dictionary containing joke(s) matching given parameters.
+            dict: A dictionary containing joke(s) matching given parameters.
         """
         endpoint = ""
     
         if category is not None:
             endpoint += f"{category}"
         else:
             endpoint += "Any"
```

### Comparing `nokey-0.7.3/nokey/language/free_dictionary.py` & `nokey-0.7.4/nokey/language/free_dictionary.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 from .. helperFuncs import make_request as mr
 
 class FreeDictionary:
     """
     A class to interact with the Free Dictionary API.
     
     Attributes:
-    - base_url: The base URL of the Free Dictionary API.
-    - about: A short description of the API.
+        base_url: The base URL of the Free Dictionary API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="free_dictionary_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.dictionaryapi.dev/api/v2/entries/en/"
         self.about = "The Free Dictionary API is a powerful tool that allows you to access the vast array of dictionary data."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Free Dictionary API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for thre API documentation.
+            string: The URL for thre API documentation.
         """
         return "https://dictionaryapi.dev/"
         
     def look_up_word(self, word):
         """
         Returns the definition and other information of a word.
         
         Args:
-        - word (str): The word to be looked up.
+            word (str): The word to be looked up.
         
         Returns:
-        - dict: A dictionary containing the definition of a word and other related information.
+            dict: A dictionary containing the definition of a word and other related information.
         """
         endpoint = f"{word}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/random/random_user.py` & `nokey-0.7.4/nokey/random/random_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 from .. helperFuncs import make_request as mr
 
 class RandomUserGenerator:
     """
     A class to interact with the Random User Generator API.
     
     Attributes:
-    - base_url: The base url of the API.
-    - about: A short description of the API.
+        base_url: The base url of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="random_user_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://randomuser.me/api/"
         self.about = "The Random User Generator API is a free, open-source API for generating random user data, like Lorem Ipsum for people."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the url for the Random User Generator API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://randomuser.me/"
         
     def generate_random_user(self):
         """
         Returns randomly generated data for a random user.
         
         Args:
-        - None
+            None
         
         Returns:
-        -dict: Dictionary containing random information (such as name, DOB, SSN, address, etc) for a random user.
+            dict: Dictionary containing random information (such as name, DOB, SSN, address, etc) for a random user.
         """
         return mr.make_request(self.base_url)
```

### Comparing `nokey-0.7.3/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.7.4/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 from .. helperFuncs import make_request as mr
 
 class ITIS:
     """ 
     A class for interacting with the Integrated Taxonomic Integration System API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="itis_cache", backend="sqlite", expire_after=3600):
         self.base_url = "http://www.itis.gov/ITISWebService/services/ITISService/"
         self.about = "The ITIS program is driven by a mission: communicate a comprehensive taxonomy of global species that enables biodiversity information to be discovered, indexed, and connected across all human endeavors."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the ITIS API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the API docs.
+            string: The URL for the API docs.
         """
         return "https://www.itis.gov/ws_description.html"
         
     #SEARCH FUNCTIONS
     def search_for_any_match(self, search_key, data_format="json"):
         """
         Returns matches found by comparing the search key to the ITIS common names, scientific names, and TSNs.
         
         Args:
-        - search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchForAnyMatch?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -52,22 +52,22 @@
             return "Error: Format must be either json or xml."
             
     def search_for_any_match_paged(self, search_key, page_size=50, page_num=1, ascend=True, data_format="json"):
         """
         Returns matches found by comparing the search key to the ITIS common names, scientific names, and TSNs.
         
         Args:
-        - search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
-        - page_size (int): Number of matches returned per page. Defaults to 50.
-        - page_num (int): The page number to return (pagination). Defaults to the first page.
-        - ascend (boolean): Whether to sort pages in ascending or descending alphabetical order. Default is True.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
+            page_size (int): Number of matches returned per page. Defaults to 50.
+            page_num (int): The page number to return (pagination). Defaults to the first page.
+            ascend (boolean): Whether to sort pages in ascending or descending alphabetical order. Default is True.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
            
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchForAnyMatchPaged?srchKey={search_key}&pageSize={page_size}&pageNum={page_num}&ascend={ascend}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -76,19 +76,19 @@
             return "Error: Format must be either json or xml."
             
     def get_any_match_count(self, search_key, data_format="json"):
         """
         Returns a count of the matches found by comparing the search key to the ITIS common names, scientific names, and TSNs..
         
         Args:
-        - search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str or int): The name (common or scientific) or Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the count matching the search key.
+            dict or string (xml): A dictionary or XML string containing the count matching the search key.
         """
         endpoint = f"getAnyMatchCount?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -97,19 +97,19 @@
             return "Error: Format must be either json or xml."
             
     def search_by_common_name(self, search_key, data_format="json"):
         """
         Returns matches found by comparing the search key to the ITIS common names.
         
         Args:
-        - search_key (str): The common name.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The common name.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchByCommonName?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -118,19 +118,19 @@
             return "Error: Format must be either json or xml."
             
     def search_by_common_name_begins_with(self, search_key, data_format="json"):
         """
         Return matches found by comparing the search key to the beginning of the ITIS common names.
         
         Args:
-        - search_key (str): The beginning of the name to be searched.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The beginning of the name to be searched.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchByCommonNameBeginsWith?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -139,19 +139,19 @@
             return "Error: Format must be either json or xml."
             
     def search_by_common_name_ends_with(self, search_key, data_format="json"):
         """
         Return matches found by comparing the search key to the end of the ITIS common names.
         
         Args:
-        - search_key (str): The end of the name to be searched.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The end of the name to be searched.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchByCommonNameEndsWith?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -160,19 +160,19 @@
             return "Error: Format must be either json or xml."
             
     def search_by_scientific_name(self, search_key, data_format="json"):
         """
         Returns matches found by comparing the search key to the ITIS scientific names.
         
         Args:
-        - search_key (str): The scientific name.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The scientific name.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"searchByScientificName?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -181,19 +181,19 @@
             return "Error: Format must be either json or xml."
             
     def get_ITIS_terms(self, search_key, data_format="json"):
         """
         Gets a list of ITIS Terms as used by the Resource Catalog Input Tool from a common or scientific name match, or an empty result set if there is no match.
         
         Args:
-        - search_key (str): The common or scientific name.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The common or scientific name.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"getITISTerms?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -202,19 +202,19 @@
             return "Error: Format must be either json or xml."
             
     def get_ITIS_terms_from_common_name(self, search_key, data_format="json"):
         """
         Gets a list of ITIS Terms as used by the Resource Catalog Input Tool from a common name match, or an empty result set if there is no match.
         
         Args:
-        - search_key (str): The common name.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The common name.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"getITISTermsFromCommonName?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -223,19 +223,19 @@
             return "Error: Format must be either json or xml."
             
     def get_ITIS_terms_from_scientific_name(self, search_key, data_format="json"):
         """
         Gets a list of ITIS Terms as used by the Resource Catalog Input Tool from a scientific name match, or an empty result set if there is no match.
         
         Args:
-        - search_key (str): The scientific name.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            search_key (str): The scientific name.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the search key.
+            dict or string (xml): A dictionary or XML string containing the data matching the search key.
         """
         endpoint = f"getITISTermsFromScientificName?srchKey={search_key}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -244,19 +244,19 @@
             return "Error: Format must be either json or xml."
             
     def get_TSNs_by_vernacular_language(self, language, data_format="json"):
         """
         Provide a listing of Taxonomic Serial Numbers (TSNs) with vernaculars entered in the requested language.
         
         Args:
-        - language (str): The desired language. Supported values are Afrikaans, Arabic, Australian, Bengali, Chinese, Djuka, Dutch, eng, English, Fijan, French, Galibi, German, Greek, Hausa, Hawaiian, Hindi, Icelandic, Iglulik Inuit, Italian, Japanese, Javanese, Khmer, Korean, Lao, Malagasy, Manyika, Native American, Ndau, Northern Sotho, Portuguese, Romanian, Shona, Spanish, Swati, unspecified, Xhosa, Zulu.
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            language (str): The desired language. Supported values are Afrikaans, Arabic, Australian, Bengali, Chinese, Djuka, Dutch, eng, English, Fijan, French, Galibi, German, Greek, Hausa, Hawaiian, Hindi, Icelandic, Iglulik Inuit, Italian, Japanese, Javanese, Khmer, Korean, Lao, Malagasy, Manyika, Native American, Ndau, Northern Sotho, Portuguese, Romanian, Shona, Spanish, Swati, unspecified, Xhosa, Zulu.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the language.
+            dict or string (xml): A dictionary or XML string containing the data matching the language.
         """
         endpoint = f"getTsnByVernacularLanguage?language={language}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -267,19 +267,19 @@
          
     #FUNCTIONS TO RETRIEVE INFORMATION BY TSN
     def get_accepted_names_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of accepted names for the TSN. This can return more than one result if the TSN is for a synonym.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getAcceptedNamesFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -288,19 +288,19 @@
             return "Error: Format must be either json or xml."
             
     def get_comment_detail_from_TSN(self, tsn, data_format="json"):
         """
         Returns the list of comments for the TSN. This can return more than result if multiple comments are entered.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCommentDetailFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -309,19 +309,19 @@
             return "Error: Format must be either json or xml."
             
     def get_common_names_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of common names for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCommonNamesFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -330,19 +330,19 @@
             return "Error: Format must be either json or xml."
             
     def get_core_metadata_from_TSN(self, tsn, data_format="json"):
         """
         Returns the set of core metadata for the TSN. This contains credibility rating, taxonomic usage, unacceptability reason, coverage, and currency data.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCoreMetadataFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -351,19 +351,19 @@
             return "Error: Format must be either json or xml."
             
     def get_coverage_from_TSN(self, tsn, data_format="json"):
         """
         Returns the taxon coverage information for the TSN. This information is  available for Genus and above (rank_id > 190) only.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCoverageFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -372,19 +372,19 @@
             return "Error: Format must be either json or xml."
             
     def get_credibility_rating_from_TSN(self, tsn, data_format="json"):
         """
         Returns the credibility rating for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCredibilityRatingFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -393,19 +393,19 @@
             return "Error: Format must be either json or xml."
             
     def get_currency_from_TSN(self, tsn, data_format="json"):
         """
         Returns the taxon currency information for the TSN. This information is  available for Genus and above (rank_id > 190) only.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getCurrencyFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -414,19 +414,19 @@
             return "Error: Format must be either json or xml."
             
     def get_date_data_from_TSN(self, tsn, data_format="json"):
         """
         Returns the initial time stamp and last update date for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getDateDataFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -435,19 +435,19 @@
             return "Error: Format must be either json or xml."
             
     def get_experts_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the expert information for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getExpertsFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -456,19 +456,19 @@
             return "Error: Format must be either json or xml."
             
     def get_full_record_from_TSN(self, tsn, data_format="json"):
         """
         Returns the full ITIS record for a TSN found by comparing the search key to the TSN field, or an empty result set if there is no match.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getFullRecordFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -477,19 +477,19 @@
             return "Error: Format must be either json or xml."
             
     def get_geographic_divisions_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the geographic divisions for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getGeographicDivisionsFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -498,19 +498,19 @@
             return "Error: Format must be either json or xml."
             
     def get_global_species_completeness_from_TSN(self, tsn, data_format="json"):
         """
         Returns the taxon completenes rating for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getGlobalSpeciesCompletenessFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -519,19 +519,19 @@
             return "Error: Format must be either json or xml."
             
     def get_jurisdictional_origin_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the jurisdiction and origin values for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getJurisdictionalOriginFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -540,19 +540,19 @@
             return "Error: Format must be either json or xml."
             
     def get_kingdom_name_from_TSN(self, tsn, data_format="json"):
         """
         Returns the kingdom name for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getKingdomNameFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -561,19 +561,19 @@
             return "Error: Format must be either json or xml."
             
     def get_other_sources_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the other sources used for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getOtherSourcesFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -582,19 +582,19 @@
             return "Error: Format must be either json or xml."
             
     def get_parent_TSN_from_TSN(self, tsn, data_format="json"):
         """
         Returns the parent TSN for the entered TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getParentTSNFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -603,19 +603,19 @@
             return "Error: Format must be either json or xml."
             
     def get_publications_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the pulications used for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getPublicationsFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -624,19 +624,19 @@
             return "Error: Format must be either json or xml."
             
     def get_review_year_from_TSN(self, tsn, data_format="json"):
         """
         Returns the review year for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getReviewYearFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -645,19 +645,19 @@
             return "Error: Format must be either json or xml."
             
     def get_scientific_name_from_TSN(self, tsn, data_format="json"):
         """
         Returns the scientific name for the TSN. Also returns the component parts (names and indicators) of the scientific name.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getScientificNameFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -666,19 +666,19 @@
             return "Error: Format must be either json or xml."
             
     def get_synonym_names_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of the synonyms (if any) for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getSynonymNamesFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -687,19 +687,19 @@
             return "Error: Format must be either json or xml."
             
     def get_taxon_authorship_from_TSN(self, tsn, data_format="json"):
         """
         Returns the author information for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getTaxonAuthorshipFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -708,19 +708,19 @@
             return "Error: Format must be either json or xml."
             
     def get_taxonomic_rank_name_from_TSN(self, tsn, data_format="json"):
         """
         Returns the kingdom and rank information for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getTaxonomicRankNameFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -729,19 +729,19 @@
             return "Error: Format must be either json or xml."
             
     def get_taxonomic_usage_from_TSN(self, tsn, data_format="json"):
         """
         Returns the usage information for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getTaxonomicUsageFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -750,19 +750,19 @@
             return "Error: Format must be either json or xml."
             
     def get_unacceptability_reason_from_TSN(self, tsn, data_format="json"):
         """
         Returns the unacceptability reason, if any, for the TSN.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getUnacceptabilityReasonFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -773,19 +773,19 @@
             
     # HIERARCHY FUNCTIONS
     def get_full_hierarchy_from_TSN(self, tsn, data_format="json"):
         """
         Returns the Taxonomic Hierarchy from the kingdom to the requested scientific name, and the immediate children of the scientific name.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getFullHierarchyFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -794,19 +794,19 @@
             return "Error: Format must be either json or xml."
             
     def get_hierarchy_down_from_TSN(self, tsn, data_format="json"):
         """
         Returns a list of all the valid/accepted scientific names contained within a particular valid/accepted scientific name and their TSNs, limited to immediate children only. The result set will be found by comparing the search key to the parent TSN field.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getHierarchyDownFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -815,19 +815,19 @@
             return "Error: Format must be either json or xml."
             
     def get_hierarchy_up_from_TSN(self, tsn, data_format="json"):
         """
         Returns the parent of the TSN (i.e. the parent of the current scientific name in the taxonomic hierarchy) found by comparing the search key to the ITIS TSN field.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getHierarchyUpFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -838,19 +838,19 @@
             
     # LIFE SCIENCE IDENTIFIER (LSID) FUNCTIONS
     def get_full_record_from_LSID(self, tsn, data_format="json"):
         """
         Returns the full ITIS record for the TSN in the LSID, found by comparing the TSN in the search key to the TSN field. Returns an empty result set if there is no match or the TSN is invalid.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getFullRecordFromLSID?lsid=urn:lsid:itis.gov:itis_tsn:{tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -859,19 +859,19 @@
             return "Error: Format must be either json or xml."
             
     def get_LSID_from_TSN(self, tsn, data_format="json"):
         """
         Gets the unique LSID for the TSN, or an empty result if there is no match.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getLSIDFromTSN?tsn={tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -880,19 +880,19 @@
             return "Error: Format must be either json or xml."
             
     def get_record_from_LSID(self, tsn, data_format="json"):
         """
         Gets the partial ITIS record for the TSN in the LSID, found by comparing the TSN in the search key to the TSN field. Returns an empty result set if there is no match or the TSN is invalid.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getRecordFromLSID?lsid=urn:lsid:itis.gov:itis_tsn:{tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -901,19 +901,19 @@
             return "Error: Format must be either json or xml."
             
     def get_TSN_from_LSID(self, tsn, data_format="json"):
         """
         Gets the TSN corresponding to the LSID, or an empty result if there is no match.
         
         Args:
-        - tsn (int): The Taxonomic Serial Number (TSN).
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            tsn (int): The Taxonomic Serial Number (TSN).
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the data matching the TSN.
+            dict or string (xml): A dictionary or XML string containing the data matching the TSN.
         """
         endpoint = f"getTSNFromLSID?lsid=urn:lsid:itis.gov:itis_tsn:{tsn}"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -924,18 +924,18 @@
             
     # META-INFORMATION FUNCTIONS
     def get_credibility_ratings(self, data_format="json"):
         """
         Provides a list of all the unique valid credibility rating values contained in the database.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the credibility rating values.
+            dict or string (xml): A dictionary or XML string containing the credibility rating values.
         """
         endpoint = "getCredibilityRatings"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -944,18 +944,18 @@
             return "Error: Format must be either json or xml."
             
     def get_description(self, data_format="json"):
         """
         Provides a description of the web service and the ITIS database.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing a description of the ITIS database.
+            dict or string (xml): A dictionary or XML string containing a description of the ITIS database.
         """
         endpoint = "getDescription"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -964,18 +964,18 @@
             return "Error: Format must be either json or xml."
             
     def get_geographic_values(self, data_format="json"):
         """
         Provides a list of all the geographic values contained in the database.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the geographic values contained in the database.
+            dict or string (xml): A dictionary or XML string containing the geographic values contained in the database.
         """
         endpoint = "getGeographicValues"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -984,18 +984,18 @@
             return "Error: Format must be either json or xml."
             
     def get_jurisdiction_values(self, data_format="json"):
         """
         Provides a list of all the jurisdiction values contained in the database.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the jurisdiction values contained in the database.
+            dict or string (xml): A dictionary or XML string containing the jurisdiction values contained in the database.
         """
         endpoint = "getJurisdictionValues"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -1004,18 +1004,18 @@
             return "Error: Format must be either json or xml."
             
     def get_jurisdictional_origin_values(self, data_format="json"):
         """
         Provides a list of all the origin values contained in the database.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the origin values contained in the database.
+            dict or string (xml): A dictionary or XML string containing the origin values contained in the database.
         """
         endpoint = "getJurisdictionalOriginValues"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -1024,18 +1024,18 @@
             return "Error: Format must be either json or xml."
             
     def get_kingdom_names(self, data_format="json"):
         """
         Provides a list of all the unique kingdom names contained in the database, their kingdom IDs and their TSNs.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the kingdom names contained in the database.
+            dict or string (xml): A dictionary or XML string containing the kingdom names contained in the database.
         """
         endpoint = "getKingdomNames"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -1044,18 +1044,18 @@
             return "Error: Format must be either json or xml."
             
     def get_last_change_date(self, data_format="json"):
         """
         Provides the date the ITIS database was last updated.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing the date the database was last updated.
+            dict or string (xml): A dictionary or XML string containing the date the database was last updated.
         """
         endpoint = "getLastChangeDate"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -1064,18 +1064,18 @@
             return "Error: Format must be either json or xml."
             
     def get_rank_names(self, data_format="json"):
         """
         Provides a list of all the unique rank names contained in the database and their kingdom and rank ID values.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing a list of all the unique rank names contained in the database.
+            dict or string (xml): A dictionary or XML string containing a list of all the unique rank names contained in the database.
         """
         endpoint = "getRankNames"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
@@ -1084,18 +1084,18 @@
             return "Error: Format must be either json or xml."
             
     def get_vernacular_languages(self, data_format="json"):
         """
         Provides a list of the unique languages used in the vernacular table.
         
         Args:
-        - data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
+            data_format (str): The desired format for returned data. Defaults to json, but other option is xml.
         
         Returns:
-        - dict or string (xml): A dictionary or XML string containing a list of all the unique languages used in the vernacular table.
+            dict or string (xml): A dictionary or XML string containing a list of all the unique languages used in the vernacular table.
         """
         endpoint = "getVernacularLanguages"
         data_format = data_format.lower()
         if data_format == "json":
             data = mr.make_request_for_content(self.base_url+endpoint)
             return xmltodict.parse(data)
         elif data_format == "xml":
```

### Comparing `nokey-0.7.3/nokey/science_and_nature/nobel_prize.py` & `nokey-0.7.4/nokey/science_and_nature/nobel_prize.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,85 +2,85 @@
 from .. helperFuncs import make_request as mr
 
 class NobelPrizeAPI:
     """
     A class to interact with the Nobel Prize API.
     
     Attributes:
-    - base_url: The base url for the Nobel Prize API.
-    - about: A short description of the API.
+        base_url: The base url for the Nobel Prize API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="nobel_prize_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.nobelprize.org/2.1/"
         self.about = "The Nobel Prize API returns all information about Laureates and Nobel Prizes."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Nobel Prize API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: The URL for the Nobel Prize API docs.
+            string: The URL for the Nobel Prize API docs.
         """
         return "https://www.nobelprize.org/about/developer-zone-2/"
         
     def get_nobel_prize_laureates(self):
         """
         Returns a list of Nobel Prize laureates with information about the winners.
         
         Args:
-        - None
+            None
         
         Returns
-        - dict: A dictionary containing a list of Nobel Prize laureates and relevant information about the winners.
+            dict: A dictionary containing a list of Nobel Prize laureates and relevant information about the winners.
         """
         endpoint = "laureates"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_nobel_prizes(self):
         """
         Returns a list of all the Nobel Prizes award along with information about the specific prize and winners.
         
         Args:
-        - None
+            None
         
         Returns
-        - dict: A dictionary containing a list of Nobel Prizes awarded and relevant information about the prize.
+            dict: A dictionary containing a list of Nobel Prizes awarded and relevant information about the prize.
         """
         endpoint = "nobelPrizes"
         return mr.make_request(self.base_url+endpoint)
         
     def get_one_nobel_prize(self, category, year):
         """
         Returns a specific Nobel Prize and information about the specific prize and winners.
         
         Args:
-        - category (str): The category of the prize awarded. Possible values are che (chemistry), eco (economic sciences), lit (literature), pea (peace), phy (physics), and med (medicine). Any other strings passed for category will return all the pieces for specified year.
-        - year (int): The year the prize was awarded.
+            category (str): The category of the prize awarded. Possible values are che (chemistry), eco (economic sciences), lit (literature), pea (peace), phy (physics), and med (medicine). Any other strings passed for category will return all the pieces for specified year.
+            year (int): The year the prize was awarded.
         
         Returns
-        - dict: A dictionary containing a specific Nobel Prize awarded and relevant information about the prize.
+            dict: A dictionary containing a specific Nobel Prize awarded and relevant information about the prize.
         """
         endpoint = f"nobelPrize/{category.lower()}/{year}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_nobel_laureate_by_id(self, laureateID):
         """
         Returns a specific Nobel Prize and information about the specific prize and winners.
         
         Args:
-        - laureateID (int): A unique identifier for a specific Nobel laureate.
+            laureateID (int): A unique identifier for a specific Nobel laureate.
         
         Returns
-        - dict: A dictionary containing a specific Nobel Prize awarded and relevant information about the prize.
+            dict: A dictionary containing a specific Nobel Prize awarded and relevant information about the prize.
         """
         endpoint = f"laureate/{laureateID}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/spaceflight/spaceflight_news.py` & `nokey-0.7.4/nokey/spaceflight/spaceflight_news.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 
 class SpaceflightNews:
     
     """
     A class to interact with the Spaceflight News API.
     
     Attributes:
-    - base_url: The base URL of the Spaceflight News API.
-    - about: A short description of the API.
+        base_url: The base URL of the Spaceflight News API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="spaceflight_news_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.spaceflightnewsapi.net/v4/"
         self.about = "The Spaceflight News API (SNAPI) is a product by The Space Devs (TSD). It's the most complete and up-to-date spaceflight news API currently available."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the url for the Spaceflight News API documentation.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://api.spaceflightnewsapi.net/v4/docs"
         
     def get_articles(self, limit=10, offset=10, search=None, summary_contains=None, title_contains=None):
         """
         Returns a list of spaceflight articles fitting the given parameters.
         
         Args:
-        - limit (int): Number of results to return per page. Defaults to 10.
-        - offset (int): The initial index from which to return the results. Defaults to 10.
-        - search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
-        - summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
-        - title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
+            limit (int): Number of results to return per page. Defaults to 10.
+            offset (int): The initial index from which to return the results. Defaults to 10.
+            search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
+            summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
+            title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
         
         Returns:
-        - dict: List of spaceflight articles matching the given parameters.
+            dict: List of spaceflight articles matching the given parameters.
         """
         if search is not None and summary_contains is not None and title_contains is not None:
             endpoint = f"articles?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}&title_contains={title_contains}"
         elif search is not None and summary_contains is not None:
             endpoint = f"articles?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}"
         elif search is not None and title_contains is not None:
             endpoint = f"articles?limit={limit}&offset={offset}&search={search}&title_contains={title_contains}"
@@ -63,35 +63,35 @@
         return mr.make_request(self.base_url + endpoint)
         
     def get_article_by_id(self, ID):
         """
         Returns a specific article.
         
         Args:
-        - ID (int): A unique integer value identifying this article.
+            ID (int): A unique integer value identifying this article.
         
         Returns:
-        - dict: A dictionary containing the article.
+            dict: A dictionary containing the article.
         """
         endpoint = f"articles/{ID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_blogs(self, limit=10, offset=10, search=None, summary_contains=None, title_contains=None):
         """
         Returns a list of spaceflight blogs fitting the given parameters.
         
         Args:
-        - limit (int): Number of results to return per page. Defaults to 10.
-        - offset (int): The initial index from which to return the results. Defaults to 10.
-        - search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
-        - summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
-        - title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
+            limit (int): Number of results to return per page. Defaults to 10.
+            offset (int): The initial index from which to return the results. Defaults to 10.
+            search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
+            summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
+            title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
         
         Returns:
-        - dict: List of spaceflight blogs matching the given parameters.
+            dict: List of spaceflight blogs matching the given parameters.
         """
         if search is not None and summary_contains is not None and title_contains is not None:
             endpoint = f"blogs?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}&title_contains={title_contains}"
         elif search is not None and summary_contains is not None:
             endpoint = f"blogs?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}"
         elif search is not None and title_contains is not None:
             endpoint = f"blogs?limit={limit}&offset={offset}&search={search}&title_contains={title_contains}"
@@ -109,48 +109,48 @@
         return mr.make_request(self.base_url + endpoint)
         
     def get_blog_by_id(self, ID):
         """
         Returns a specific blog.
         
         Args:
-        - ID (int): A unique integer value identifying this blog.
+            ID (int): A unique integer value identifying this blog.
         
         Returns:
-        - dict: A dictionary containing the blog.
+            dict: A dictionary containing the blog.
         """
         endpoint = f"blogs/{ID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_info(self):
         """
         Returns information containing API version and news sites featured.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the version number and a list of features news sites.
+            dict: A dictionary containing the version number and a list of features news sites.
         """
         endpoint = "info"
         return mr.make_request(self.base_url+endpoint)
         
     def get_reports(self, limit=10, offset=10, search=None, summary_contains=None, title_contains=None):
         """
         Returns a list of spaceflight reports fitting the given parameters.
         
         Args:
-        - limit (int): Number of results to return per page. Defaults to 10.
-        - offset (int): The initial index from which to return the results. Defaults to 10.
-        - search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
-        - summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
-        - title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
+            limit (int): Number of results to return per page. Defaults to 10.
+            offset (int): The initial index from which to return the results. Defaults to 10.
+            search (str): Search for documents with a specific phrase in the title or summary. Defaults to None.
+            summary_contains (str): Search for all documents with a specific phrase in the summary. Defaults to None.
+            title_contains (str): Search for all documents with a specific phrase in the title. Defaults to None.
         
         Returns:
-        - dict: List of spaceflight reports matching the given parameters.
+            dict: List of spaceflight reports matching the given parameters.
         """
         if search is not None and summary_contains is not None and title_contains is not None:
             endpoint = f"reports?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}&title_contains={title_contains}"
         elif search is not None and summary_contains is not None:
             endpoint = f"reports?limit={limit}&offset={offset}&search={search}&summary_contains={summary_contains}"
         elif search is not None and title_contains is not None:
             endpoint = f"reports?limit={limit}&offset={offset}&search={search}&title_contains={title_contains}"
@@ -168,18 +168,18 @@
         return mr.make_request(self.base_url + endpoint)
         
     def get_report_by_id(self, ID):
         """
         Returns a specific report.
         
         Args:
-        - ID (int): A unique integer value identifying this report.
+            ID (int): A unique integer value identifying this report.
         
         Returns:
-        - dict: A dictionary containing the report.
+            dict: A dictionary containing the report.
         """
         endpoint = f"reports/{ID}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/tv_and_film/star_trek_api.py` & `nokey-0.7.4/nokey/tv_and_film/star_trek_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,1125 +2,1125 @@
 from .. helperFuncs import make_request as mr
 
 class STAPI:
     """
     A class for interacting with the Star Trek API.
     
     Attributes:
-    - base_url: The base URL of the API.
-    - about: A short description of the API.
+        base_url: The base URL of the API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="stapi_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://stapi.co/api/"
         self.about = "STAPI (Star Trek API) is an API for accessing information about all things Star Trek."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns the URL for the Star Trek API.
         
         Args:
-        - None
+            None
         
         Returns:
-        - str: The URL for the API.
+            str: The URL for the API.
         """
         return "https://editor.swagger.io/?url=https://stapi.co/api/v1/rest/common/download/stapi.yaml"
         
     def get_animal_by_id(self, uid):
         """
         Returns information about a Star Trek animal matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the animal.
+            uid (str): The unique identifier for the animal.
         
         Returns:
-        - dict: A dictionary containing information about the animal.
+            dict: A dictionary containing information about the animal.
         """
         endpoint = f"v1/rest/animal?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_animals(self, pageNumber=0, pageSize=50):
         """
         Returns a list of animals of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of animals per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of animals per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of animals.
+            dict: A dictionary containing a list of animals.
         """
         endpoint = f"v1/rest/animal/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_astronomical_object_by_id(self, uid):
         """
         Returns information about a Star Trek astronomical object matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the astronomical object.
+            uid (str): The unique identifier for the astronomical object.
         
         Returns:
-        - dict: A dictionary containing information about the astronomical object.
+            dict: A dictionary containing information about the astronomical object.
         """
         endpoint = f"v2/rest/astronomicalObject?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_astronomical_objects(self, pageNumber=0, pageSize=50):
         """
         Returns a list of astronomical objects of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of objects per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of objects per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of astronomical objects.
+            dict: A dictionary containing a list of astronomical objects.
         """
         endpoint = f"v2/rest/astronomicalObject/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_by_id(self, uid):
         """
         Returns information about a Star Trek book matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the book.
+            uid (str): The unique identifier for the book.
         
         Returns:
-        - dict: A dictionary containing information about the book.
+            dict: A dictionary containing information about the book.
         """
         endpoint = f"v2/rest/book?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_books(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek books of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of books per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of books per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of books.
+            dict: A dictionary containing a list of books.
         """
         endpoint = f"v2/rest/book/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_collection_by_id(self, uid):
         """
         Returns information about a Star Trek book collection matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the book collection.
+            uid (str): The unique identifier for the book collection.
         
         Returns:
-        - dict: A dictionary containing information about the book collection.
+            dict: A dictionary containing information about the book collection.
         """
         endpoint = f"v1/rest/bookCollection?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_collections(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek book collections of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of book collections per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of book collections per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of book collections.
+            dict: A dictionary containing a list of book collections.
         """
         endpoint = f"v1/rest/bookCollection/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_series_by_id(self, uid):
         """
         Returns information about a Star Trek book series matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the book series.
+            uid (str): The unique identifier for the book series.
         
         Returns:
-        - dict: A dictionary containing information about the book series.
+            dict: A dictionary containing information about the book series.
         """
         endpoint = f"v1/rest/bookSeries?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_book_series(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek book series of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of book series per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of book series per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of book series.
+            dict: A dictionary containing a list of book series.
         """
         endpoint = f"v1/rest/bookSeries/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_character_by_id(self, uid):
         """
         Returns information about a Star Trek character matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the character.
+            uid (str): The unique identifier for the character.
         
         Returns:
-        - dict: A dictionary containing information about the character.
+            dict: A dictionary containing information about the character.
         """
         endpoint = f"v1/rest/character?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_characters(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek characters of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of characters per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of characters per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of characters.
+            dict: A dictionary containing a list of characters.
         """
         endpoint = f"v1/rest/character/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_by_id(self, uid):
         """
         Returns information about a Star Trek comic matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the comic.
+            uid (str): The unique identifier for the comic.
         
         Returns:
-        - dict: A dictionary containing information about the comic.
+            dict: A dictionary containing information about the comic.
         """
         endpoint = f"v1/rest/comics?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comics(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek comics of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of comics per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of comics per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of comics.
+            dict: A dictionary containing a list of comics.
         """
         endpoint = f"v1/rest/comics/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_collection_by_id(self, uid):
         """
         Returns information about a Star Trek comic collection matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the comic collection.
+            uid (str): The unique identifier for the comic collection.
         
         Returns:
-        - dict: A dictionary containing information about the comic collection.
+            dict: A dictionary containing information about the comic collection.
         """
         endpoint = f"v1/rest/comicCollection?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_collections(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek comic collections of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of comic collections per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of comic collections per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of comic collections.
+            dict: A dictionary containing a list of comic collections.
         """
         endpoint = f"v1/rest/comicCollection/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_series_by_id(self, uid):
         """
         Returns information about a Star Trek comic series matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the comic series.
+            uid (str): The unique identifier for the comic series.
         
         Returns:
-        - dict: A dictionary containing information about the comic series.
+            dict: A dictionary containing information about the comic series.
         """
         endpoint = f"v1/rest/comicSeries?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_series(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek comic series of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of comic series per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of comic series per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of comic series.
+            dict: A dictionary containing a list of comic series.
         """
         endpoint = f"v1/rest/comicSeries/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_strip_by_id(self, uid):
         """
         Returns information about a Star Trek comic strip matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the comic strip.
+            uid (str): The unique identifier for the comic strip.
         
         Returns:
-        - dict: A dictionary containing information about the comic strip.
+            dict: A dictionary containing information about the comic strip.
         """
         endpoint = f"v1/rest/comicStrip?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_comic_strips(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek comic strips of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of comic strips per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of comic strips per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of comic strips.
+            dict: A dictionary containing a list of comic strips.
         """
         endpoint = f"v1/rest/comicStrip/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_company_by_id(self, uid):
         """
         Returns information about a Star Trek company matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the company.
+            uid (str): The unique identifier for the company.
         
         Returns:
-        - dict: A dictionary containing information about the company.
+            dict: A dictionary containing information about the company.
         """
         endpoint = f"v2/rest/company?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_companies(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek companies of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of companies per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of companies per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of companies.
+            dict: A dictionary containing a list of companies.
         """
         endpoint = f"v2/rest/company/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_conflict_by_id(self, uid):
         """
         Returns information about a Star Trek conflict matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the conflict.
+            uid (str): The unique identifier for the conflict.
         
         Returns:
-        - dict: A dictionary containing information about the conflict.
+            dict: A dictionary containing information about the conflict.
         """
         endpoint = f"v2/rest/conflict?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_conflicts(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek conflicts of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of conflicts per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of conflicts per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of conflicts.
+            dict: A dictionary containing a list of conflicts.
         """
         endpoint = f"v1/rest/conflict/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_data_version(self):
         """
         Returns the data version of the API.
         
         Args:
-        - None
+            None
         
         Returns:
-        - dict: A dictionary containing the data version of the API.
+            dict: A dictionary containing the data version of the API.
         """
         endpoint = "v1/rest/common/dataVersion"
         return mr.make_request(self.base_url+endpoint)
         
     def get_element_by_id(self, uid):
         """
         Returns information about a Star Trek element matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the element.
+            uid (str): The unique identifier for the element.
         
         Returns:
-        - dict: A dictionary containing information about the element.
+            dict: A dictionary containing information about the element.
         """
         endpoint = f"v2/rest/element?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_elements(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek elements of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of elements per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of elements per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of elements.
+            dict: A dictionary containing a list of elements.
         """
         endpoint = f"v2/rest/element/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_episode_by_id(self, uid):
         """
         Returns information about a Star Trek episode matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the episode.
+            uid (str): The unique identifier for the episode.
         
         Returns:
-        - dict: A dictionary containing information about the episode.
+            dict: A dictionary containing information about the episode.
         """
         endpoint = f"v1/rest/episode?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_episodes(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek episodes of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of eposodes per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of eposodes per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of episodes.
+            dict: A dictionary containing a list of episodes.
         """
         endpoint = f"v1/rest/episode/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_food_by_id(self, uid):
         """
         Returns information about a Star Trek food matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the food.
+            uid (str): The unique identifier for the food.
         
         Returns:
-        - dict: A dictionary containing information about the food.
+            dict: A dictionary containing information about the food.
         """
         endpoint = f"v1/rest/food?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_foods(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek foods of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of foods per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of foods per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of foods.
+            dict: A dictionary containing a list of foods.
         """
         endpoint = f"v1/rest/food/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_literature_by_id(self, uid):
         """
         Returns information about Star Trek literature matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the literature.
+            uid (str): The unique identifier for the literature.
         
         Returns:
-        - dict: A dictionary containing information about the literature.
+            dict: A dictionary containing information about the literature.
         """
         endpoint = f"v1/rest/literature?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_literature(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek literature of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of literature per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of literature per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of literature.
+            dict: A dictionary containing a list of literature.
         """
         endpoint = f"v1/rest/literature/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_location_by_id(self, uid):
         """
         Returns information about a Star Trek location matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the location.
+            uid (str): The unique identifier for the location.
         
         Returns:
-        - dict: A dictionary containing information about the location.
+            dict: A dictionary containing information about the location.
         """
         endpoint = f"v2/rest/location?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_locations(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek locations of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of locations per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of locations per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of locations.
+            dict: A dictionary containing a list of locations.
         """
         endpoint = f"v2/rest/location/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_magazine_by_id(self, uid):
         """
         Returns information about a Star Trek magazine matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the magazine.
+            uid (str): The unique identifier for the magazine.
         
         Returns:
-        - dict: A dictionary containing information about the magazine.
+            dict: A dictionary containing information about the magazine.
         """
         endpoint = f"v1/rest/magazine?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_magazines(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek magazines of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of magazines per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of magazines per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of magazines.
+            dict: A dictionary containing a list of magazines.
         """
         endpoint = f"v1/rest/magazine/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_magazine_series_by_id(self, uid):
         """
         Returns information about a Star Trek magazine series matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the magazine series.
+            uid (str): The unique identifier for the magazine series.
         
         Returns:
-        - dict: A dictionary containing information about the magazine series.
+            dict: A dictionary containing information about the magazine series.
         """
         endpoint = f"v1/rest/magazineSeries?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_magazine_series(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek magazine series of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of magazine series per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of magazine series per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of magazine series.
+            dict: A dictionary containing a list of magazine series.
         """
         endpoint = f"v1/rest/magazineSeries/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_material_by_id(self, uid):
         """
         Returns information about a Star Trek material matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the material.
+            uid (str): The unique identifier for the material.
         
         Returns:
-        - dict: A dictionary containing information about the material.
+            dict: A dictionary containing information about the material.
         """
         endpoint = f"v1/rest/material?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_materials(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek materials of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of materials per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of materials per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of materials.
+            dict: A dictionary containing a list of materials.
         """
         endpoint = f"v1/rest/material/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_medical_condition_by_id(self, uid):
         """
         Returns information about a Star Trek medical condition matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the medical condition.
+            uid (str): The unique identifier for the medical condition.
         
         Returns:
-        - dict: A dictionary containing information about the medical condition.
+            dict: A dictionary containing information about the medical condition.
         """
         endpoint = f"v1/rest/medicalCondition?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_medical_conditions(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek medical conditions of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of medical conditions per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of medical conditions per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of medical conditions.
+            dict: A dictionary containing a list of medical conditions.
         """
         endpoint = f"v1/rest/medicalCondition/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_movie_by_id(self, uid):
         """
         Returns information about a Star Trek movie matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the movie.
+            uid (str): The unique identifier for the movie.
         
         Returns:
-        - dict: A dictionary containing information about the movie.
+            dict: A dictionary containing information about the movie.
         """
         endpoint = f"v1/rest/movie?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_movies(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek movies of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of movies per page. Defaults to 50 (although at this time there are only 14 entries).
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of movies per page. Defaults to 50 (although at this time there are only 14 entries).
         
         Returns:
-        - dict: A dictionary containing a list of movies.
+            dict: A dictionary containing a list of movies.
         """
         endpoint = f"v1/rest/movie/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_occupation_by_id(self, uid):
         """
         Returns information about a Star Trek occupation matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the occupation.
+            uid (str): The unique identifier for the occupation.
         
         Returns:
-        - dict: A dictionary containing information about the occupation.
+            dict: A dictionary containing information about the occupation.
         """
         endpoint = f"v2/rest/occupation?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_occupations(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek occupations of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of occupations per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of occupations per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of occupations.
+            dict: A dictionary containing a list of occupations.
         """
         endpoint = f"v2/rest/occupation/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_organization_by_id(self, uid):
         """
         Returns information about a Star Trek organization matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the organization.
+            uid (str): The unique identifier for the organization.
         
         Returns:
-        - dict: A dictionary containing information about the organization.
+            dict: A dictionary containing information about the organization.
         """
         endpoint = f"v1/rest/organization?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_organizations(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek organizations of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of organizations per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of organizations per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of organizations.
+            dict: A dictionary containing a list of organizations.
         """
         endpoint = f"v1/rest/organization/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_performer_by_id(self, uid):
         """
         Returns information about a Star Trek performer matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the performer.
+            uid (str): The unique identifier for the performer.
         
         Returns:
-        - dict: A dictionary containing information about the performer.
+            dict: A dictionary containing information about the performer.
         """
         endpoint = f"v2/rest/performer?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_performers(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek performers of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of performers per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of performers per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of performers.
+            dict: A dictionary containing a list of performers.
         """
         endpoint = f"v2/rest/performer/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_season_by_id(self, uid):
         """
         Returns information about a Star Trek season matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the season.
+            uid (str): The unique identifier for the season.
         
         Returns:
-        - dict: A dictionary containing information about the season.
+            dict: A dictionary containing information about the season.
         """
         endpoint = f"v1/rest/season?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_seasons(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek seasons of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of seasons per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of seasons per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of seasons.
+            dict: A dictionary containing a list of seasons.
         """
         endpoint = f"v1/rest/season/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_series_by_id(self, uid):
         """
         Returns information about a Star Trek series matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the series.
+            uid (str): The unique identifier for the series.
         
         Returns:
-        - dict: A dictionary containing information about the series.
+            dict: A dictionary containing information about the series.
         """
         endpoint = f"v1/rest/series?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_series(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek series of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of series per page. Defaults to 50 (although at this time there are only 12 entries).
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of series per page. Defaults to 50 (although at this time there are only 12 entries).
         
         Returns:
-        - dict: A dictionary containing a list of series.
+            dict: A dictionary containing a list of series.
         """
         endpoint = f"v1/rest/series/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_soundtrack_by_id(self, uid):
         """
         Returns information about a Star Trek soundtrack.matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the soundtrack.
+            uid (str): The unique identifier for the soundtrack.
         
         Returns:
-        - dict: A dictionary containing information about the soundtrack.
+            dict: A dictionary containing information about the soundtrack.
         """
         endpoint = f"v1/rest/soundtrack?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_soundtracks(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek soundtracks of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of soundtracks per page. Defaults to 50 (although at this time there are only 12 entries).
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of soundtracks per page. Defaults to 50 (although at this time there are only 12 entries).
         
         Returns:
-        - dict: A dictionary containing a list of soundtracks.
+            dict: A dictionary containing a list of soundtracks.
         """
         endpoint = f"v1/rest/soundtrack/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_spacecraft_by_id(self, uid):
         """
         Returns information about a Star Trek spacecraft matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the spacecraft.
+            uid (str): The unique identifier for the spacecraft.
         
         Returns:
-        - dict: A dictionary containing information about the spacecraft.
+            dict: A dictionary containing information about the spacecraft.
         """
         endpoint = f"v2/rest/spacecraft?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_spacecrafts(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek spacecrafts of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of spacecrafts per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of spacecrafts per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of spacecrafts.
+            dict: A dictionary containing a list of spacecrafts.
         """
         endpoint = f"v2/rest/spacecraft/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_spacecraft_class_by_id(self, uid):
         """
         Returns information about a Star Trek spacecraft class matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the spacecraft class.
+            uid (str): The unique identifier for the spacecraft class.
         
         Returns:
-        - dict: A dictionary containing information about the spacecraft class.
+            dict: A dictionary containing information about the spacecraft class.
         """
         endpoint = f"v2/rest/spacecraftClass?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_spacecraft_classes(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek spacecraft classes of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of spacecraft classes per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of spacecraft classes per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of spacecraft classes.
+            dict: A dictionary containing a list of spacecraft classes.
         """
         endpoint = f"v2/rest/spacecraftClass/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_species_by_id(self, uid):
         """
         Returns information about a Star Trek species matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the species.
+            uid (str): The unique identifier for the species.
         
         Returns:
-        - dict: A dictionary containing information about the species.
+            dict: A dictionary containing information about the species.
         """
         endpoint = f"v2/rest/species?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_species(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek species of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of species per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of species per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of species.
+            dict: A dictionary containing a list of species.
         """
         endpoint = f"v2/rest/species/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_staff_by_id(self, uid):
         """
         Returns information about a Star Trek staff matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the staff.
+            uid (str): The unique identifier for the staff.
         
         Returns:
-        - dict: A dictionary containing information about the staff.
+            dict: A dictionary containing information about the staff.
         """
         endpoint = f"v2/rest/staff?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_staff(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek staff of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of staff per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of staff per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of staff.
+            dict: A dictionary containing a list of staff.
         """
         endpoint = f"v2/rest/staff/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_technology_by_id(self, uid):
         """
         Returns information about a Star Trek technology matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the technology.
+            uid (str): The unique identifier for the technology.
         
         Returns:
-        - dict: A dictionary containing information about the technology.
+            dict: A dictionary containing information about the technology.
         """
         endpoint = f"v2/rest/technology?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_technologies(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek technologies of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of technologies per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of technologies per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of technologies.
+            dict: A dictionary containing a list of technologies.
         """
         endpoint = f"v2/rest/technology/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_title_by_id(self, uid):
         """
         Returns information about a Star Trek titles matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the title.
+            uid (str): The unique identifier for the title.
         
         Returns:
-        - dict: A dictionary containing information about the title.
+            dict: A dictionary containing information about the title.
         """
         endpoint = f"v2/rest/title?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_titles(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek titles of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of titles per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of titles per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of titles.
+            dict: A dictionary containing a list of titles.
         """
         endpoint = f"v2/rest/title/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_card_by_id(self, uid):
         """
         Returns information about a Star Trek trading card matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the trading card.
+            uid (str): The unique identifier for the trading card.
         
         Returns:
-        - dict: A dictionary containing information about the trading card.
+            dict: A dictionary containing information about the trading card.
         """
         endpoint = f"v1/rest/tradingCard?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_cards(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek trading cards of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of trading cards per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of trading cards per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of trading cards.
+            dict: A dictionary containing a list of trading cards.
         """
         endpoint = f"v1/rest/tradingCard/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_card_deck_by_id(self, uid):
         """
         Returns information about a Star Trek trading card deck matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the trading card deck.
+            uid (str): The unique identifier for the trading card deck.
         
         Returns:
-        - dict: A dictionary containing information about the trading card deck.
+            dict: A dictionary containing information about the trading card deck.
         """
         endpoint = f"v1/rest/tradingCardDeck?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_card_decks(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek trading card decks of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of trading card decks per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of trading card decks per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of trading card decks.
+            dict: A dictionary containing a list of trading card decks.
         """
         endpoint = f"v1/rest/tradingCardDeck/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_card_set_by_id(self, uid):
         """
         Returns information about a Star Trek trading card set matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the trading card set.
+            uid (str): The unique identifier for the trading card set.
         
         Returns:
-        - dict: A dictionary containing information about the trading card set.
+            dict: A dictionary containing information about the trading card set.
         """
         endpoint = f"v1/rest/tradingCardSet?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_trading_card_sets(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek trading card sets of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of trading card sets per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of trading card sets per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of trading card sets.
+            dict: A dictionary containing a list of trading card sets.
         """
         endpoint = f"v1/rest/tradingCardSet/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_video_game_by_id(self, uid):
         """
         Returns information about a Star Trek video game matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the video game.
+            uid (str): The unique identifier for the video game.
         
         Returns:
-        - dict: A dictionary containing information about the video game.
+            dict: A dictionary containing information about the video game.
         """
         endpoint = f"v1/rest/videoGame?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_video_games(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek video games of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of video games per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of video games per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of video games.
+            dict: A dictionary containing a list of video games.
         """
         endpoint = f"v1/rest/videoGame/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_video_release_by_id(self, uid):
         """
         Returns information about a Star Trek video release matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the video release.
+            uid (str): The unique identifier for the video release.
         
         Returns:
-        - dict: A dictionary containing information about the video release.
+            dict: A dictionary containing information about the video release.
         """
         endpoint = f"v2/rest/videoRelease?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_video_releases(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek video releases of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of video releases per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of video releases per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of video releases.
+            dict: A dictionary containing a list of video releases.
         """
         endpoint = f"v2/rest/videoRelease/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_weapon_by_id(self, uid):
         """
         Returns information about a Star Trek weapon matching the unique id.
         
         Args:
-        - uid (str): The unique identifier for the weapon.
+            uid (str): The unique identifier for the weapon.
         
         Returns:
-        - dict: A dictionary containing information about the weapon.
+            dict: A dictionary containing information about the weapon.
         """
         endpoint = f"v2/rest/weapon?uid={uid}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_weapons(self, pageNumber=0, pageSize=50):
         """
         Returns a list of Star Trek weapons of the specified page number and page size.
         
         Args:
-        - pageNumber (int): The page number of the list. Defaults to 0, the first page.
-        - pageSize (int): The number of weapons per page. Defaults to 50.
+            pageNumber (int): The page number of the list. Defaults to 0, the first page.
+            pageSize (int): The number of weapons per page. Defaults to 50.
         
         Returns:
-        - dict: A dictionary containing a list of weapons.
+            dict: A dictionary containing a list of weapons.
         """
         endpoint = f"v2/rest/weapon/search?pageNumber={pageNumber}&pageSize={pageSize}"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/nokey/weather/national_weather_service.py` & `nokey-0.7.4/nokey/weather/national_weather_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,722 +3,722 @@
 
 
 class NationalWeatherService:
     """
     A class to interact with the National Weather Service API.
     
     Attributes:
-    - base_url: The base URL of the National Weather Service API.
-    - about: A short description of the API.
+        base_url: The base URL of the National Weather Service API.
+        about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="nws_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://api.weather.gov/"
         self.about = "The National Weather Service (NWS) API allows developers access to critical forecasts, alerts, and observations, along with other weather data."
         
         if use_caching:
             requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
             
     def get_docs_url(self):
         """
         Returns URL for API docs.
         
         Args:
-        - None
+            None
         
         Returns:
-        - string: URL for API documentation.
+            string: URL for API documentation.
         """
         return "https://www.weather.gov/documentation/services-web-api"       
     
     def get_alerts(self):
         """
         Returns a collection of weather alerts.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: Inforation on weather alerts
+            dict: Inforation on weather alerts
         """
         endpoint = "alerts"
         return mr.make_request(self.base_url+endpoint)
         
     def get_active_alerts(self):
         """
         Returns a collection of currently active weather alerts.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: Inforation on currently active weather alerts
+            dict: Inforation on currently active weather alerts
         """
         endpoint = "alerts/active"
         return mr.make_request(self.base_url+endpoint)
         
     def get_active_alerts_count(self):
         """
         Returns the count of currently active weather alerts broken down by various categories.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: Count of currently active weather alerts broke down by categories.
+            dict: Count of currently active weather alerts broke down by categories.
         """
         endpoint = "alerts/active/count"
         return mr.make_request(self.base_url+endpoint)
         
     def get_active_alerts_by_zone(self, zoneID):
         """
         Returns active alerts for the given NWS public zone or county.
         
         Args:
-        - zoneID (str): NWS public zone/county identifier
+            zoneID (str): NWS public zone/county identifier
         
         Returns:
-        - dict: Information of active alerts in the zone specified by zoneID.
+            dict: Information of active alerts in the zone specified by zoneID.
         """
         endpoint = f"alerts/active/zone/{zoneID}"
         return mr.make_request(self.base_url+endpoint)
     
     def get_active_alerts_by_area(self, area):
         """
         Returns active alerts for the given area (state or marine area).
         
         Args:
-        - area (str): State or marine area ID
+            area (str): State or marine area ID
         
         Returns:
-        - dict: Information of active alerts in the area specified.
+            dict: Information of active alerts in the area specified.
         """
         endpoint = f"alerts/active/area/{area}"
         return mr.make_request(self.base_url+endpoint)
     
     def get_active_alerts_by_region(self, region):
         """
         Returns active alerts for the given marine region ID. Available values : AL, AT, GL, GM, PA, PI."
         
         Args:
-        - region (str): Marine region ID. Available values : AL, AT, GL, GM, PA, PI.
+            region (str): Marine region ID. Available values : AL, AT, GL, GM, PA, PI.
         
         Returns:
-        - dict: Information of active alerts in the area specified.
+            dict: Information of active alerts in the area specified.
         """
         endpoint = f"alerts/active/region/{region}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_alert_types(self):
         """
         Returns a list of alerts types.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of alert types.
+            dict: A dictionary containing a list of alert types.
         """
         endpoint = "alerts/types"
         return mr.make_request(self.base_url+endpoint)
         
     def get_alert_by_id(self, ID):
         """
         Returns a specific alert record.
 
         Args:
-        - ID (str): Alert identifier.
+            ID (str): Alert identifier.
 
         Returns:
-        - dict: A dictionary containing information about a specific alert.
+            dict: A dictionary containing information about a specific alert.
         """
         endpoint = f"alerts/{ID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_cwsu_metadata(self, cwsuID):
         """
         Returns metadata about a Center Weather Service Unit.
 
         Args:
-        - cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
+            cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
 
         Returns:
-        - dict: Metadata about a cwsu.
+            dict: Metadata about a cwsu.
         """
         endpoint = f"aviation/cwsus/{cwsuID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_cwsu_advisories(self, cwsuID):
         """
         Returns a list of Center Weather Advisories from a CWSU.
 
         Args:
-        - cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
+            cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
 
         Returns:
-        - dict: Dictionary containing list of  Center Weather Advisories from a CWSU.
+            dict: Dictionary containing list of  Center Weather Advisories from a CWSU.
         """
         endpoint = f"aviation/cwsus/{cwsuID}/cwas"
         return mr.make_request(self.base_url+endpoint)
     
     def get_cwsu_advisories_by_date_and_seq(self, cwsuID, date, sequence):
         """
         Returns a list of Center Weather Advisories from a CWSU.
 
         Args:
-        - cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
-        - date (str): (YYYY-MM-DD format) Date of advisory.
-        - sequence (int): Sequence number
+            cwsuID (str): NWS CWSU ID. Available values : ZAB, ZAN, ZAU, ZBW, ZDC, ZDV, ZFA, ZFW, ZHU, ZID, ZJX, ZKC, ZLA, ZLC, ZMA, ZME, ZMP, ZNY, ZOA, ZOB, ZSE, ZTL.
+            date (str): (YYYY-MM-DD format) Date of advisory.
+            sequence (int): Sequence number
         
         Returns:
-        - dict: Dictionary containing list of Center Weather Advisories from a CWSU.
+            dict: Dictionary containing list of Center Weather Advisories from a CWSU.
         """
         endpoint = f"aviation/cwsus/{cwsuID}/cwas/{date}/{sequence}"
         return mr.make_request(self.base_url+endpoint)
 
 # DON'T YET KNOW HOW THIS WORKS. ARGS ARE QUERIES, NOT PATHS      
 #    def get_sigmets(self, start_time, end_time, date, atsu, sequence):
 #        """
 #        Returns a list of SIGMET/AIRMETs.
 #
 #        Args:
-#        - start_time (str): Start time.
-#        - end_time (str): End time.
-#        - date (str): (YYYY-MM-DD format) Date
-#        - atsu (str): ATSU identifier
-#        - sequence (str): SIGMET sequence number
+#            start_time (str): Start time.
+#            end_time (str): End time.
+#            date (str): (YYYY-MM-DD format) Date
+#            atsu (str): ATSU identifier
+#            sequence (str): SIGMET sequence number
 #
 #        Returns:
-#        - dict: Metadata about a cwsu.
+#            dict: Metadata about a cwsu.
 #        """
 #        endpoint = f"aviation/sigmet?{start_time}?{end_time}?{date}?{atsu}?{sequence}"
 #        return mr.make_request(self.base_url+endpoint)
 
     def get_sigmets_by_atsu(self, atsu):
         """
         Returns a list of SIGMET/AIRMETs for the specified ATSU.
 
         Args:
-        - atsu (str): ATSU identifier.
+            atsu (str): ATSU identifier.
         
         Returns:
-        - dict: Dictionary containing list of SIGMET/AIRMETs for the specified ATSU.
+            dict: Dictionary containing list of SIGMET/AIRMETs for the specified ATSU.
         """
         endpoint = f"aviation/sigmets/{atsu}"
         return mr.make_request(self.base_url+endpoint)
 
     def get_sigmets_by_atsu_and_date(self, atsu, date):
         """
         Returns a list of SIGMET/AIRMETs for the specified ATSU for the specified date.
 
         Args:
-        - atsu (str): ATSU identifier.
-        - date (str): Date (YYYY-MM-DD format)
+            atsu (str): ATSU identifier.
+            date (str): Date (YYYY-MM-DD format)
         
         Returns:
-        - dict: Dictionary containing list of SIGMET/AIRMETs for the specified ATSU and specified date.
+            dict: Dictionary containing list of SIGMET/AIRMETs for the specified ATSU and specified date.
         """
         endpoint = f"aviation/sigmets/{atsu}/{date}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_specific_sigmet(self, atsu, date, time):
         """
         Returns a list of SIGMET/AIRMETs for the specified ATSU for the specified date.
 
         Args:
-        - atsu (str): ATSU identifier.
-        - date (str): Date (YYYY-MM-DD format)
-        - time (str): Time (HHMM format). This time is always specified in UTC (Zulu) time.
+            atsu (str): ATSU identifier.
+            date (str): Date (YYYY-MM-DD format)
+            time (str): Time (HHMM format). This time is always specified in UTC (Zulu) time.
         
         Returns:
-        - dict: Dictionary containing a specific SIGMET/AIRMET.
+            dict: Dictionary containing a specific SIGMET/AIRMET.
         """
         endpoint = f"aviation/sigmets/{atsu}/{date}/{time}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_glossary(self):
         """
         Returns glossary terms.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of glossary terms and definitions.
+            dict: A dictionary containing a list of glossary terms and definitions.
         """
         endpoint = "glossary"
         return mr.make_request(self.base_url+endpoint)
         
     def get_raw_data_by_gridpoints(self, wfo, x, y):
         """
         Returns raw numerical forecast data for a 2.5km grid area.
 
         Args:
-        - wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
-        - x (int): Forecast grid X coordinate.
-        - y (int): Forecast grid Y coordinate.
+            wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
+            x (int): Forecast grid X coordinate.
+            y (int): Forecast grid Y coordinate.
         
         Returns:
-        - dict: Dictionary containing the raw numerical forcast data.
+            dict: Dictionary containing the raw numerical forcast data.
         """
         endpoint = f"gridpoints/{wfo}/{x},{y}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_textual_forecast_by_gridpoints(self, wfo, x, y):
         """
         Returns a textual forecast for a 2.5km grid area.
 
         Args:
-        - wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
-        - x (int): Forecast grid X coordinate.
-        - y (int): Forecast grid Y coordinate.
+            wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
+            x (int): Forecast grid X coordinate.
+            y (int): Forecast grid Y coordinate.
         
         Returns:
-        - dict: Dictionary containing the textual forcast data.
+            dict: Dictionary containing the textual forcast data.
         """
         endpoint = f"gridpoints/{wfo}/{x},{y}/forecast"
         return mr.make_request(self.base_url+endpoint)
         
     def get_textual_hourly_forecast_by_gridpoints(self, wfo, x, y):
         """
         Returns a textual hourly forecast for a 2.5km grid area.
 
         Args:
-        - wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
-        - x (int): Forecast grid X coordinate.
-        - y (int): Forecast grid Y coordinate.
+            wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
+            x (int): Forecast grid X coordinate.
+            y (int): Forecast grid Y coordinate.
         
         Returns:
-        - dict: Dictionary containing the textual hourly forcast data.
+            dict: Dictionary containing the textual hourly forcast data.
         """
         endpoint = f"gridpoints/{wfo}/{x},{y}/forecast/hourly"
         return mr.make_request(self.base_url+endpoint)
         
     def get_observation_stations_by_gridpoints(self, wfo, x, y):
         """
         Returns a list of observation stations usable for a given 2.5km grid area.
 
         Args:
-        - wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
-        - x (int): Forecast grid X coordinate.
-        - y (int): Forecast grid Y coordinate.
+            wfo (str): Forecast office ID. Available values : AKQ, ALY, BGM, BOX, BTV, BUF, CAE, CAR, CHS, CLE, CTP, GSP, GYX, ILM, ILN, LWX, MHX, OKX, PBZ, PHI, RAH, RLX, RNK, ABQ, AMA, BMX, BRO, CRP, EPZ, EWX, FFC, FWD, HGX, HUN, JAN, JAX, KEY, LCH, LIX, LUB, LZK, MAF, MEG, MFL, MLB, MOB, MRX, OHX, OUN, SHV, SJT, SJU, TAE, TBW, TSA, ABR, APX, ARX, BIS, BOU, CYS, DDC, DLH, DMX, DTX, DVN, EAX, FGF, FSD, GID, GJT, GLD, GRB, GRR, ICT, ILX, IND, IWX, JKL, LBF, LMK, LOT, LSX, MKX, MPX, MQT, OAX, PAH, PUB, RIW, SGF, TOP, UNR, BOI, BYZ, EKA, FGZ, GGW, HNX, LKN, LOX, MFR, MSO, MTR, OTX, PDT, PIH, PQR, PSR, REV, SEW, SGX, SLC, STO, TFX, TWC, VEF, AER, AFC, AFG, AJK, ALU, GUM, HPA, HFO, PPG, STU, NH1, NH2, ONA, ONP
+            x (int): Forecast grid X coordinate.
+            y (int): Forecast grid Y coordinate.
         
         Returns:
-        - dict: Dictionary containing a list of observation stations usable for a given 2.5km grid area.
+            dict: Dictionary containing a list of observation stations usable for a given 2.5km grid area.
         """
         endpoint = f"gridpoints/{wfo}/{x},{y}/stations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_observations_by_station(self, stationID):
         """
         Returns a list of observations for a given station.
 
         Args:
-        - stationID (str): Observation station ID.
+            stationID (str): Observation station ID.
         
         Returns:
-        - dict: Dictionary containing list of observations for a given station.
+            dict: Dictionary containing list of observations for a given station.
         """
         endpoint = f"stations/{stationID}/observations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_station_observation_by_time(self, stationID, time):
         """
         Returns a single observation.
 
         Args:
-        - stationID (str): Observation station ID.
-        - time (str): Timestamp of requested observation.
+            stationID (str): Observation station ID.
+            time (str): Timestamp of requested observation.
         
         Returns:
-        - dict: Dictionary containing single observation for a given station at a given time.
+            dict: Dictionary containing single observation for a given station at a given time.
         """
         endpoint = f"stations/{stationID}/observations/{time}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_tafs_by_station(self, stationID):
         """
         Returns Terminal Aerodrome Forecasts for the specified airport station.
 
         Args:
-        - stationID (str): Observation station ID.
+            stationID (str): Observation station ID.
         
         Returns:
-        - dict: Dictionary containing TAFS for given station.
+            dict: Dictionary containing TAFS for given station.
         """
         endpoint = f"stations/{stationID}/tafs"
         return mr.make_request(self.base_url+endpoint)
         
     def get_taf_by_date_time(self, stationID, date, time):
         """
         Returns a single Terminal Aerodrome Forecast..
 
         Args:
-        - stationID (str): Observation station ID.
-        - date (str): Date (YYYY-MM-DD format)
-        - time (str) Time (HHMM format). This time is always specified in UTC (Zulu) time.
+            stationID (str): Observation station ID.
+            date (str): Date (YYYY-MM-DD format)
+            time (str) Time (HHMM format). This time is always specified in UTC (Zulu) time.
         
         Returns:
-        - dict: Dictionary containing TAF.
+            dict: Dictionary containing TAF.
         """
         endpoint = f"stations/{stationID}/tafs/{date}/{time}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_stations(self):
         """
         Returns a list of observation stations.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of observation stations.
+            dict: A dictionary containing a list of observation stations.
         """
         endpoint = "stations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_station_metadata(self, stationID):
         """
         Returns metadata about a given observation station.
 
         Args:
-        - stationID (str): Observation station ID.
+            stationID (str): Observation station ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given station.
+            dict: Dictionary containing metadata for given station.
         """
         endpoint = f"stations/{stationID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_NWS_office_metadata(self, officeID):
         """
         Returns metadata about a NWS forecast office.
 
         Args:
-        - officeID (str): NWS office ID.
+            officeID (str): NWS office ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given NWS office.
+            dict: Dictionary containing metadata for given NWS office.
         """
         endpoint = f"offices/{officeID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_NWS_office_headline_by_headline_id(self, officeID, headlineID):
         """
         Returns a specific news headline for a given NWS office.
 
         Args:
-        - officeID (str): NWS office ID.
-        - headlineID (str): Headline record ID.
+            officeID (str): NWS office ID.
+            headlineID (str): Headline record ID.
         
         Returns:
-        - dict: Dictionary containing headline for given NWS office and given headline ID.
+            dict: Dictionary containing headline for given NWS office and given headline ID.
         """
         endpoint = f"offices/{officeID}/headlines/{headlineID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_NWS_office_headlines(self, officeID):
         """
         Returns a list of news headlines for a given NWS office.
 
         Args:
-        - officeID (str): NWS office ID.
+            officeID (str): NWS office ID.
         
         Returns:
-        - dict: Dictionary containing headlines for given NWS office.
+            dict: Dictionary containing headlines for given NWS office.
         """
         endpoint = f"offices/{officeID}/headlines"
         return mr.make_request(self.base_url+endpoint)
 
 # HAVEN'T FIGURED THIS ONE OUT, HOW TO PASS POINT ARG AS LAT AND LONG      
 #    def get_metadata_by_point(self, point):
 #        """
 #        Returns metadata about a given latitude/longitude point.
 #
 #        Args:
-#        - point (str): Point(latitude,longitude)
+#            point (str): Point(latitude,longitude)
 #        
 #        Returns:
-#        - dict: Dictionary containing metadata for given point.
+#            dict: Dictionary containing metadata for given point.
 #        """
 #        endpoint = f"points/{point}"
 #        return mr.make_request(self.base_url+endpoint)
 
     def get_radar_servers(self):
         """
         Returns a list of radar servers.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of radar servers.
+            dict: A dictionary containing a list of radar servers.
         """
         endpoint = "radar/servers"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_server_metadata_by_id(self, serverID):
         """
         Returns metadata about a given radar server.
 
         Args:
-        - serverID (str): Radar server ID.
+            serverID (str): Radar server ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given radar server.
+            dict: Dictionary containing metadata for given radar server.
         """
         endpoint = f"radar/servers/{serverID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_stations(self):
         """
         Returns a list of radar stations.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of radar stations.
+            dict: A dictionary containing a list of radar stations.
         """
         endpoint = "radar/stations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_station_metadata_by_id(self, stationID):
         """
         Returns metadata about a given radar station.
 
         Args:
-        - stationID (str): Radar station ID.
+            stationID (str): Radar station ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given radar station.
+            dict: Dictionary containing metadata for given radar station.
         """
         endpoint = f"radar/stations/{stationID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_station_alarms_metadata_by_id(self, stationID):
         """
         Returns metadata about a given radar station alarms.
 
         Args:
-        - stationID (str): Radar station ID.
+            stationID (str): Radar station ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given radar station alarms.
+            dict: Dictionary containing metadata for given radar station alarms.
         """
         endpoint = f"radar/stations/{stationID}/alarms"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_queue_metadata(self, host):
         """
         Returns metadata about a given radar queue.
 
         Args:
-        - host (str): LDM host.
+            host (str): LDM host.
         
         Returns:
-        - dict: Dictionary containing metadata for given radar queue.
+            dict: Dictionary containing metadata for given radar queue.
         """
         endpoint = f"radar/queues/{host}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_radar_wind_profiler_metadata(self, stationID):
         """
         Returns metadata about a given radar wind profiler.
 
         Args:
-        - stationID (str): Profiler station ID.
+            stationID (str): Profiler station ID.
         
         Returns:
-        - dict: Dictionary containing metadata for given radar wind profiler.
+            dict: Dictionary containing metadata for given radar wind profiler.
         """
         endpoint = f"radar/profilers/{stationID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_products(self):
         """
         Returns a list of text products.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of text products.
+            dict: A dictionary containing a list of text products.
         """
         endpoint = "products"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_product_locations(self):
         """
         Returns a list of valid text product issuance locations.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of valid text product issuance locations.
+            dict: A dictionary containing a list of valid text product issuance locations.
         """
         endpoint = "products/locations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_product_types(self):
         """
         Returns a list of valid text product types and codes.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of valid text product types and codes.
+            dict: A dictionary containing a list of valid text product types and codes.
         """
         endpoint = "products/types"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_product_by_id(self, productID):
         """
         Returns a specific text product.
 
         Args:
-        - productID (str): Text product ID.
+            productID (str): Text product ID.
         
         Returns:
-        - dict: Dictionary containing specific text product.
+            dict: Dictionary containing specific text product.
         """
         endpoint = f"products/{productID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_products_by_type(self, typeID):
         """
         Returns a list of text products of a given type.
 
         Args:
-        - typeID (str): Text product type ID.
+            typeID (str): Text product type ID.
         
         Returns:
-        - dict: Dictionary containing list of text products of given type.
+            dict: Dictionary containing list of text products of given type.
         """
         endpoint = f"products/types/{typeID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_product_locations_by_type(self, typeID):
         """
         Returns a list of valid text product issuance locations for a given product type.
 
         Args:
-        - typeID (str): Text product type ID.
+            typeID (str): Text product type ID.
         
         Returns:
-        - dict: Dictionary containing list of valid text product issuance locations for a given type.
+            dict: Dictionary containing list of valid text product issuance locations for a given type.
         """
         endpoint = f"products/types/{typeID}/locations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_product_types_by_location(self, locationID):
         """
         Returns a list of valid text product types for a given issuance location.
 
         Args:
-        - locationID (str): Location ID.
+            locationID (str): Location ID.
         
         Returns:
-        - dict: Dictionary containing list of valid text product types for a given location.
+            dict: Dictionary containing list of valid text product types for a given location.
         """
         endpoint = f"products/locations/{locationID}/types"
         return mr.make_request(self.base_url+endpoint)
         
     def get_text_products_by_type_and_location(self, typeID, locationID):
         """
         Returns a list of text products of a given type for a given issuance location.
 
         Args:
-        - typeID (str): Text product type ID.
-        - locationID (str): Location ID.
+            typeID (str): Text product type ID.
+            locationID (str): Location ID.
         
         Returns:
-        - dict: Dictionary containing list of text product of a given type for a given issuance location.
+            dict: Dictionary containing list of text product of a given type for a given issuance location.
         """
         endpoint = f"products/types/{typeID}/locations/{locationID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_zones(self):
         """
         Returns a list of zones.
 
         Args:
-        - None
+            None
 
         Returns:
-        - dict: A dictionary containing a list of zones.
+            dict: A dictionary containing a list of zones.
         """
         endpoint = "zones"
         return mr.make_request(self.base_url+endpoint)
 
 # HAVEN'T FIGURED THIS ONE OUT. PARAMETER IS A QUERY, NOT PATH  
     def get_zones_by_type(self, Type):
         """
         Returns a list of valid text product types for a given issuance location.
 
         Args:
-        - Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
+            Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
         
         Returns:
-        - dict: Dictionary containing list of valid text product types for a given location.
+            dict: Dictionary containing list of valid text product types for a given location.
         """
         endpoint = f"zones/{Type}"
         return mr.make_request(self.base_url+endpoint)
 
     def get_zone_metadata(self, Type, zoneID):
         """
         Returns metadata about a given zone.
 
         Args:
-        - Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
-        - zoneID (str): NWS public zone/county identifier.
+            Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
+            zoneID (str): NWS public zone/county identifier.
         
         Returns:
-        - dict: Dictionary containing metadata about a given zone.
+            dict: Dictionary containing metadata about a given zone.
         """
         endpoint = f"zones/{Type}/{zoneID}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_zone_forecast(self, Type, zoneID):
         """
         Returns the current zone forecast for a given zone.
 
         Args:
-        - Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
-        - zoneID (str): NWS public zone/county identifier.
+            Type (str): Zone type. Available values : land, marine, forecast, public, coastal, offshore, fire, county.
+            zoneID (str): NWS public zone/county identifier.
         
         Returns:
-        - dict: Dictionary containing zone forecast for a given zone.
+            dict: Dictionary containing zone forecast for a given zone.
         """
         endpoint = f"zones/{Type}/{zoneID}/forecast"
         return mr.make_request(self.base_url+endpoint)
         
     def get_zone_observations(self, zoneID):
         """
         Returns a list of observations for a given zone.
 
         Args:
-        - zoneID (str): NWS public zone/county identifier.
+            zoneID (str): NWS public zone/county identifier.
         
         Returns:
-        - dict: Dictionary containing a list of observations for a given zkne.
+            dict: Dictionary containing a list of observations for a given zkne.
         """
         endpoint = f"zones/forecast/{zoneID}/observations"
         return mr.make_request(self.base_url+endpoint)
         
     def get_observation_stations_by_zone(self, zoneID):
         """
         Returns a list of observation stations for a given zone.
 
         Args:
-        - zoneID (str): NWS public zone/county identifier.
+            zoneID (str): NWS public zone/county identifier.
         
         Returns:
-        - dict: Dictionary containing a list of observation stations for a given zkne.
+            dict: Dictionary containing a list of observation stations for a given zkne.
         """
         endpoint = f"zones/forecast/{zoneID}/stations"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.7.3/pyproject.toml` & `nokey-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nokey"
-version = "0.7.3"
+version = "0.7.4"
 description = "A python package for accessing APIs that require no key."
 authors = ["Spyder Rex <billyjohnsonauthor@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/SpyderRex/nokey"
 repository = "https://github.com/SpyderRex/nokey"
 license = "MIT"
 keywords = ["API", "requests", "xmltodict"]
```

### Comparing `nokey-0.7.3/PKG-INFO` & `nokey-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.7.3
+Version: 0.7.4
 Summary: A python package for accessing APIs that require no key.
 Home-page: https://github.com/SpyderRex/nokey
 License: MIT
 Keywords: API,requests,xmltodict
 Author: Spyder Rex
 Author-email: billyjohnsonauthor@gmail.com
 Requires-Python: >=3.8,<4.0
```

