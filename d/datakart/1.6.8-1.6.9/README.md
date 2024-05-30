# Comparing `tmp/datakart-1.6.8.tar.gz` & `tmp/datakart-1.6.9.tar.gz`

## Comparing `datakart-1.6.8.tar` & `datakart-1.6.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.8/requirements.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.8/.vscode/settings.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/__init__.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/datagokr.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/ecos.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/jusogokr.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/kakao.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/naver.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/naver_ad.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/sgis.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/_converter.py
--rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/na_biztp.json
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 datakart-1.6.8/src/datakart/core/assets/na_event.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.8/tests/__init__.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.8/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.8/LICENSE
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.8/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.8/pyproject.toml
--rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 datakart-1.6.9/requirements.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 datakart-1.6.9/.vscode/settings.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/__init__.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/datagokr.py
+-rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/ecos.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/jusogokr.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/kakao.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/naver.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/naver_ad.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/sgis.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/assets/_converter.py
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/assets/na_biztp.tsv
+-rwxr-xr-x   0        0        0     2107 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/assets/na_event.md
+-rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/assets/naver_ad_biztp.json
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 datakart-1.6.9/src/datakart/core/assets/naver_ad_event.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datakart-1.6.9/tests/__init__.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 datakart-1.6.9/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 datakart-1.6.9/LICENSE
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 datakart-1.6.9/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 datakart-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 datakart-1.6.9/PKG-INFO
```

### Comparing `datakart-1.6.8/src/datakart/core/datagokr.py` & `datakart-1.6.9/src/datakart/core/datagokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/ecos.py` & `datakart-1.6.9/src/datakart/core/ecos.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/jusogokr.py` & `datakart-1.6.9/src/datakart/core/jusogokr.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/kakao.py` & `datakart-1.6.9/src/datakart/core/kakao.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/naver.py` & `datakart-1.6.9/src/datakart/core/naver.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/naver_ad.py` & `datakart-1.6.9/src/datakart/core/naver_ad.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,22 +55,26 @@
             **({"month": month} if month else {}),
         }
         resp = requests.get(self.host_url + url, headers=headers, params=params)
         resp.raise_for_status()
         return resp.json()
 
     @staticmethod
-    def biztp_cd() -> List[Dict]:
+    def get_biztp_codes() -> List[Dict]:
         import json
         import pathlib
 
-        with open(pathlib.Path(__file__).parent / "assets" / "na_biztp.json") as fp:
+        with open(
+            pathlib.Path(__file__).parent / "assets" / "naver_ad_biztp.json"
+        ) as fp:
             return json.load(fp)
 
     @staticmethod
-    def event_cd() -> List[Dict]:
+    def get_event_codes() -> List[Dict]:
         # https://gist.github.com/naver-searchad/235202ffb08f9433b6f7cb10e45875f7#file-seasonal_event_code-md
         import json
         import pathlib
 
-        with open(pathlib.Path(__file__).parent / "assets" / "na_event.json") as fp:
+        with open(
+            pathlib.Path(__file__).parent / "assets" / "naver_ad_event.json"
+        ) as fp:
             return json.load(fp)
```

### Comparing `datakart-1.6.8/src/datakart/core/sgis.py` & `datakart-1.6.9/src/datakart/core/sgis.py`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/src/datakart/core/assets/na_biztp.json` & `datakart-1.6.9/src/datakart/core/assets/naver_ad_biztp.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7532894736842105%*

 * *Differences: {'100': "{'id': 103, 'name_kr': 'IT수리/관리서비스'}",*

 * * '101': "{'id': 104, 'name_kr': 'IT시스템/솔루션'}",*

 * * '102': "{'id': 105, 'name_kr': '웹호스팅/사이트제작'}",*

 * * '105': "{'id': 121, 'name_kr': '스튜디오/사진관', 'pid': 24}",*

 * * '106': "{'id': 122, 'name_kr': '운세/사주/작명'}",*

 * * '108': "{'id': 124, 'name_kr': '장례/상조'}",*

 * * '110': "{'id': 126, 'name_kr': '생활정보/커뮤니티'}",*

 * * '111': "{'id': 127, 'name_kr': '기타생활서비스'}",*

 * * '112': "{'id': 128, 'name_kr': '생활용품판매', 'pid': 25}",*

 * * '114': "{'id': 130, 'name_kr': '애완동물/용품', 'pid': 26}",*

 * * '120': "{'id': 137, […]*

```diff
@@ -1,33 +1,21 @@
 [
     {
-        "id": 20,
-        "level": 1,
-        "name_kr": "IT/\ud154\ub808\ucf64",
-        "pid": 0
-    },
-    {
         "id": 1,
         "level": 1,
         "name_kr": "\uac00\uc815/\uc0dd\ud65c",
         "pid": 0
     },
     {
         "id": 2,
         "level": 1,
         "name_kr": "\uac74\uac15/\ubbf8\uc6a9",
         "pid": 0
     },
     {
-        "id": 376,
-        "level": 1,
-        "name_kr": "\uac74\ucd95/\uc778\ud14c\ub9ac\uc5b4",
-        "pid": 0
-    },
-    {
         "id": 3,
         "level": 1,
         "name_kr": "\uacb0\ud63c/\ucd9c\uc0b0/\uc721\uc544",
         "pid": 0
     },
     {
         "id": 4,
@@ -86,14 +74,20 @@
     {
         "id": 13,
         "level": 1,
         "name_kr": "\uc5ec\ud589/\uad50\ud1b5",
         "pid": 0
     },
     {
+        "id": 14,
+        "level": 1,
+        "name_kr": "\uc885\ud569\uc1fc\ud551",
+        "pid": 0
+    },
+    {
         "id": 15,
         "level": 1,
         "name_kr": "\uc758\ub958/\ud328\uc158\uc7a1\ud654",
         "pid": 0
     },
     {
         "id": 16,
@@ -116,17 +110,17 @@
     {
         "id": 19,
         "level": 1,
         "name_kr": "\uc804\uc790/\uac00\uc804",
         "pid": 0
     },
     {
-        "id": 14,
+        "id": 20,
         "level": 1,
-        "name_kr": "\uc885\ud569\uc1fc\ud551",
+        "name_kr": "IT/\ud154\ub808\ucf64",
         "pid": 0
     },
     {
         "id": 23,
         "level": 2,
         "name_kr": "\uac00\uad6c",
         "pid": 1
@@ -212,41 +206,41 @@
     {
         "id": 37,
         "level": 2,
         "name_kr": "\ucd9c\uc0b0/\uc721\uc544\uad00\ub828\uc11c\ube44\uc2a4",
         "pid": 3
     },
     {
-        "id": 40,
+        "id": 38,
         "level": 2,
-        "name_kr": "\uad50\uc721/\ucde8\uc5c5\uc815\ubcf4",
+        "name_kr": "\ud559\uad50",
         "pid": 4
     },
     {
-        "id": 41,
+        "id": 39,
         "level": 2,
-        "name_kr": "\uad50\uc721\uc9c0\uc6d0",
+        "name_kr": "\ud559\uc6d0/\ud559\uc2b5",
         "pid": 4
     },
     {
-        "id": 42,
+        "id": 40,
         "level": 2,
-        "name_kr": "\uad50\uc7ac/\uc6a9\ud488\ud310\ub9e4",
+        "name_kr": "\uad50\uc721/\ucde8\uc5c5\uc815\ubcf4",
         "pid": 4
     },
     {
-        "id": 38,
+        "id": 41,
         "level": 2,
-        "name_kr": "\ud559\uad50",
+        "name_kr": "\uad50\uc721\uc9c0\uc6d0",
         "pid": 4
     },
     {
-        "id": 39,
+        "id": 42,
         "level": 2,
-        "name_kr": "\ud559\uc6d0/\ud559\uc2b5",
+        "name_kr": "\uad50\uc7ac/\uc6a9\ud488\ud310\ub9e4",
         "pid": 4
     },
     {
         "id": 43,
         "level": 2,
         "name_kr": "\uae08\uc735/\ubcf4\ud5d8\uae30\uad00",
         "pid": 5
@@ -272,59 +266,53 @@
     {
         "id": 47,
         "level": 2,
         "name_kr": "\uc774\ubca4\ud2b8",
         "pid": 6
     },
     {
-        "id": 49,
-        "level": 2,
-        "name_kr": "\uac15\uc2b5/\ud504\ub85c\uadf8\ub7a8",
-        "pid": 7
-    },
-    {
-        "id": 51,
+        "id": 48,
         "level": 2,
-        "name_kr": "\ub808\uc800/\ucde8\ubbf8\uc815\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
+        "name_kr": "\uc2dc\uc124\uc6b4\uc601",
         "pid": 7
     },
     {
-        "id": 48,
+        "id": 49,
         "level": 2,
-        "name_kr": "\uc2dc\uc124\uc6b4\uc601",
+        "name_kr": "\uac15\uc2b5/\ud504\ub85c\uadf8\ub7a8",
         "pid": 7
     },
     {
         "id": 50,
         "level": 2,
         "name_kr": "\uc6a9\ud488\ud310\ub9e4/\uc784\ub300",
         "pid": 7
     },
     {
-        "id": 57,
+        "id": 51,
         "level": 2,
-        "name_kr": "\uae30\ud0c0\ubb38\ud654/\uc624\ub77d\uc2dc\uc124",
-        "pid": 8
+        "name_kr": "\ub808\uc800/\ucde8\ubbf8\uc815\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
+        "pid": 7
     },
     {
         "id": 52,
         "level": 2,
         "name_kr": "\ubb38\ud654\uc0c1\ud488\ud310\ub9e4/\uc608\ub9e4\uc11c\ube44\uc2a4",
         "pid": 8
     },
     {
-        "id": 54,
+        "id": 53,
         "level": 2,
-        "name_kr": "\uc5f0\uc608\uae30\ud68d/\uc608\uc220\ub2e8\uccb4",
+        "name_kr": "\uc628\ub77c\uc778\uc11c\ube44\uc2a4",
         "pid": 8
     },
     {
-        "id": 53,
+        "id": 54,
         "level": 2,
-        "name_kr": "\uc628\ub77c\uc778\uc11c\ube44\uc2a4",
+        "name_kr": "\uc5f0\uc608\uae30\ud68d/\uc608\uc220\ub2e8\uccb4",
         "pid": 8
     },
     {
         "id": 55,
         "level": 2,
         "name_kr": "\ucd9c\ud310\uc0ac",
         "pid": 8
@@ -332,35 +320,41 @@
     {
         "id": 56,
         "level": 2,
         "name_kr": "\ud64d\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
         "pid": 8
     },
     {
+        "id": 57,
+        "level": 2,
+        "name_kr": "\uae30\ud0c0\ubb38\ud654/\uc624\ub77d\uc2dc\uc124",
+        "pid": 8
+    },
+    {
         "id": 58,
         "level": 2,
         "name_kr": "\uacf5\uc778\uc911\uac1c",
         "pid": 9
     },
     {
-        "id": 61,
+        "id": 59,
         "level": 2,
-        "name_kr": "\ubd80\ub3d9\uc0b0\uc815\ubcf4\ud3ec\ud138",
+        "name_kr": "\uc784\ub300",
         "pid": 9
     },
     {
         "id": 60,
         "level": 2,
         "name_kr": "\ubd84\uc591",
         "pid": 9
     },
     {
-        "id": 59,
+        "id": 61,
         "level": 2,
-        "name_kr": "\uc784\ub300",
+        "name_kr": "\ubd80\ub3d9\uc0b0\uc815\ubcf4\ud3ec\ud138",
         "pid": 9
     },
     {
         "id": 62,
         "level": 2,
         "name_kr": "\ubd80\ud488\ud310\ub9e4",
         "pid": 10
@@ -368,23 +362,23 @@
     {
         "id": 63,
         "level": 2,
         "name_kr": "\uc0b0\uc5c5\uae30\uae30\ud310\ub9e4",
         "pid": 10
     },
     {
-        "id": 65,
+        "id": 64,
         "level": 2,
-        "name_kr": "\uc131\uc778\uc6a9\ud488\ud310\ub9e4",
+        "name_kr": "\uc131\uc778\ucf58\ud150\uce20",
         "pid": 11
     },
     {
-        "id": 64,
+        "id": 65,
         "level": 2,
-        "name_kr": "\uc131\uc778\ucf58\ud150\uce20",
+        "name_kr": "\uc131\uc778\uc6a9\ud488\ud310\ub9e4",
         "pid": 11
     },
     {
         "id": 66,
         "level": 2,
         "name_kr": "\uc5ed\ud560\ub300\ud589/\ucc44\ud305",
         "pid": 11
@@ -398,114 +392,114 @@
     {
         "id": 68,
         "level": 2,
         "name_kr": "\uc720\ud765\uc5c5\uc18c\uad6c\uc778\uad6c\uc9c1",
         "pid": 11
     },
     {
-        "id": 71,
+        "id": 69,
         "level": 2,
-        "name_kr": "\uc2dd\ub2f9/\ucd9c\uc7a5\uc694\ub9ac/\uc74c\uc2dd\ubc30\ub2ec",
+        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\uc790\uc7ac\uc81c\uc870/\ud310\ub9e4",
         "pid": 12
     },
     {
-        "id": 72,
+        "id": 70,
         "level": 2,
-        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\ube0c\ub79c\ub4dc\ud648\ud398\uc774\uc9c0",
+        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\ud310\ub9e4",
         "pid": 12
     },
     {
-        "id": 69,
+        "id": 71,
         "level": 2,
-        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\uc790\uc7ac\uc81c\uc870/\ud310\ub9e4",
+        "name_kr": "\uc2dd\ub2f9/\ucd9c\uc7a5\uc694\ub9ac/\uc74c\uc2dd\ubc30\ub2ec",
         "pid": 12
     },
     {
-        "id": 70,
+        "id": 72,
         "level": 2,
-        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\ud310\ub9e4",
+        "name_kr": "\uc2dd\ud488/\uc74c\ub8cc\ube0c\ub79c\ub4dc\ud648\ud398\uc774\uc9c0",
         "pid": 12
     },
     {
         "id": 73,
         "level": 2,
         "name_kr": "\uc219\ubc15\uc2dc\uc124",
         "pid": 13
     },
     {
-        "id": 75,
+        "id": 74,
         "level": 2,
-        "name_kr": "\uc5ec\ud589/\uad50\ud1b5\uc815\ubcf4",
+        "name_kr": "\uc5ec\ud589\uc0ac",
         "pid": 13
     },
     {
-        "id": 74,
+        "id": 75,
         "level": 2,
-        "name_kr": "\uc5ec\ud589\uc0ac",
+        "name_kr": "\uc5ec\ud589/\uad50\ud1b5\uc815\ubcf4",
         "pid": 13
     },
     {
-        "id": 77,
+        "id": 76,
         "level": 2,
-        "name_kr": "\uac00\uaca9\ube44\uad50/\uc0c1\ud488\uc815\ubcf4",
+        "name_kr": "\uc911\uc18c\ud615\uc885\ud569\uc1fc\ud551\ubab0",
         "pid": 14
     },
     {
-        "id": 347,
+        "id": 77,
         "level": 2,
-        "name_kr": "\ub300\ud615\uc885\ud569\uc1fc\ud551\ubab0",
+        "name_kr": "\uac00\uaca9\ube44\uad50/\uc0c1\ud488\uc815\ubcf4",
         "pid": 14
     },
     {
-        "id": 76,
+        "id": 78,
         "level": 2,
-        "name_kr": "\uc911\uc18c\ud615\uc885\ud569\uc1fc\ud551\ubab0",
-        "pid": 14
+        "name_kr": "\uc758\ub958/\ud328\uc158\uc7a1\ud654\ud310\ub9e4",
+        "pid": 15
     },
     {
         "id": 79,
         "level": 2,
         "name_kr": "\uc6d0\ub2e8/\ud328\ube0c\ub9ad/\ubd80\uc790\uc7ac\ud310\ub9e4",
         "pid": 15
     },
     {
         "id": 80,
         "level": 2,
         "name_kr": "\uc758\ub958/\uc7a1\ud654\uc218\uc120",
         "pid": 15
     },
     {
-        "id": 78,
+        "id": 81,
         "level": 2,
-        "name_kr": "\uc758\ub958/\ud328\uc158\uc7a1\ud654\ud310\ub9e4",
-        "pid": 15
+        "name_kr": "\uc778\uc1c4\uc18c",
+        "pid": 16
     },
     {
-        "id": 84,
+        "id": 82,
         "level": 2,
-        "name_kr": "\ub9de\ucda4/\ud310\ucd09\uc6a9\ud488\uc81c\uc791/\ud310\ub9e4",
+        "name_kr": "\uc0ac\ubb34\uae30\uae30",
         "pid": 16
     },
     {
         "id": 83,
         "level": 2,
         "name_kr": "\ubb38\uad6c/\uc0ac\ubb34\uc6a9\ud488",
         "pid": 16
     },
     {
-        "id": 82,
+        "id": 84,
         "level": 2,
-        "name_kr": "\uc0ac\ubb34\uae30\uae30",
+        "name_kr": "\ub9de\ucda4/\ud310\ucd09\uc6a9\ud488\uc81c\uc791/\ud310\ub9e4",
         "pid": 16
     },
     {
-        "id": 81,
+        "id": 85,
         "level": 2,
-        "name_kr": "\uc778\uc1c4\uc18c",
-        "pid": 16
+        "name_kr": "\ud310\ub9e4/\ub9ac\uc2a4",
+        "pid": 17
     },
     {
         "id": 86,
         "level": 2,
         "name_kr": "\ub80c\ud130\uce74",
         "pid": 17
     },
@@ -518,65 +512,65 @@
     {
         "id": 88,
         "level": 2,
         "name_kr": "\uc790\ub3d9\ucc28\uc815\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
         "pid": 17
     },
     {
-        "id": 85,
+        "id": 89,
         "level": 2,
-        "name_kr": "\ud310\ub9e4/\ub9ac\uc2a4",
-        "pid": 17
+        "name_kr": "\uac74\ucd95/\uc124\uacc4/\ud1a0\ubaa9",
+        "pid": 376
     },
     {
         "id": 90,
         "level": 2,
         "name_kr": "\uacbd\uc601/\uae08\uc735\ucee8\uc124\ud305",
         "pid": 18
     },
     {
-        "id": 92,
+        "id": 91,
         "level": 2,
-        "name_kr": "\uad11\uace0/\ud64d\ubcf4",
+        "name_kr": "\ucc3d\uc5c5",
         "pid": 18
     },
     {
-        "id": 97,
+        "id": 92,
         "level": 2,
-        "name_kr": "\uae30\ud0c0\uc11c\ube44\uc2a4",
+        "name_kr": "\uad11\uace0/\ud64d\ubcf4",
         "pid": 18
     },
     {
         "id": 93,
         "level": 2,
         "name_kr": "\ub514\uc790\uc778\uc81c\uc791",
         "pid": 18
     },
     {
-        "id": 95,
+        "id": 94,
         "level": 2,
-        "name_kr": "\ubc88\uc5ed/\ud1b5\uc5ed",
+        "name_kr": "\uc601\uc0c1/\uc74c\ud5a5\uc81c\uc791",
         "pid": 18
     },
     {
-        "id": 96,
+        "id": 95,
         "level": 2,
-        "name_kr": "\uc138\ubb34/\ud68c\uacc4/\ubc95\ub960\uc815\ubcf4",
+        "name_kr": "\ubc88\uc5ed/\ud1b5\uc5ed",
         "pid": 18
     },
     {
-        "id": 94,
+        "id": 96,
         "level": 2,
-        "name_kr": "\uc601\uc0c1/\uc74c\ud5a5\uc81c\uc791",
+        "name_kr": "\uc138\ubb34/\ud68c\uacc4/\ubc95\ub960\uc815\ubcf4",
         "pid": 18
     },
     {
-        "id": 91,
+        "id": 97,
         "level": 2,
-        "name_kr": "\ucc3d\uc5c5",
+        "name_kr": "\uae30\ud0c0\uc11c\ube44\uc2a4",
         "pid": 18
     },
     {
         "id": 98,
         "level": 2,
         "name_kr": "\uc0dd\ud65c\uac00\uc804",
         "pid": 19
@@ -590,122 +584,122 @@
     {
         "id": 100,
         "level": 2,
         "name_kr": "\ud2b9\uc218\uc6a9\ub3c4",
         "pid": 19
     },
     {
-        "id": 103,
+        "id": 101,
         "level": 2,
-        "name_kr": "IT\uc218\ub9ac/\uad00\ub9ac\uc11c\ube44\uc2a4",
+        "name_kr": "\ucf58\ud150\uce20\uc11c\ube44\uc2a4",
         "pid": 20
     },
     {
-        "id": 104,
+        "id": 102,
         "level": 2,
-        "name_kr": "IT\uc2dc\uc2a4\ud15c/\uc194\ub8e8\uc158",
+        "name_kr": "\ud1b5\uc2e0\uc11c\ube44\uc2a4\ud310\ub9e4/\ud64d\ubcf4",
         "pid": 20
     },
     {
-        "id": 105,
+        "id": 103,
         "level": 2,
-        "name_kr": "\uc6f9\ud638\uc2a4\ud305/\uc0ac\uc774\ud2b8\uc81c\uc791",
+        "name_kr": "IT\uc218\ub9ac/\uad00\ub9ac\uc11c\ube44\uc2a4",
         "pid": 20
     },
     {
-        "id": 101,
+        "id": 104,
         "level": 2,
-        "name_kr": "\ucf58\ud150\uce20\uc11c\ube44\uc2a4",
+        "name_kr": "IT\uc2dc\uc2a4\ud15c/\uc194\ub8e8\uc158",
         "pid": 20
     },
     {
-        "id": 102,
+        "id": 105,
         "level": 2,
-        "name_kr": "\ud1b5\uc2e0\uc11c\ube44\uc2a4\ud310\ub9e4/\ud64d\ubcf4",
+        "name_kr": "\uc6f9\ud638\uc2a4\ud305/\uc0ac\uc774\ud2b8\uc81c\uc791",
         "pid": 20
     },
     {
+        "id": 119,
+        "level": 3,
+        "name_kr": "\uac00\uad6c\ud310\ub9e4/\uc784\ub300",
+        "pid": 23
+    },
+    {
         "id": 120,
         "level": 3,
         "name_kr": "\uac00\uad6c\uc218\ub9ac/\ub9ac\ud3fc",
         "pid": 23
     },
     {
-        "id": 119,
+        "id": 121,
         "level": 3,
-        "name_kr": "\uac00\uad6c\ud310\ub9e4/\uc784\ub300",
-        "pid": 23
+        "name_kr": "\uc2a4\ud29c\ub514\uc624/\uc0ac\uc9c4\uad00",
+        "pid": 24
     },
     {
-        "id": 127,
+        "id": 122,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc0dd\ud65c\uc11c\ube44\uc2a4",
+        "name_kr": "\uc6b4\uc138/\uc0ac\uc8fc/\uc791\uba85",
         "pid": 24
     },
     {
         "id": 123,
         "level": 3,
         "name_kr": "\ub300\ub9ac\uc6b4\uc804",
         "pid": 24
     },
     {
-        "id": 126,
+        "id": 124,
         "level": 3,
-        "name_kr": "\uc0dd\ud65c\uc815\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
+        "name_kr": "\uc7a5\ub840/\uc0c1\uc870",
         "pid": 24
     },
     {
         "id": 125,
         "level": 3,
         "name_kr": "\uc138\ud0c1/\uccad\uc18c",
         "pid": 24
     },
     {
-        "id": 121,
+        "id": 126,
         "level": 3,
-        "name_kr": "\uc2a4\ud29c\ub514\uc624/\uc0ac\uc9c4\uad00",
+        "name_kr": "\uc0dd\ud65c\uc815\ubcf4/\ucee4\ubba4\ub2c8\ud2f0",
         "pid": 24
     },
     {
-        "id": 122,
+        "id": 127,
         "level": 3,
-        "name_kr": "\uc6b4\uc138/\uc0ac\uc8fc/\uc791\uba85",
+        "name_kr": "\uae30\ud0c0\uc0dd\ud65c\uc11c\ube44\uc2a4",
         "pid": 24
     },
     {
-        "id": 124,
+        "id": 128,
         "level": 3,
-        "name_kr": "\uc7a5\ub840/\uc0c1\uc870",
-        "pid": 24
+        "name_kr": "\uc0dd\ud65c\uc6a9\ud488\ud310\ub9e4",
+        "pid": 25
     },
     {
         "id": 129,
         "level": 3,
         "name_kr": "\uc0dd\ud65c\uc6a9\ud488\uc81c\uc870/B2B\ud310\ub9e4",
         "pid": 25
     },
     {
-        "id": 128,
+        "id": 130,
         "level": 3,
-        "name_kr": "\uc0dd\ud65c\uc6a9\ud488\ud310\ub9e4",
-        "pid": 25
+        "name_kr": "\uc560\uc644\ub3d9\ubb3c/\uc6a9\ud488",
+        "pid": 26
     },
     {
         "id": 131,
         "level": 3,
         "name_kr": "\ub3d9\ubb3c\ubcd1\uc6d0",
         "pid": 26
     },
     {
-        "id": 130,
-        "level": 3,
-        "name_kr": "\uc560\uc644\ub3d9\ubb3c/\uc6a9\ud488",
-        "pid": 26
-    },
-    {
         "id": 132,
         "level": 3,
         "name_kr": "\uc2b9\uac1d\uc6b4\uc1a1",
         "pid": 27
     },
     {
         "id": 133,
@@ -722,53 +716,47 @@
     {
         "id": 135,
         "level": 3,
         "name_kr": "\uc778\ud14c\ub9ac\uc5b4\uc18c\ud488",
         "pid": 28
     },
     {
-        "id": 148,
-        "level": 3,
-        "name_kr": "\uae30\ud0c0\uc77c\ubc18\uc758\uc6d0",
-        "pid": 30
-    },
-    {
-        "id": 142,
+        "id": 137,
         "level": 3,
-        "name_kr": "\ub0b4\uacfc/\uc774\ube44\uc778\ud6c4\uacfc",
+        "name_kr": "\ubcd1\uc6d0/\uac74\uac15\uc815\ubcf4",
         "pid": 30
     },
     {
-        "id": 149,
+        "id": 138,
         "level": 3,
-        "name_kr": "\ub300\uccb4\uc758\ud559",
+        "name_kr": "\uc77c\ubc18/\uc885\ud569\ubcd1\uc6d0",
         "pid": 30
     },
     {
-        "id": 137,
+        "id": 139,
         "level": 3,
-        "name_kr": "\ubcd1\uc6d0/\uac74\uac15\uc815\ubcf4",
+        "name_kr": "\uce58\uacfc/\uce58\uacfc\ubcd1\uc6d0",
         "pid": 30
     },
     {
-        "id": 145,
+        "id": 140,
         "level": 3,
-        "name_kr": "\ube44\ub1e8\uae30\uacfc",
+        "name_kr": "\ud55c\uc758\uc6d0/\ud55c\ubc29\ubcd1\uc6d0",
         "pid": 30
     },
     {
-        "id": 146,
+        "id": 141,
         "level": 3,
-        "name_kr": "\uc0b0\ubd80\uc778\uacfc",
+        "name_kr": "\uc131\ud615\uc678\uacfc/\ud53c\ubd80\uacfc",
         "pid": 30
     },
     {
-        "id": 141,
+        "id": 142,
         "level": 3,
-        "name_kr": "\uc131\ud615\uc678\uacfc/\ud53c\ubd80\uacfc",
+        "name_kr": "\ub0b4\uacfc/\uc774\ube44\uc778\ud6c4\uacfc",
         "pid": 30
     },
     {
         "id": 143,
         "level": 3,
         "name_kr": "\uc548\uacfc",
         "pid": 30
@@ -776,47 +764,47 @@
     {
         "id": 144,
         "level": 3,
         "name_kr": "\uc678\uacfc",
         "pid": 30
     },
     {
-        "id": 138,
+        "id": 145,
         "level": 3,
-        "name_kr": "\uc77c\ubc18/\uc885\ud569\ubcd1\uc6d0",
+        "name_kr": "\ube44\ub1e8\uae30\uacfc",
         "pid": 30
     },
     {
-        "id": 150,
+        "id": 146,
         "level": 3,
-        "name_kr": "\uc7ac\ud65c\uc804\ubb38\uae30\uad00",
+        "name_kr": "\uc0b0\ubd80\uc778\uacfc",
         "pid": 30
     },
     {
         "id": 147,
         "level": 3,
         "name_kr": "\uc815\uc2e0\uacfc",
         "pid": 30
     },
     {
-        "id": 139,
+        "id": 148,
         "level": 3,
-        "name_kr": "\uce58\uacfc/\uce58\uacfc\ubcd1\uc6d0",
+        "name_kr": "\uae30\ud0c0\uc77c\ubc18\uc758\uc6d0",
         "pid": 30
     },
     {
-        "id": 341,
+        "id": 149,
         "level": 3,
-        "name_kr": "\ud074\ub9ac\ub2c9",
+        "name_kr": "\ub300\uccb4\uc758\ud559",
         "pid": 30
     },
     {
-        "id": 140,
+        "id": 150,
         "level": 3,
-        "name_kr": "\ud55c\uc758\uc6d0/\ud55c\ubc29\ubcd1\uc6d0",
+        "name_kr": "\uc7ac\ud65c\uc804\ubb38\uae30\uad00",
         "pid": 30
     },
     {
         "id": 151,
         "level": 3,
         "name_kr": "\uac74\uac15/\ubbf8\uc6a9\uad00\ub9ac",
         "pid": 33
@@ -830,23 +818,23 @@
     {
         "id": 153,
         "level": 3,
         "name_kr": "\uc6e8\ub529\uc0c1\ud488",
         "pid": 35
     },
     {
-        "id": 155,
+        "id": 154,
         "level": 3,
-        "name_kr": "\uc6e8\ub529\uc815\ubcf4\ud3ec\ud138",
+        "name_kr": "\uc6e8\ub529\ucee8\uc124\ud305",
         "pid": 35
     },
     {
-        "id": 154,
+        "id": 155,
         "level": 3,
-        "name_kr": "\uc6e8\ub529\ucee8\uc124\ud305",
+        "name_kr": "\uc6e8\ub529\uc815\ubcf4\ud3ec\ud138",
         "pid": 35
     },
     {
         "id": 156,
         "level": 3,
         "name_kr": "\ucd9c\uc0b0/\uc720\uc544\ub3d9\uc6a9\ud488\uc804\ubb38\ud310\ub9e4",
         "pid": 36
@@ -854,95 +842,89 @@
     {
         "id": 157,
         "level": 3,
         "name_kr": "\ucd9c\uc0b0/\uc720\uc544\ub3d9\uc6a9\ud488\uc81c\uc870/B2B\ud310\ub9e4",
         "pid": 36
     },
     {
-        "id": 159,
+        "id": 158,
         "level": 3,
-        "name_kr": "\ubcf4\uc721/\ud0c1\uc544",
+        "name_kr": "\ucd9c\uc0b0\uc900\ube44/\uc0b0\ud6c4\uc870\ub9ac",
         "pid": 37
     },
     {
-        "id": 160,
+        "id": 159,
         "level": 3,
-        "name_kr": "\uc81c\ub300\ud608\uc740\ud589",
+        "name_kr": "\ubcf4\uc721/\ud0c1\uc544",
         "pid": 37
     },
     {
-        "id": 158,
+        "id": 160,
         "level": 3,
-        "name_kr": "\ucd9c\uc0b0\uc900\ube44/\uc0b0\ud6c4\uc870\ub9ac",
+        "name_kr": "\uc81c\ub300\ud608\uc740\ud589",
         "pid": 37
     },
     {
-        "id": 163,
-        "level": 3,
-        "name_kr": "\uace0\ub4f1\uad50\uc721\uae30\uad00",
-        "pid": 38
-    },
-    {
         "id": 161,
         "level": 3,
         "name_kr": "\uc720\uc544\uad50\uc721\uae30\uad00",
         "pid": 38
     },
     {
         "id": 162,
         "level": 3,
         "name_kr": "\ucd08/\uc911/\uace0\ub4f1\ud559\uad50",
         "pid": 38
     },
     {
-        "id": 384,
+        "id": 163,
         "level": 3,
-        "name_kr": "\ud3c9\uc0dd\uad50\uc721\uae30\uad00",
+        "name_kr": "\uace0\ub4f1\uad50\uc721\uae30\uad00",
         "pid": 38
     },
     {
-        "id": 167,
+        "id": 164,
         "level": 3,
-        "name_kr": "\uace0\uc2dc\ud559\uc6d0",
+        "name_kr": "\uc218\ub2a5/\uc785\uc2dc\ud559\uc6d0",
         "pid": 39
     },
     {
-        "id": 170,
+        "id": 165,
         "level": 3,
-        "name_kr": "\uacfc\uc678/\ud559\uc2b5\uc9c0/\ud648\uc2a4\ud130\ub514",
+        "name_kr": "\uc77c\ubc18\ud559\uc2b5\ud559\uc6d0",
         "pid": 39
     },
     {
-        "id": 164,
+        "id": 166,
         "level": 3,
-        "name_kr": "\uc218\ub2a5/\uc785\uc2dc\ud559\uc6d0",
+        "name_kr": "\uc5b4\ud559\uc6d0",
         "pid": 39
     },
     {
-        "id": 166,
+        "id": 167,
         "level": 3,
-        "name_kr": "\uc5b4\ud559\uc6d0",
+        "name_kr": "\uace0\uc2dc\ud559\uc6d0",
         "pid": 39
     },
     {
         "id": 168,
         "level": 3,
         "name_kr": "\uc6b4\uc804\ud559\uc6d0",
         "pid": 39
     },
     {
-        "id": 165,
+        "id": 169,
         "level": 3,
-        "name_kr": "\uc77c\ubc18\ud559\uc2b5\ud559\uc6d0",
+        "name_kr": "\uc790\uaca9\uc99d/\uae30\uc220/\uae30\ud0c0",
         "pid": 39
     },
     {
-        "id": 169,
+        "id": 170,
         "level": 3,
-        "name_kr": "\uc790\uaca9\uc99d/\uae30\uc220/\uae30\ud0c0",
+        "name_kr": "\uacfc\uc678/\ud559\uc2b5\uc9c0/\ud648\uc2a4\ud130\ub514",
         "pid": 39
     },
     {
         "id": 171,
         "level": 3,
         "name_kr": "\uad50\uc721\uc815\ubcf4",
         "pid": 40
@@ -962,42 +944,30 @@
     {
         "id": 174,
         "level": 3,
         "name_kr": "\uc720\ud559/\uc5f0\uc218\uc9c0\uc6d0",
         "pid": 41
     },
     {
-        "id": 177,
-        "level": 3,
-        "name_kr": "\uc2e0\uc6a9\ud3c9\uac00/\uc870\uc0ac\uae30\uad00",
-        "pid": 43
-    },
-    {
         "id": 175,
         "level": 3,
         "name_kr": "\uc81c1\uae08\uc735\uad8c\uae30\uad00",
         "pid": 43
     },
     {
         "id": 176,
         "level": 3,
         "name_kr": "\uc81c2\uae08\uc735\uad8c\uae30\uad00",
         "pid": 43
     },
     {
-        "id": 363,
-        "level": 3,
-        "name_kr": "\ub300\ucd9c\uc911\uac1c/\uac00\uaca9\ube44\uad50",
-        "pid": 44
-    },
-    {
-        "id": 181,
+        "id": 177,
         "level": 3,
-        "name_kr": "\ubcf4\ud5d8\ud310\ub9e4",
-        "pid": 44
+        "name_kr": "\uc2e0\uc6a9\ud3c9\uac00/\uc870\uc0ac\uae30\uad00",
+        "pid": 43
     },
     {
         "id": 178,
         "level": 3,
         "name_kr": "\uc81c1\uae08\uc735\uad8c\ub300\ucd9c",
         "pid": 44
     },
@@ -1010,14 +980,20 @@
     {
         "id": 180,
         "level": 3,
         "name_kr": "\uc81c3\uae08\uc735\uad8c\ub300\ucd9c",
         "pid": 44
     },
     {
+        "id": 181,
+        "level": 3,
+        "name_kr": "\ubcf4\ud5d8\ud310\ub9e4",
+        "pid": 44
+    },
+    {
         "id": 182,
         "level": 3,
         "name_kr": "\uce74\ub4dc/\ud3ec\uc778\ud2b8\uc0c1\ub2f4",
         "pid": 44
     },
     {
         "id": 183,
@@ -1028,29 +1004,23 @@
     {
         "id": 184,
         "level": 3,
         "name_kr": "\uc870\ud654/\uc6d0\uc608",
         "pid": 46
     },
     {
-        "id": 360,
-        "level": 3,
-        "name_kr": "\uc774\ubca4\ud2b8\uae30\ud68d",
-        "pid": 47
-    },
-    {
         "id": 185,
         "level": 3,
         "name_kr": "\uc774\ubca4\ud2b8\uc18c\ud488/\uc120\ubb3c\uc6a9\ud488",
         "pid": 47
     },
     {
-        "id": 189,
+        "id": 186,
         "level": 3,
-        "name_kr": "\ub3c4\ubc15/\ubcf5\uad8c",
+        "name_kr": "\uccb4\ub825\ub2e8\ub828\uc2dc\uc124",
         "pid": 48
     },
     {
         "id": 187,
         "level": 3,
         "name_kr": "\ub808\uc800\uc2a4\ud3ec\uce20\uc2dc\uc124",
         "pid": 48
@@ -1058,98 +1028,92 @@
     {
         "id": 188,
         "level": 3,
         "name_kr": "\ubb38\ud654/\ucde8\ubbf8\uc2dc\uc124",
         "pid": 48
     },
     {
-        "id": 186,
+        "id": 189,
         "level": 3,
-        "name_kr": "\uccb4\ub825\ub2e8\ub828\uc2dc\uc124",
+        "name_kr": "\ub3c4\ubc15/\ubcf5\uad8c",
         "pid": 48
     },
     {
         "id": 190,
         "level": 3,
         "name_kr": "\uace8\ud504\uac15\uc2b5",
         "pid": 49
     },
     {
-        "id": 193,
-        "level": 3,
-        "name_kr": "\uae30\ud0c0\uc2a4\ud3ec\uce20\uac15\uc2b5",
-        "pid": 49
-    },
-    {
         "id": 191,
         "level": 3,
         "name_kr": "\uc218\uc0c1\uc2a4\ud3ec\uce20\uac15\uc2b5",
         "pid": 49
     },
     {
         "id": 192,
         "level": 3,
         "name_kr": "\uc2a4\ud0a4/\ubcf4\ub4dc\uac15\uc2b5",
         "pid": 49
     },
     {
+        "id": 193,
+        "level": 3,
+        "name_kr": "\uae30\ud0c0\uc2a4\ud3ec\uce20\uac15\uc2b5",
+        "pid": 49
+    },
+    {
         "id": 194,
         "level": 3,
         "name_kr": "\ucde8\ubbf8\uac15\uc2b5",
         "pid": 49
     },
     {
         "id": 195,
         "level": 3,
         "name_kr": "\ucea0\ud504",
         "pid": 49
     },
     {
-        "id": 200,
+        "id": 196,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc6a9\ud488\ud310\ub9e4",
+        "name_kr": "\ub808\uc800\uc2a4\ud3ec\uce20\uc6a9\ud488",
         "pid": 50
     },
     {
-        "id": 196,
+        "id": 197,
         "level": 3,
-        "name_kr": "\ub808\uc800\uc2a4\ud3ec\uce20\uc6a9\ud488",
+        "name_kr": "\ucde8\ubbf8/\uc608\uc220\uc6a9\ud488",
         "pid": 50
     },
     {
         "id": 198,
         "level": 3,
         "name_kr": "\uc545\uae30",
         "pid": 50
     },
     {
-        "id": 197,
+        "id": 199,
         "level": 3,
-        "name_kr": "\ucde8\ubbf8/\uc608\uc220\uc6a9\ud488",
+        "name_kr": "\ud0a4\ub35c\ud2b8/\uc644\uad6c",
         "pid": 50
     },
     {
-        "id": 199,
+        "id": 200,
         "level": 3,
-        "name_kr": "\ud0a4\ub35c\ud2b8/\uc644\uad6c",
+        "name_kr": "\uae30\ud0c0\uc6a9\ud488\ud310\ub9e4",
         "pid": 50
     },
     {
         "id": 201,
         "level": 3,
         "name_kr": "\uc5f0\uc608\uae30\ud68d\uc0ac",
         "pid": 54
     },
     {
-        "id": 361,
-        "level": 3,
-        "name_kr": "\uc608\uc220/\uacf5\uc5f0\ub2e8\uccb4",
-        "pid": 54
-    },
-    {
         "id": 203,
         "level": 3,
         "name_kr": "\uad6d\ub0b4",
         "pid": 58
     },
     {
         "id": 204,
@@ -1166,20 +1130,14 @@
     {
         "id": 206,
         "level": 3,
         "name_kr": "\uacfc\ud559\uae30\uae30",
         "pid": 63
     },
     {
-        "id": 210,
-        "level": 3,
-        "name_kr": "\uae30\ud0c0\uae30\uae30",
-        "pid": 63
-    },
-    {
         "id": 207,
         "level": 3,
         "name_kr": "\uc601\uc0c1/\uc74c\ud5a5\uc7a5\ube44",
         "pid": 63
     },
     {
         "id": 208,
@@ -1190,150 +1148,138 @@
     {
         "id": 209,
         "level": 3,
         "name_kr": "\ud658\uacbd\uae30\uae30",
         "pid": 63
     },
     {
-        "id": 212,
+        "id": 210,
         "level": 3,
-        "name_kr": "\uac00\uacf5\uc2dd\ud488/\uae30\ud0c0",
-        "pid": 70
+        "name_kr": "\uae30\ud0c0\uae30\uae30",
+        "pid": 63
     },
     {
         "id": 211,
         "level": 3,
         "name_kr": "\ub18d\uc218\uc0b0/\ucd95\uc0b0\ubb3c",
         "pid": 70
     },
     {
-        "id": 218,
+        "id": 212,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc2dd\ub2f9",
+        "name_kr": "\uac00\uacf5\uc2dd\ud488/\uae30\ud0c0",
+        "pid": 70
+    },
+    {
+        "id": 213,
+        "level": 3,
+        "name_kr": "\ucd9c\uc7a5\uc694\ub9ac\uc804\ubb38",
         "pid": 71
     },
     {
-        "id": 217,
+        "id": 214,
         "level": 3,
-        "name_kr": "\uc591\uc2dd\ub2f9",
+        "name_kr": "\ud55c\uc2dd\ub2f9",
         "pid": 71
     },
     {
-        "id": 216,
+        "id": 215,
         "level": 3,
-        "name_kr": "\uc77c\uc2dd\ub2f9",
+        "name_kr": "\uc911\uc2dd\ub2f9",
         "pid": 71
     },
     {
-        "id": 220,
+        "id": 216,
         "level": 3,
-        "name_kr": "\uc8fc\uc810",
+        "name_kr": "\uc77c\uc2dd\ub2f9",
         "pid": 71
     },
     {
-        "id": 215,
+        "id": 217,
         "level": 3,
-        "name_kr": "\uc911\uc2dd\ub2f9",
+        "name_kr": "\uc591\uc2dd\ub2f9",
         "pid": 71
     },
     {
-        "id": 213,
+        "id": 218,
         "level": 3,
-        "name_kr": "\ucd9c\uc7a5\uc694\ub9ac\uc804\ubb38",
+        "name_kr": "\uae30\ud0c0\uc2dd\ub2f9",
         "pid": 71
     },
     {
         "id": 219,
         "level": 3,
         "name_kr": "\uce74\ud398",
         "pid": 71
     },
     {
-        "id": 214,
+        "id": 220,
         "level": 3,
-        "name_kr": "\ud55c\uc2dd\ub2f9",
+        "name_kr": "\uc8fc\uc810",
         "pid": 71
     },
     {
+        "id": 221,
+        "level": 3,
+        "name_kr": "\ucf58\ub3c4/\ub9ac\uc870\ud2b8",
+        "pid": 73
+    },
+    {
         "id": 222,
         "level": 3,
         "name_kr": "\uad6d\ub0b4\ubbfc\ubc15",
         "pid": 73
     },
     {
         "id": 223,
         "level": 3,
         "name_kr": "\uad6d\uc678\ubbfc\ubc15",
         "pid": 73
     },
     {
-        "id": 228,
+        "id": 224,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc219\ubc15\uc2dc\uc124",
+        "name_kr": "\ud638\ud154/\ub808\uc9c0\ub358\uc2a4",
         "pid": 73
     },
     {
         "id": 225,
         "level": 3,
         "name_kr": "\uc218\ub828\uc2dc\uc124",
         "pid": 73
     },
     {
-        "id": 362,
-        "level": 3,
-        "name_kr": "\uc219\ubc15\uc911\uac1c/\uc608\uc57d\ub300\ud589",
-        "pid": 73
-    },
-    {
         "id": 226,
         "level": 3,
         "name_kr": "\uc5ec\uad00",
         "pid": 73
     },
     {
-        "id": 221,
-        "level": 3,
-        "name_kr": "\ucf58\ub3c4/\ub9ac\uc870\ud2b8",
-        "pid": 73
-    },
-    {
         "id": 227,
         "level": 3,
         "name_kr": "\ud39c\uc158",
         "pid": 73
     },
     {
-        "id": 224,
+        "id": 228,
         "level": 3,
-        "name_kr": "\ud638\ud154/\ub808\uc9c0\ub358\uc2a4",
+        "name_kr": "\uae30\ud0c0\uc219\ubc15\uc2dc\uc124",
         "pid": 73
     },
     {
-        "id": 230,
-        "level": 3,
-        "name_kr": "\uad50\ud1b5\uc608\uc57d\ub300\ud589",
-        "pid": 75
-    },
-    {
         "id": 229,
         "level": 3,
         "name_kr": "\uc5ec\ud589/\uad50\ud1b5\uc815\ubcf4",
         "pid": 75
     },
     {
-        "id": 349,
-        "level": 3,
-        "name_kr": "\uad6c\ub9e4\ub300\ud589\uc885\ud569\uc1fc\ud551\ubab0",
-        "pid": 76
-    },
-    {
-        "id": 348,
+        "id": 230,
         "level": 3,
-        "name_kr": "\uc77c\ubc18\uc911\uc18c\ud615\uc885\ud569\uc1fc\ud551\ubab0",
-        "pid": 76
+        "name_kr": "\uad50\ud1b5\uc608\uc57d\ub300\ud589",
+        "pid": 75
     },
     {
         "id": 231,
         "level": 3,
         "name_kr": "\uc758\ub958/\ud328\uc158\uc7a1\ud654\ube0c\ub79c\ub4dc",
         "pid": 78
     },
@@ -1346,41 +1292,41 @@
     {
         "id": 233,
         "level": 3,
         "name_kr": "\uc804\ubb38/\ud2b9\uc218\uc758\ub958",
         "pid": 78
     },
     {
-        "id": 235,
+        "id": 234,
         "level": 3,
-        "name_kr": "\ub80c\ud0c8\uc804\ubb38",
+        "name_kr": "\ud310\ub9e4",
         "pid": 82
     },
     {
-        "id": 234,
+        "id": 235,
         "level": 3,
-        "name_kr": "\ud310\ub9e4",
+        "name_kr": "\ub80c\ud0c8\uc804\ubb38",
         "pid": 82
     },
     {
         "id": 236,
         "level": 3,
         "name_kr": "\uc2e0\uaddc",
         "pid": 85
     },
     {
-        "id": 238,
+        "id": 237,
         "level": 3,
-        "name_kr": "\uc624\ud1a0\ub9ac\uc2a4\uc804\ubb38",
+        "name_kr": "\uc911\uace0",
         "pid": 85
     },
     {
-        "id": 237,
+        "id": 238,
         "level": 3,
-        "name_kr": "\uc911\uace0",
+        "name_kr": "\uc624\ud1a0\ub9ac\uc2a4\uc804\ubb38",
         "pid": 85
     },
     {
         "id": 239,
         "level": 3,
         "name_kr": "\uc790\ub3d9\ucc28\uc6a9\ud488\ud310\ub9e4",
         "pid": 87
@@ -1424,47 +1370,41 @@
     {
         "id": 246,
         "level": 3,
         "name_kr": "\ucc3d\uc5c5\ucee8\uc124\ud305",
         "pid": 91
     },
     {
-        "id": 381,
-        "level": 3,
-        "name_kr": "\ud504\ub79c\ucc28\uc774\uc988",
-        "pid": 91
-    },
-    {
         "id": 247,
         "level": 3,
         "name_kr": "\uad11\uace0\ub300\ud589/\uc81c\uc791",
         "pid": 92
     },
     {
-        "id": 251,
+        "id": 248,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uad11\uace0/\ud64d\ubcf4",
+        "name_kr": "\uc628\ub77c\uc778\uad11\uace0",
         "pid": 92
     },
     {
         "id": 249,
         "level": 3,
         "name_kr": "\uc625\uc678\uad11\uace0",
         "pid": 92
     },
     {
-        "id": 248,
+        "id": 250,
         "level": 3,
-        "name_kr": "\uc628\ub77c\uc778\uad11\uace0",
+        "name_kr": "\uc778\uc801\ud310\ub9e4",
         "pid": 92
     },
     {
-        "id": 250,
+        "id": 251,
         "level": 3,
-        "name_kr": "\uc778\uc801\ud310\ub9e4",
+        "name_kr": "\uae30\ud0c0\uad11\uace0/\ud64d\ubcf4",
         "pid": 92
     },
     {
         "id": 252,
         "level": 3,
         "name_kr": "\ubc95\ubb34/\ubc95\ub960",
         "pid": 96
@@ -1472,119 +1412,101 @@
     {
         "id": 253,
         "level": 3,
         "name_kr": "\uc138\ubb34/\ud68c\uacc4",
         "pid": 96
     },
     {
-        "id": 256,
+        "id": 254,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\ub300\ud589\uc11c\ube44\uc2a4",
+        "name_kr": "\uae30\ud0c0\uc81c\uc870/\uc81c\uc791",
         "pid": 97
     },
     {
-        "id": 257,
+        "id": 255,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc804\ubb38\uc11c\ube44\uc2a4",
+        "name_kr": "\uae30\ud0c0\ucee8\uc124\ud305",
         "pid": 97
     },
     {
-        "id": 254,
+        "id": 256,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\uc81c\uc870/\uc81c\uc791",
+        "name_kr": "\uae30\ud0c0\ub300\ud589\uc11c\ube44\uc2a4",
         "pid": 97
     },
     {
-        "id": 255,
+        "id": 257,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\ucee8\uc124\ud305",
+        "name_kr": "\uae30\ud0c0\uc804\ubb38\uc11c\ube44\uc2a4",
         "pid": 97
     },
     {
-        "id": 260,
+        "id": 258,
         "level": 3,
-        "name_kr": "\uae30\ud0c0\ud1b5\uc2e0\uc11c\ube44\uc2a4",
+        "name_kr": "\uc720\uc120\uc11c\ube44\uc2a4",
         "pid": 102
     },
     {
         "id": 259,
         "level": 3,
         "name_kr": "\ubb34\uc120\uc11c\ube44\uc2a4",
         "pid": 102
     },
     {
-        "id": 258,
+        "id": 260,
         "level": 3,
-        "name_kr": "\uc720\uc120\uc11c\ube44\uc2a4",
+        "name_kr": "\uae30\ud0c0\ud1b5\uc2e0\uc11c\ube44\uc2a4",
         "pid": 102
     },
     {
-        "id": 380,
-        "level": 4,
-        "name_kr": "\uc0ac\ubb34/\uc5c5\uc18c\uc6a9\uac00\uad6c",
-        "pid": 119
-    },
-    {
-        "id": 379,
+        "id": 261,
         "level": 4,
-        "name_kr": "\uc77c\ubc18/\uac00\uc815\uc6a9\uac00\uad6c",
-        "pid": 119
+        "name_kr": "\uc560\uc644\ub3d9\ubb3c\ubd84\uc591/\ud310\ub9e4",
+        "pid": 130
     },
     {
         "id": 262,
         "level": 4,
         "name_kr": "\uc560\uc644\ub3d9\ubb3c\uad00\ub828\uc11c\ube44\uc2a4",
         "pid": 130
     },
     {
-        "id": 261,
-        "level": 4,
-        "name_kr": "\uc560\uc644\ub3d9\ubb3c\ubd84\uc591/\ud310\ub9e4",
-        "pid": 130
-    },
-    {
         "id": 263,
         "level": 4,
         "name_kr": "\uc560\uc644\ub3d9\ubb3c\uc6a9\ud488\ud310\ub9e4",
         "pid": 130
     },
     {
         "id": 264,
         "level": 4,
         "name_kr": "\ub178\uc778\ubcd1\uc6d0",
         "pid": 138
     },
     {
-        "id": 393,
-        "level": 4,
-        "name_kr": "\uc694\uc591\uc6d0",
-        "pid": 138
-    },
-    {
         "id": 265,
         "level": 4,
         "name_kr": "\uc77c\ubc18\ubcd1\uc6d0",
         "pid": 138
     },
     {
         "id": 266,
         "level": 4,
         "name_kr": "\uc885\ud569\ubcd1\uc6d0",
         "pid": 138
     },
     {
-        "id": 269,
+        "id": 267,
         "level": 4,
-        "name_kr": "\uc77c\ubc18\uce58\uacfc",
+        "name_kr": "\uce58\uacfc\ubcd1\uc6d0",
         "pid": 139
     },
     {
-        "id": 267,
+        "id": 269,
         "level": 4,
-        "name_kr": "\uce58\uacfc\ubcd1\uc6d0",
+        "name_kr": "\uc77c\ubc18\uce58\uacfc",
         "pid": 139
     },
     {
         "id": 270,
         "level": 4,
         "name_kr": "\ud55c\ubc29\ubcd1\uc6d0",
         "pid": 140
@@ -1592,83 +1514,41 @@
     {
         "id": 271,
         "level": 4,
         "name_kr": "\ud55c\uc758\uc6d0",
         "pid": 140
     },
     {
-        "id": 358,
-        "level": 4,
-        "name_kr": "\uae30\ud0c0\uc77c\ubc18\uc758\uc6d0",
-        "pid": 148
-    },
-    {
-        "id": 359,
-        "level": 4,
-        "name_kr": "\ud63c\ud569\uc758\uc6d0",
-        "pid": 148
-    },
-    {
-        "id": 389,
-        "level": 4,
-        "name_kr": "\uae30\ud0c0 \uace0\ub4f1\uad50\uc721\uae30\uad00",
-        "pid": 163
-    },
-    {
-        "id": 386,
-        "level": 4,
-        "name_kr": "\ub300\ud559\uad50",
-        "pid": 163
-    },
-    {
-        "id": 387,
-        "level": 4,
-        "name_kr": "\ub300\ud559\uc6d0",
-        "pid": 163
-    },
-    {
-        "id": 388,
-        "level": 4,
-        "name_kr": "\uc6d0\uaca9\ub300\ud559\uad50",
-        "pid": 163
-    },
-    {
-        "id": 385,
-        "level": 4,
-        "name_kr": "\uc804\ubb38\ub300\ud559",
-        "pid": 163
-    },
-    {
-        "id": 276,
+        "id": 272,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\uc678\uad6d\uc5b4\ud559\uc6d0",
+        "name_kr": "\uc885\ud569\uc678\uad6d\uc5b4\ud559\uc6d0",
         "pid": 166
     },
     {
         "id": 273,
         "level": 4,
         "name_kr": "\uc601\uc5b4\ud559\uc6d0",
         "pid": 166
     },
     {
-        "id": 275,
+        "id": 274,
         "level": 4,
-        "name_kr": "\uc77c\ubcf8\uc5b4\ud559\uc6d0",
+        "name_kr": "\uc911\uad6d\uc5b4\ud559\uc6d0",
         "pid": 166
     },
     {
-        "id": 272,
+        "id": 275,
         "level": 4,
-        "name_kr": "\uc885\ud569\uc678\uad6d\uc5b4\ud559\uc6d0",
+        "name_kr": "\uc77c\ubcf8\uc5b4\ud559\uc6d0",
         "pid": 166
     },
     {
-        "id": 274,
+        "id": 276,
         "level": 4,
-        "name_kr": "\uc911\uad6d\uc5b4\ud559\uc6d0",
+        "name_kr": "\uae30\ud0c0\uc678\uad6d\uc5b4\ud559\uc6d0",
         "pid": 166
     },
     {
         "id": 277,
         "level": 4,
         "name_kr": "\uac04\ud638\ud559\uc6d0",
         "pid": 169
@@ -1676,20 +1556,14 @@
     {
         "id": 278,
         "level": 4,
         "name_kr": "\uac74\ucd95/\uc778\ud14c\ub9ac\uc5b4\ud559\uc6d0",
         "pid": 169
     },
     {
-        "id": 287,
-        "level": 4,
-        "name_kr": "\uae30\ud0c0\ud559\uc6d0",
-        "pid": 169
-    },
-    {
         "id": 279,
         "level": 4,
         "name_kr": "\ubbf8\uc6a9\ud559\uc6d0",
         "pid": 169
     },
     {
         "id": 280,
@@ -1730,23 +1604,23 @@
     {
         "id": 286,
         "level": 4,
         "name_kr": "\ucef4\ud4e8\ud130\ud559\uc6d0",
         "pid": 169
     },
     {
-        "id": 292,
+        "id": 287,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\uc81c2\uae08\uc735\uad8c",
-        "pid": 176
+        "name_kr": "\uae30\ud0c0\ud559\uc6d0",
+        "pid": 169
     },
     {
-        "id": 291,
+        "id": 288,
         "level": 4,
-        "name_kr": "\ubcf4\ud5d8\uae30\uad00",
+        "name_kr": "\uc99d\uad8c\uae30\uad00",
         "pid": 176
     },
     {
         "id": 289,
         "level": 4,
         "name_kr": "\uc0c1\ud638\uc800\ucd95\uc740\ud589\uae30\uad00",
         "pid": 176
@@ -1754,83 +1628,89 @@
     {
         "id": 290,
         "level": 4,
         "name_kr": "\uc2e0\uc6a9\uce74\ub4dc\uae30\uad00",
         "pid": 176
     },
     {
-        "id": 288,
+        "id": 291,
         "level": 4,
-        "name_kr": "\uc99d\uad8c\uae30\uad00",
+        "name_kr": "\ubcf4\ud5d8\uae30\uad00",
         "pid": 176
     },
     {
-        "id": 295,
+        "id": 292,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\uc81c2\uae08\uc735\uad8c\ub300\ucd9c\uc0c1\ub2f4",
+        "name_kr": "\uae30\ud0c0\uc81c2\uae08\uc735\uad8c",
+        "pid": 176
+    },
+    {
+        "id": 293,
+        "level": 4,
+        "name_kr": "\uc99d\uad8c\ub300\ucd9c\uc0c1\ub2f4",
         "pid": 179
     },
     {
         "id": 294,
         "level": 4,
         "name_kr": "\uc0c1\ud638\uc800\ucd95\uc740\ud589\ub300\ucd9c\uc0c1\ub2f4",
         "pid": 179
     },
     {
-        "id": 293,
+        "id": 295,
         "level": 4,
-        "name_kr": "\uc99d\uad8c\ub300\ucd9c\uc0c1\ub2f4",
+        "name_kr": "\uae30\ud0c0\uc81c2\uae08\uc735\uad8c\ub300\ucd9c\uc0c1\ub2f4",
         "pid": 179
     },
     {
-        "id": 297,
+        "id": 296,
         "level": 4,
-        "name_kr": "\uace8\ud504\uc5f0\uc2b5\uc7a5",
+        "name_kr": "\uc885\ud569\uc2a4\ud3ec\uce20\uc13c\ud130",
         "pid": 186
     },
     {
-        "id": 301,
+        "id": 297,
         "level": 4,
-        "name_kr": "\uae30\uccb4\uc870/\uc218\ub828",
+        "name_kr": "\uace8\ud504\uc5f0\uc2b5\uc7a5",
         "pid": 186
     },
     {
-        "id": 303,
+        "id": 298,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\uccb4\ub825\ub2e8\ub828\uc2dc\uc124",
+        "name_kr": "\uc694\uac00\uc6d0",
         "pid": 186
     },
     {
         "id": 299,
         "level": 4,
         "name_kr": "\ub304\uc2a4\ud559\uc6d0",
         "pid": 186
     },
     {
-        "id": 302,
+        "id": 300,
         "level": 4,
-        "name_kr": "\ubb34\uc608/\uaca9\ud22c",
+        "name_kr": "\ud0dc\uad8c\ub3c4/\uac80\ub3c4",
         "pid": 186
     },
     {
-        "id": 298,
+        "id": 301,
         "level": 4,
-        "name_kr": "\uc694\uac00\uc6d0",
+        "name_kr": "\uae30\uccb4\uc870/\uc218\ub828",
         "pid": 186
     },
     {
-        "id": 296,
+        "id": 302,
         "level": 4,
-        "name_kr": "\uc885\ud569\uc2a4\ud3ec\uce20\uc13c\ud130",
+        "name_kr": "\ubb34\uc608/\uaca9\ud22c",
         "pid": 186
     },
     {
-        "id": 300,
+        "id": 303,
         "level": 4,
-        "name_kr": "\ud0dc\uad8c\ub3c4/\uac80\ub3c4",
+        "name_kr": "\uae30\ud0c0\uccb4\ub825\ub2e8\ub828\uc2dc\uc124",
         "pid": 186
     },
     {
         "id": 304,
         "level": 4,
         "name_kr": "\uace8\ud504\uc7a5(\ud544\ub4dc)",
         "pid": 187
@@ -1838,23 +1718,17 @@
     {
         "id": 305,
         "level": 4,
         "name_kr": "\uace8\ud504\uc7a5\uc608\uc57d\uc804\ubb38",
         "pid": 187
     },
     {
-        "id": 311,
-        "level": 4,
-        "name_kr": "\uae30\ud0c0\ub808\uc800\uc2dc\uc124",
-        "pid": 187
-    },
-    {
-        "id": 309,
+        "id": 306,
         "level": 4,
-        "name_kr": "\ub09a\uc2dc\ud130",
+        "name_kr": "\uc2a4\ud0a4/\ub208\uc370\ub9e4\uc7a5",
         "pid": 187
     },
     {
         "id": 307,
         "level": 4,
         "name_kr": "\uc11c\ubc14\uc774\ubc8c/\ub798\ud504\ud305/ATV",
         "pid": 187
@@ -1862,164 +1736,158 @@
     {
         "id": 308,
         "level": 4,
         "name_kr": "\uc218\uc0c1\uc2a4\ud3ec\uce20\uc2dc\uc124",
         "pid": 187
     },
     {
-        "id": 306,
+        "id": 309,
         "level": 4,
-        "name_kr": "\uc2a4\ud0a4/\ub208\uc370\ub9e4\uc7a5",
+        "name_kr": "\ub09a\uc2dc\ud130",
         "pid": 187
     },
     {
         "id": 310,
         "level": 4,
         "name_kr": "\uccb4\ud5d8\ud559\uc2b5",
         "pid": 187
     },
     {
-        "id": 313,
+        "id": 311,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\ucde8\ubbf8\uc2dc\uc124",
-        "pid": 188
+        "name_kr": "\uae30\ud0c0\ub808\uc800\uc2dc\uc124",
+        "pid": 187
     },
     {
         "id": 312,
         "level": 4,
         "name_kr": "\ubb38\ud654\uc13c\ud130",
         "pid": 188
     },
     {
-        "id": 315,
+        "id": 313,
         "level": 4,
-        "name_kr": "\uacbd\ub9c8\uc7a5",
+        "name_kr": "\uae30\ud0c0\ucde8\ubbf8\uc2dc\uc124",
+        "pid": 188
+    },
+    {
+        "id": 314,
+        "level": 4,
+        "name_kr": "\uce74\uc9c0\ub178",
         "pid": 189
     },
     {
-        "id": 316,
+        "id": 315,
         "level": 4,
-        "name_kr": "\ubcf5\uad8c",
+        "name_kr": "\uacbd\ub9c8\uc7a5",
         "pid": 189
     },
     {
-        "id": 314,
+        "id": 316,
         "level": 4,
-        "name_kr": "\uce74\uc9c0\ub178",
+        "name_kr": "\ubcf5\uad8c",
         "pid": 189
     },
     {
-        "id": 325,
+        "id": 319,
         "level": 4,
-        "name_kr": "\uac00\ubc29/\uc9c0\uac11\ube0c\ub79c\ub4dc",
+        "name_kr": "\uc885\ud569\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
         "id": 320,
         "level": 4,
         "name_kr": "\uad6c\ub9e4\ub300\ud589",
         "pid": 231
     },
     {
-        "id": 326,
+        "id": 321,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\ud328\uc158\uc7a1\ud654\ube0c\ub79c\ub4dc",
+        "name_kr": "\uba40\ud2f0\uc0f5",
         "pid": 231
     },
     {
-        "id": 321,
+        "id": 322,
         "level": 4,
-        "name_kr": "\uba40\ud2f0\uc0f5",
+        "name_kr": "\uc758\ub958\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
-        "id": 324,
+        "id": 323,
         "level": 4,
-        "name_kr": "\uc2e0\ubc1c\ube0c\ub79c\ub4dc",
+        "name_kr": "\uc96c\uc5bc\ub9ac\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
-        "id": 322,
+        "id": 324,
         "level": 4,
-        "name_kr": "\uc758\ub958\ube0c\ub79c\ub4dc",
+        "name_kr": "\uc2e0\ubc1c\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
-        "id": 319,
+        "id": 325,
         "level": 4,
-        "name_kr": "\uc885\ud569\ube0c\ub79c\ub4dc",
+        "name_kr": "\uac00\ubc29/\uc9c0\uac11\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
-        "id": 323,
+        "id": 326,
         "level": 4,
-        "name_kr": "\uc96c\uc5bc\ub9ac\ube0c\ub79c\ub4dc",
+        "name_kr": "\uae30\ud0c0\ud328\uc158\uc7a1\ud654\ube0c\ub79c\ub4dc",
         "pid": 231
     },
     {
-        "id": 330,
+        "id": 327,
         "level": 4,
-        "name_kr": "\uac00\ubc29/\uc9c0\uac11\uc804\ubb38",
+        "name_kr": "\uc758\ub958\uc804\ubb38",
         "pid": 232
     },
     {
-        "id": 331,
+        "id": 328,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\ud328\uc158\uc7a1\ud654\uc804\ubb38",
+        "name_kr": "\uc96c\uc5bc\ub9ac\uc804\ubb38",
         "pid": 232
     },
     {
         "id": 329,
         "level": 4,
         "name_kr": "\uc2e0\ubc1c\uc804\ubb38",
         "pid": 232
     },
     {
-        "id": 327,
+        "id": 330,
         "level": 4,
-        "name_kr": "\uc758\ub958\uc804\ubb38",
+        "name_kr": "\uac00\ubc29/\uc9c0\uac11\uc804\ubb38",
         "pid": 232
     },
     {
-        "id": 328,
+        "id": 331,
         "level": 4,
-        "name_kr": "\uc96c\uc5bc\ub9ac\uc804\ubb38",
+        "name_kr": "\uae30\ud0c0\ud328\uc158\uc7a1\ud654\uc804\ubb38",
         "pid": 232
     },
     {
-        "id": 339,
+        "id": 332,
         "level": 4,
-        "name_kr": "\uae30\ud0c0\ud2b9\uc218\uc758\ub958\uc804\ubb38",
+        "name_kr": "\ube45\uc0ac\uc774\uc988\uc804\ubb38",
         "pid": 233
     },
     {
         "id": 333,
         "level": 4,
         "name_kr": "\ube44\uce58\uc6e8\uc5b4\uc804\ubb38",
         "pid": 233
     },
     {
-        "id": 332,
-        "level": 4,
-        "name_kr": "\ube45\uc0ac\uc774\uc988\uc804\ubb38",
-        "pid": 233
-    },
-    {
         "id": 334,
         "level": 4,
         "name_kr": "\uc18d\uc637\uc804\ubb38",
         "pid": 233
     },
     {
-        "id": 338,
-        "level": 4,
-        "name_kr": "\uc2a4\ud3ec\uce20\uc758\ub958\uc804\ubb38",
-        "pid": 233
-    },
-    {
         "id": 335,
         "level": 4,
         "name_kr": "\uc720\ub2c8\ud3fc/\ub2e8\uccb4\ubcf5\uc804\ubb38",
         "pid": 233
     },
     {
         "id": 336,
@@ -2030,24 +1898,48 @@
     {
         "id": 337,
         "level": 4,
         "name_kr": "\ucee4\ud50c\ub8e9/\ud328\ubc00\ub9ac\ub8e9\uc804\ubb38",
         "pid": 233
     },
     {
-        "id": 383,
+        "id": 338,
         "level": 4,
-        "name_kr": "\ubb34\uc120\ubd80\uac00\uc11c\ube44\uc2a4",
-        "pid": 259
+        "name_kr": "\uc2a4\ud3ec\uce20\uc758\ub958\uc804\ubb38",
+        "pid": 233
     },
     {
-        "id": 382,
+        "id": 339,
         "level": 4,
-        "name_kr": "\ubb34\uc120\ud1b5\uc2e0\uc11c\ube44\uc2a4",
-        "pid": 259
+        "name_kr": "\uae30\ud0c0\ud2b9\uc218\uc758\ub958\uc804\ubb38",
+        "pid": 233
+    },
+    {
+        "id": 341,
+        "level": 3,
+        "name_kr": "\ud074\ub9ac\ub2c9",
+        "pid": 30
+    },
+    {
+        "id": 347,
+        "level": 2,
+        "name_kr": "\ub300\ud615\uc885\ud569\uc1fc\ud551\ubab0",
+        "pid": 14
+    },
+    {
+        "id": 348,
+        "level": 3,
+        "name_kr": "\uc77c\ubc18\uc911\uc18c\ud615\uc885\ud569\uc1fc\ud551\ubab0",
+        "pid": 76
+    },
+    {
+        "id": 349,
+        "level": 3,
+        "name_kr": "\uad6c\ub9e4\ub300\ud589\uc885\ud569\uc1fc\ud551\ubab0",
+        "pid": 76
     },
     {
         "id": 350,
         "level": 3,
         "name_kr": "\uc624\ud508\ub9c8\ucf13",
         "pid": 347
     },
@@ -2060,79 +1952,187 @@
     {
         "id": 352,
         "level": 4,
         "name_kr": "\uc624\ud508\ub9c8\ucf13",
         "pid": 350
     },
     {
-        "id": 355,
+        "id": 353,
         "level": 4,
-        "name_kr": "\ub9c8\ud2b8",
+        "name_kr": "\ud648\uc1fc\ud551",
         "pid": 351
     },
     {
-        "id": 357,
+        "id": 354,
         "level": 4,
-        "name_kr": "\uba74\uc138\uc810",
+        "name_kr": "\ubc31\ud654\uc810",
         "pid": 351
     },
     {
-        "id": 354,
+        "id": 355,
         "level": 4,
-        "name_kr": "\ubc31\ud654\uc810",
+        "name_kr": "\ub9c8\ud2b8",
         "pid": 351
     },
     {
         "id": 356,
         "level": 4,
         "name_kr": "\uc628\ub77c\uc778",
         "pid": 351
     },
     {
-        "id": 353,
+        "id": 357,
         "level": 4,
-        "name_kr": "\ud648\uc1fc\ud551",
+        "name_kr": "\uba74\uc138\uc810",
         "pid": 351
     },
     {
-        "id": 89,
-        "level": 2,
-        "name_kr": "\uac74\ucd95/\uc124\uacc4/\ud1a0\ubaa9",
-        "pid": 376
+        "id": 358,
+        "level": 4,
+        "name_kr": "\uae30\ud0c0\uc77c\ubc18\uc758\uc6d0",
+        "pid": 148
     },
     {
-        "id": 378,
-        "level": 2,
-        "name_kr": "\uc778\ud14c\ub9ac\uc5b4",
-        "pid": 376
+        "id": 359,
+        "level": 4,
+        "name_kr": "\ud63c\ud569\uc758\uc6d0",
+        "pid": 148
+    },
+    {
+        "id": 360,
+        "level": 3,
+        "name_kr": "\uc774\ubca4\ud2b8\uae30\ud68d",
+        "pid": 47
+    },
+    {
+        "id": 361,
+        "level": 3,
+        "name_kr": "\uc608\uc220/\uacf5\uc5f0\ub2e8\uccb4",
+        "pid": 54
+    },
+    {
+        "id": 362,
+        "level": 3,
+        "name_kr": "\uc219\ubc15\uc911\uac1c/\uc608\uc57d\ub300\ud589",
+        "pid": 73
+    },
+    {
+        "id": 363,
+        "level": 3,
+        "name_kr": "\ub300\ucd9c\uc911\uac1c/\uac00\uaca9\ube44\uad50",
+        "pid": 44
     },
     {
         "id": 374,
         "level": 3,
         "name_kr": "\uc778\ud14c\ub9ac\uc5b4\uc2dc\uacf5/\ub9ac\ubaa8\ub378\ub9c1",
         "pid": 378
     },
     {
         "id": 375,
         "level": 3,
         "name_kr": "\uc778\ud14c\ub9ac\uc5b4\uc790\uc7ac\ud310\ub9e4",
         "pid": 378
     },
     {
-        "id": 392,
+        "id": 376,
+        "level": 1,
+        "name_kr": "\uac74\ucd95/\uc778\ud14c\ub9ac\uc5b4",
+        "pid": 0
+    },
+    {
+        "id": 378,
+        "level": 2,
+        "name_kr": "\uc778\ud14c\ub9ac\uc5b4",
+        "pid": 376
+    },
+    {
+        "id": 379,
         "level": 4,
-        "name_kr": "\uae30\ud0c0 \ud3c9\uc0dd\uad50\uc721\uae30\uad00",
-        "pid": 384
+        "name_kr": "\uc77c\ubc18/\uac00\uc815\uc6a9\uac00\uad6c",
+        "pid": 119
+    },
+    {
+        "id": 380,
+        "level": 4,
+        "name_kr": "\uc0ac\ubb34/\uc5c5\uc18c\uc6a9\uac00\uad6c",
+        "pid": 119
+    },
+    {
+        "id": 381,
+        "level": 3,
+        "name_kr": "\ud504\ub79c\ucc28\uc774\uc988",
+        "pid": 91
+    },
+    {
+        "id": 382,
+        "level": 4,
+        "name_kr": "\ubb34\uc120\ud1b5\uc2e0\uc11c\ube44\uc2a4",
+        "pid": 259
+    },
+    {
+        "id": 383,
+        "level": 4,
+        "name_kr": "\ubb34\uc120\ubd80\uac00\uc11c\ube44\uc2a4",
+        "pid": 259
+    },
+    {
+        "id": 384,
+        "level": 3,
+        "name_kr": "\ud3c9\uc0dd\uad50\uc721\uae30\uad00",
+        "pid": 38
+    },
+    {
+        "id": 385,
+        "level": 4,
+        "name_kr": "\uc804\ubb38\ub300\ud559",
+        "pid": 163
+    },
+    {
+        "id": 386,
+        "level": 4,
+        "name_kr": "\ub300\ud559\uad50",
+        "pid": 163
+    },
+    {
+        "id": 387,
+        "level": 4,
+        "name_kr": "\ub300\ud559\uc6d0",
+        "pid": 163
+    },
+    {
+        "id": 388,
+        "level": 4,
+        "name_kr": "\uc6d0\uaca9\ub300\ud559\uad50",
+        "pid": 163
+    },
+    {
+        "id": 389,
+        "level": 4,
+        "name_kr": "\uae30\ud0c0 \uace0\ub4f1\uad50\uc721\uae30\uad00",
+        "pid": 163
     },
     {
         "id": 390,
         "level": 4,
         "name_kr": "\ub300\ud559\ubd80\uc124 \ud3c9\uc0dd\uad50\uc721\uc6d0",
         "pid": 384
     },
     {
         "id": 391,
         "level": 4,
         "name_kr": "\uc9c1\uc5c5 \uc804\ubb38\ud559\uad50",
         "pid": 384
+    },
+    {
+        "id": 392,
+        "level": 4,
+        "name_kr": "\uae30\ud0c0 \ud3c9\uc0dd\uad50\uc721\uae30\uad00",
+        "pid": 384
+    },
+    {
+        "id": 393,
+        "level": 4,
+        "name_kr": "\uc694\uc591\uc6d0",
+        "pid": 138
     }
 ]
```

### Comparing `datakart-1.6.8/src/datakart/core/assets/na_event.json` & `datakart-1.6.9/src/datakart/core/assets/naver_ad_event.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666663%*

 * *Differences: {'0': "{'naem_eng': 'Living', delete: ['name_eng']}",*

 * * '1': "{'naem_eng': 'Home Appliances', delete: ['name_eng']}",*

 * * '10': "{'naem_eng': 'Fishing', delete: ['name_eng']}",*

 * * '11': "{'naem_eng': 'Horticulture', delete: ['name_eng']}",*

 * * '12': "{'naem_eng': 'Movies & Entertainment', delete: ['name_eng']}",*

 * * '13': "{'naem_eng': 'Bedding', delete: ['name_eng']}",*

 * * '14': "{'naem_eng': 'Household Goods', delete: ['name_eng']}",*

 * * '15': "{'naem_eng': 'Health', delete: ['name_eng']}",*

 * * '16': "{'naem_eng': 'Health', d […]*

```diff
@@ -1,478 +1,478 @@
 [
     {
         "id": 1,
         "level": 1,
-        "name_eng": "Living",
+        "naem_eng": "Living",
         "name_kr": "\uc0dd\ud65c",
         "pid": 0
     },
     {
         "id": 3,
         "level": 2,
-        "name_eng": "Home Appliances",
+        "naem_eng": "Home Appliances",
         "name_kr": "\uac00\uc804",
         "pid": 1
     },
     {
         "id": 5,
         "level": 2,
-        "name_eng": "Rainy Season",
+        "naem_eng": "Rainy Season",
         "name_kr": "\uc7a5\ub9c8",
         "pid": 1
     },
     {
         "id": 6,
         "level": 2,
-        "name_eng": "Heating",
+        "naem_eng": "Heating",
         "name_kr": "\ub09c\ubc29/\ubc29\ud55c",
         "pid": 1
     },
     {
         "id": 7,
         "level": 2,
-        "name_eng": "Insect",
+        "naem_eng": "Insect",
         "name_kr": "\ubc29\ucda9",
         "pid": 1
     },
     {
         "id": 8,
         "level": 2,
-        "name_eng": "Cooling",
+        "naem_eng": "Cooling",
         "name_kr": "\ub0c9\ubc29",
         "pid": 1
     },
     {
         "id": 10,
         "level": 2,
-        "name_eng": "Baby & Kids",
+        "naem_eng": "Baby & Kids",
         "name_kr": "\uc720\uc544/\uc544\ub3d9",
         "pid": 1
     },
     {
         "id": 12,
         "level": 2,
-        "name_eng": "Vehicles",
+        "naem_eng": "Vehicles",
         "name_kr": "\uc790\ub3d9\ucc28",
         "pid": 1
     },
     {
         "id": 14,
         "level": 2,
-        "name_eng": "Jobs",
+        "naem_eng": "Jobs",
         "name_kr": "\ucde8\uc5c5",
         "pid": 1
     },
     {
         "id": 16,
         "level": 2,
-        "name_eng": "Handmade",
+        "naem_eng": "Handmade",
         "name_kr": "\uc218\uacf5\uc608",
         "pid": 1
     },
     {
         "id": 17,
         "level": 2,
-        "name_eng": "Fishing",
+        "naem_eng": "Fishing",
         "name_kr": "\ub09a\uc2dc",
         "pid": 1
     },
     {
         "id": 18,
         "level": 2,
-        "name_eng": "Horticulture",
+        "naem_eng": "Horticulture",
         "name_kr": "\uc6d0\uc608",
         "pid": 1
     },
     {
         "id": 20,
         "level": 2,
-        "name_eng": "Movies & Entertainment",
+        "naem_eng": "Movies & Entertainment",
         "name_kr": "\uc601\ud654/\uacf5\uc5f0",
         "pid": 1
     },
     {
         "id": 22,
         "level": 2,
-        "name_eng": "Bedding",
+        "naem_eng": "Bedding",
         "name_kr": "\uce68\uad6c",
         "pid": 1
     },
     {
         "id": 23,
         "level": 2,
-        "name_eng": "Household Goods",
+        "naem_eng": "Household Goods",
         "name_kr": "\uc0dd\ud65c\uc6a9\ud488",
         "pid": 1
     },
     {
         "id": 24,
         "level": 1,
-        "name_eng": "Health",
+        "naem_eng": "Health",
         "name_kr": "\uac74\uac15",
         "pid": 0
     },
     {
         "id": 26,
         "level": 2,
-        "name_eng": "Health",
+        "naem_eng": "Health",
         "name_kr": "\uac74\uac15",
         "pid": 24
     },
     {
         "id": 27,
         "level": 1,
-        "name_eng": "Leisure & Sports",
+        "naem_eng": "Leisure & Sports",
         "name_kr": "\ub808\uc800/\uc2a4\ud3ec\uce20",
         "pid": 0
     },
     {
         "id": 29,
         "level": 2,
-        "name_eng": "Baseball",
+        "naem_eng": "Baseball",
         "name_kr": "\ud504\ub85c\uc57c\uad6c",
         "pid": 27
     },
     {
         "id": 30,
         "level": 2,
-        "name_eng": "Climbing",
+        "naem_eng": "Climbing",
         "name_kr": "\ub4f1\uc0b0",
         "pid": 27
     },
     {
         "id": 31,
         "level": 2,
-        "name_eng": "Skiing & Snowboarding",
+        "naem_eng": "Skiing & Snowboarding",
         "name_kr": "\uc2a4\ud0a4/\ubcf4\ub4dc",
         "pid": 27
     },
     {
         "id": 32,
         "level": 2,
-        "name_eng": "Aquatic Sports",
+        "naem_eng": "Aquatic Sports",
         "name_kr": "\uc218\uc0c1\uc2a4\ud3ec\uce20",
         "pid": 27
     },
     {
         "id": 33,
         "level": 2,
-        "name_eng": "Sports",
+        "naem_eng": "Sports",
         "name_kr": "\uc2a4\ud3ec\uce20",
         "pid": 27
     },
     {
         "id": 34,
         "level": 2,
-        "name_eng": "Bicycles",
+        "naem_eng": "Bicycles",
         "name_kr": "\uc790\uc804\uac70",
         "pid": 27
     },
     {
         "id": 35,
         "level": 1,
-        "name_eng": "Seasons",
+        "naem_eng": "Seasons",
         "name_kr": "\uc2dc\uae30",
         "pid": 0
     },
     {
         "id": 37,
         "level": 2,
-        "name_eng": "Korean New Year",
+        "naem_eng": "Korean New Year",
         "name_kr": "\uc124",
         "pid": 35
     },
     {
         "id": 38,
         "level": 2,
-        "name_eng": "Chuseok",
+        "naem_eng": "Chuseok",
         "name_kr": "\ucd94\uc11d",
         "pid": 35
     },
     {
         "id": 39,
         "level": 2,
-        "name_eng": "Teachers' Day",
+        "naem_eng": "Teachers' Day",
         "name_kr": "\uc2a4\uc2b9\uc758\ub0a0",
         "pid": 35
     },
     {
         "id": 40,
         "level": 2,
-        "name_eng": "Children's Day",
+        "naem_eng": "Children's Day",
         "name_kr": "\uc5b4\ub9b0\uc774\ub0a0",
         "pid": 35
     },
     {
         "id": 41,
         "level": 2,
-        "name_eng": "White Day",
+        "naem_eng": "White Day",
         "name_kr": "\ud654\uc774\ud2b8\ub370\uc774",
         "pid": 35
     },
     {
         "id": 42,
         "level": 2,
-        "name_eng": "Christmas",
+        "naem_eng": "Christmas",
         "name_kr": "\ud06c\ub9ac\uc2a4\ub9c8\uc2a4",
         "pid": 35
     },
     {
         "id": 43,
         "level": 2,
-        "name_eng": "Valentine's Day",
+        "naem_eng": "Valentine's Day",
         "name_kr": "\ubc1c\ub80c\ud0c0\uc778\ub370\uc774",
         "pid": 35
     },
     {
         "id": 44,
         "level": 2,
-        "name_eng": "Mother's Day & Father's Day",
+        "naem_eng": "Mother's Day & Father's Day",
         "name_kr": "\uc5b4\ubc84\uc774\ub0a0",
         "pid": 35
     },
     {
         "id": 45,
         "level": 2,
-        "name_eng": "Coming of Age Day",
+        "naem_eng": "Coming of Age Day",
         "name_kr": "\uc131\ub144\uc758\ub0a0",
         "pid": 35
     },
     {
         "id": 46,
         "level": 2,
-        "name_eng": "Halloween",
+        "naem_eng": "Halloween",
         "name_kr": "\ud560\ub85c\uc708",
         "pid": 35
     },
     {
         "id": 47,
         "level": 2,
-        "name_eng": "Pepero Day",
+        "naem_eng": "Pepero Day",
         "name_kr": "\ube7c\ube7c\ub85c\ub370\uc774",
         "pid": 35
     },
     {
         "id": 49,
         "level": 2,
-        "name_eng": "Festivals & Events",
+        "naem_eng": "Festivals & Events",
         "name_kr": "\ucd95\uc81c/\ud589\uc0ac",
         "pid": 35
     },
     {
         "id": 50,
         "level": 2,
-        "name_eng": "Cherry Blossom Season",
+        "naem_eng": "Cherry Blossom Season",
         "name_kr": "\ubc9a\uaf43",
         "pid": 35
     },
     {
         "id": 52,
         "level": 2,
-        "name_eng": "Spring",
+        "naem_eng": "Spring",
         "name_kr": "\ubd04",
         "pid": 35
     },
     {
         "id": 53,
         "level": 2,
-        "name_eng": "Fall",
+        "naem_eng": "Fall",
         "name_kr": "\uac00\uc744",
         "pid": 35
     },
     {
         "id": 54,
         "level": 2,
-        "name_eng": "Winter",
+        "naem_eng": "Winter",
         "name_kr": "\uaca8\uc6b8",
         "pid": 35
     },
     {
         "id": 55,
         "level": 2,
-        "name_eng": "New Year & Fortune",
+        "naem_eng": "New Year & Fortune",
         "name_kr": "\uc0c8\ud574/\uc6b4\uc138",
         "pid": 35
     },
     {
         "id": 56,
         "level": 2,
-        "name_eng": "Year End",
+        "naem_eng": "Year End",
         "name_kr": "\uc5f0\ub9d0",
         "pid": 35
     },
     {
         "id": 57,
         "level": 2,
-        "name_eng": "Summer",
+        "naem_eng": "Summer",
         "name_kr": "\uc5ec\ub984",
         "pid": 35
     },
     {
         "id": 58,
         "level": 1,
-        "name_eng": "Education & School",
+        "naem_eng": "Education & School",
         "name_kr": "\uad50\uc721/\ud559\uad50",
         "pid": 0
     },
     {
         "id": 60,
         "level": 2,
-        "name_eng": "Graduation",
+        "naem_eng": "Graduation",
         "name_kr": "\uc878\uc5c5",
         "pid": 58
     },
     {
         "id": 61,
         "level": 2,
-        "name_eng": "Private Institutes",
+        "naem_eng": "Private Institutes",
         "name_kr": "\ud559\uc6d0",
         "pid": 58
     },
     {
         "id": 62,
         "level": 2,
-        "name_eng": "School Events",
+        "naem_eng": "School Events",
         "name_kr": "\ud559\uad50\ud589\uc0ac",
         "pid": 58
     },
     {
         "id": 63,
         "level": 2,
-        "name_eng": "Admissions & SAT Tests",
+        "naem_eng": "Admissions & SAT Tests",
         "name_kr": "\ub300\uc785/\uc218\ub2a5",
         "pid": 58
     },
     {
         "id": 64,
         "level": 2,
-        "name_eng": "Teaching Materials & Aids",
+        "naem_eng": "Teaching Materials & Aids",
         "name_kr": "\uad50\uc7ac/\uad50\uad6c",
         "pid": 58
     },
     {
         "id": 65,
         "level": 2,
-        "name_eng": "Entrance & New Semester",
+        "naem_eng": "Entrance & New Semester",
         "name_kr": "\uc785\ud559/\uac1c\ud559",
         "pid": 58
     },
     {
         "id": 66,
         "level": 2,
-        "name_eng": "School Assignments",
+        "naem_eng": "School Assignments",
         "name_kr": "\uacfc\uc81c",
         "pid": 58
     },
     {
         "id": 67,
         "level": 1,
-        "name_eng": "Farming",
+        "naem_eng": "Farming",
         "name_kr": "\ub18d\uc5c5",
         "pid": 0
     },
     {
         "id": 69,
         "level": 2,
-        "name_eng": "Plants",
+        "naem_eng": "Plants",
         "name_kr": "\uc2dd\ubb3c",
         "pid": 67
     },
     {
         "id": 70,
         "level": 1,
-        "name_eng": "Food & Cooking",
+        "naem_eng": "Food & Cooking",
         "name_kr": "\uc74c\uc2dd/\uc694\ub9ac",
         "pid": 0
     },
     {
         "id": 72,
         "level": 2,
-        "name_eng": "Health Supplements",
+        "naem_eng": "Health Supplements",
         "name_kr": "\uac74\uac15\uc2dd\ud488",
         "pid": 70
     },
     {
         "id": 73,
         "level": 2,
-        "name_eng": "Agricultural & Fishery",
+        "naem_eng": "Agricultural & Fishery",
         "name_kr": "\ub18d\uc0b0\ubb3c/\uc218\uc0b0\ubb3c",
         "pid": 70
     },
     {
         "id": 74,
         "level": 2,
-        "name_eng": "Restaurants",
+        "naem_eng": "Restaurants",
         "name_kr": "\uc74c\uc2dd\uc810",
         "pid": 70
     },
     {
         "id": 75,
         "level": 2,
-        "name_eng": "Food",
+        "naem_eng": "Food",
         "name_kr": "\uc74c\uc2dd",
         "pid": 70
     },
     {
         "id": 76,
         "level": 2,
-        "name_eng": "Refreshment",
+        "naem_eng": "Refreshment",
         "name_kr": "\uae30\ud638\uc2dd\ud488",
         "pid": 70
     },
     {
         "id": 77,
         "level": 1,
-        "name_eng": "Fashion & Beauty",
+        "naem_eng": "Fashion & Beauty",
         "name_kr": "\ud328\uc158/\ubbf8\uc6a9",
         "pid": 0
     },
     {
         "id": 79,
         "level": 2,
-        "name_eng": "Fashion",
+        "naem_eng": "Fashion",
         "name_kr": "\ud328\uc158",
         "pid": 77
     },
     {
         "id": 80,
         "level": 2,
-        "name_eng": "Beauty",
+        "naem_eng": "Beauty",
         "name_kr": "\ubbf8\uc6a9",
         "pid": 77
     },
     {
         "id": 81,
         "level": 1,
-        "name_eng": "Outdoors",
+        "naem_eng": "Outdoors",
         "name_kr": "\uc5ec\ud589",
         "pid": 0
     },
     {
         "id": 83,
         "level": 2,
-        "name_eng": "Travel",
+        "naem_eng": "Travel",
         "name_kr": "\uc5ec\ud589",
         "pid": 81
     },
     {
         "id": 84,
         "level": 2,
-        "name_eng": "Camping",
+        "naem_eng": "Camping",
         "name_kr": "\ucea0\ud551",
         "pid": 81
     },
     {
         "id": 85,
         "level": 2,
-        "name_eng": "Picnic",
+        "naem_eng": "Picnic",
         "name_kr": "\ud53c\ud06c\ub2c9",
         "pid": 81
     },
     {
         "id": 86,
         "level": 2,
-        "name_eng": "Pet",
+        "naem_eng": "Pet",
         "name_kr": "\ubc18\ub824\ub3d9\ubb3c",
         "pid": 1
     }
 ]
```

### Comparing `datakart-1.6.8/.gitignore` & `datakart-1.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/LICENSE` & `datakart-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datakart-1.6.8/pyproject.toml` & `datakart-1.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "datakart"
-version = "1.6.8"
+version = "1.6.9"
 authors = [
   { name="HYUNIL MOON", email="hyunil.moon@gmail.com" },
 ]
 description = "A small data kart package"
 readme = "README.md"
 keywords = ["datakart", "data", "kart", "ECOS", "SGIS", "NAVER", "Kakao", "K-data", "ecos.bok.or.kr", "data.go.kr", "kostat.go.kr", "juso.go.kr"]
 requires-python = ">=3.7"
```

### Comparing `datakart-1.6.8/PKG-INFO` & `datakart-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datakart
-Version: 1.6.8
+Version: 1.6.9
 Summary: A small data kart package
 Project-URL: Homepage, https://github.com/himoon/datakart
 Project-URL: Issues, https://github.com/himoon/datakart/issues
 Author-email: HYUNIL MOON <hyunil.moon@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

