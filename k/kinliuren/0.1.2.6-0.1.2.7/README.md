# Comparing `tmp/kinliuren-0.1.2.6.tar.gz` & `tmp/kinliuren-0.1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinliuren-0.1.2.6.tar", last modified: Mon Oct  9 04:26:49 2023, max compression
+gzip compressed data, was "kinliuren-0.1.2.7.tar", last modified: Thu May 30 04:34:13 2024, max compression
```

## Comparing `kinliuren-0.1.2.6.tar` & `kinliuren-0.1.2.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-10-09 04:26:49.310776 kinliuren-0.1.2.6/
--rw-rw-rw-   0        0        0     4006 2023-10-09 04:26:49.308779 kinliuren-0.1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3558 2021-12-18 05:12:54.000000 kinliuren-0.1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-10-09 04:26:49.275793 kinliuren-0.1.2.6/kinliuren/
--rw-rw-rw-   0        0        0        3 2023-10-04 10:42:21.000000 kinliuren-0.1.2.6/kinliuren/__init__.py
--rw-rw-rw-   0        0        0    81859 2023-10-04 10:42:21.000000 kinliuren-0.1.2.6/kinliuren/kinliuren.py
-drwxrwxrwx   0        0        0        0 2023-10-09 04:26:49.305780 kinliuren-0.1.2.6/kinliuren.egg-info/
--rw-rw-rw-   0        0        0     4006 2023-10-09 04:26:48.000000 kinliuren-0.1.2.6/kinliuren.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-10-09 04:26:49.000000 kinliuren-0.1.2.6/kinliuren.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-09 04:26:48.000000 kinliuren-0.1.2.6/kinliuren.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-10-09 04:26:48.000000 kinliuren-0.1.2.6/kinliuren.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-09 04:26:49.310776 kinliuren-0.1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-10-09 04:26:27.000000 kinliuren-0.1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:34:13.683584 kinliuren-0.1.2.7/
+-rw-rw-rw-   0        0        0     1086 2024-05-30 04:14:03.000000 kinliuren-0.1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4481 2024-05-30 04:34:13.683584 kinliuren-0.1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4010 2024-05-30 04:14:04.000000 kinliuren-0.1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 04:34:13.657692 kinliuren-0.1.2.7/kinliuren/
+-rw-rw-rw-   0        0        0        3 2024-05-30 04:14:04.000000 kinliuren-0.1.2.7/kinliuren/__init__.py
+-rw-rw-rw-   0        0        0    82510 2024-05-30 04:14:04.000000 kinliuren-0.1.2.7/kinliuren/kinliuren.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:34:13.681576 kinliuren-0.1.2.7/kinliuren.egg-info/
+-rw-rw-rw-   0        0        0     4481 2024-05-30 04:34:12.000000 kinliuren-0.1.2.7/kinliuren.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-30 04:34:12.000000 kinliuren-0.1.2.7/kinliuren.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 04:34:12.000000 kinliuren-0.1.2.7/kinliuren.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 04:34:12.000000 kinliuren-0.1.2.7/kinliuren.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 04:34:13.686574 kinliuren-0.1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      767 2024-05-30 04:26:36.000000 kinliuren-0.1.2.7/setup.py
```

### Comparing `kinliuren-0.1.2.6/PKG-INFO` & `kinliuren-0.1.2.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-Metadata-Version: 2.1
-Name: kinliuren
-Version: 0.1.2.6
-Summary: Dailiuren (大六壬) is one of the three greatest Chinese Divination systems ever.
-Home-page: https://github.com/kentang2017/kinliuren
-Author: Ken Tang
-Author-email: kinyeah@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
-﻿# **Python 大六壬 Kinliuren 堅大六壬**
+﻿# **Python 大六壬 Kinliuren 堅大六壬 堅六壬**
 [![Python](https://img.shields.io/pypi/pyversions/kinliuren)](https://pypi.org/project/kinliuren/)
 [![PIP](https://img.shields.io/pypi/v/kinliuren)](https://pypi.org/project/kinliuren/)
 [![Downloads](https://img.shields.io/pypi/dm/kinliuren)](https://pypi.org/project/kinliuren/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
+[![TG Channel](https://img.shields.io/badge/chat-on%20telegram-red)](https://t.me/numerology_coding)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
-![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf/page568-428px-%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf.jpg "六壬軍帳神機")
 
+![alt text](https://github.com/kentang2017/kinliuren/blob/master/pic/Untitled-33.png)
 ## 1. 導讀 Introduction
 大六壬，或稱六壬神課，簡稱六壬，是中國古老三大占卜術之一。大六壬與奇門遁甲、太乙神數並稱三式。大六壬盛行於漢朝、三國、魏晉南北朝，文人名士多有以此為休閒，常以懷中藏物互相占卜猜測，名曰「射覆」。唐宋以來，明清相繼，相承至今。然六壬演式繁雜，主要在士大夫之間流傳，在民間社會中漸被文王卦所代替。當今社會，在中國大陸、香港和台灣均有一部分人在研習六壬。六壬術傳至日本後，在平安時代由陰陽師安倍晴明發揚光大。為現代算命相術之一。
 
+堅六壬排盤 https://kinliuren.streamlit.app/
+
 Da Liu Ren is a form of Chinese calendrical astrology dating from the later Warring States period. It is also a member of the Three Styles (三式; sānshì; 'three rites') of divination, along with Qi Men Dun Jia (奇门遁甲) and Taiyi (太乙).
 
 In the words of a contemporary Chinese master of Da Liu Ren, the six rén indicate an entire movement of the sexagenary cycle, during which an something may appear, rise to maturity and then decline and disappear. Thus the six rén indicate the life cycle of phenomena. There is a homonym in the Chinese language which carries the meaning of pregnancy and so the six rén also carry the meaning of the birth of a phenomenon.
 
-
 ## 2. 安裝套件 Installation
 ```python
 	pip install kinliuren
 ```
 ## 3. 起課方式 Quickstart
 ```python
 	from kinliuren import kinliuren
-	kinliuren.Liuren( 節氣, 日干支, 時干支).result(0)
-	例如 Liuren("冬至", "丁未", "乙巳")
-{'節氣': '冬至', '日期': '丁未日乙巳時', '格局': ['賊尅', '元首'], '三傳': {'初傳': ['卯', '勾陳', '父母', '空'], '中傳': ['亥', '貴人', '官鬼', '辛'], '末傳': ['未', '太常', '子孫', '丁']}, '四課': {'四課': ['亥卯', '貴人'], '三課': ['卯未', '勾陳'], '二課': ['亥卯', '貴人'], '一課': ['卯丁', '勾陳']}, '天地盤': {'天盤': ['丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌', '亥', '子'], '地盤': ['巳', '午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰'], '天將': ['朱雀', '六合', '勾陳', '青龍', '天空', '白虎', '太常', '玄武', '太陰', '天后', '貴人', '螣蛇']}, '地轉天盤': {'巳': '丑', '午': '寅', '未': '卯', '申': '辰', '酉': '巳', '戌': '午', '亥': '未', '子': '申', '丑': '酉', '寅': '戌', '卯': '亥', '辰': '子'}, '地轉天將': {'巳': '朱雀', '午': '六合', '未': '勾陳', '申': '青龍', '酉': '天空', '戌': '白虎', '亥': '太常', '子': '玄武', '丑': '太陰', '寅': '天后', '卯': '貴人', '辰': '螣蛇'}}
+	kinliuren.Liuren( 節氣, 農曆月份, 日干支, 時干支).result(0)
+	例如 Liuren("驚蟄","二","己未","甲午").result(0)
+{'節氣': '驚蟄', '日期': '己未日甲午時', '格局': ['賊尅', '重審'], '日馬': '巳', '三傳': {'初傳': ['巳', '虎', '父', '丁'], '中傳': ['戌', '雀', '兄', '壬'], '末傳': ['卯', '玄', '官', '乙']}, '四課': {'四課': ['巳子', '虎'], '三課': ['子未', '貴'], '二課': ['巳子', '虎'], '一課': ['子己', '貴']}, '天地盤': {'天盤': ['亥', '子', '丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌'], '地盤': ['午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰', '巳'], '天將': ['蛇', '貴', '后', '陰', '玄', '常', '虎', '空', '龍', '勾', '合', '雀']}, '地轉天盤': {'午': '亥', '未': '子', '申': '丑', '酉': '寅', '戌': '卯', '亥': '辰', '子': '巳', '丑': '午', '寅': '未', '卯': '申', '辰': '酉', '巳': '戌'}, '地轉天將': {'午': '蛇', '未': '貴', '申': '后', '酉': '陰', '戌': '玄', '亥': '常', '子': '虎', '丑': '空', '寅': '龍', '卯': '勾', '辰': '合', '巳': '雀'}, '神煞': {'天城': '申', '天吏': '寅', '皇書': '寅', '天喜': '戌', '天耳': '申', '戲神': '巳', '遊神': '丑', '天車': '巳', '月馬': '辰', '日馬': '巳', '丁馬': '巳', '日德': '寅', '日祿': '午', '賢貴': '丑', '進神': '卯', '進神二': '酉', '五合': '寅', '支德': '午', '將星': '卯', '六合': '午', '天馬': '申', '聖心': '巳', '天恩': '酉', '天財': '午', '飛廉': '巳', '會神': '戌', '成神': '申', '生氣': '丑', '月合': '戌', '閃電': '丑'}}
 ```
+
+
```

### Comparing `kinliuren-0.1.2.6/README.md` & `kinliuren-0.1.2.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-﻿# **Python 大六壬 Kinliuren 堅大六壬**
+Metadata-Version: 2.1
+Name: kinliuren
+Version: 0.1.2.7
+Summary: Dailiuren (大六壬) is one of the three greatest Chinese Divination systems ever.
+Home-page: https://github.com/kentang2017/kinliuren
+Author: Ken Tang
+Author-email: kinyeah@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿# **Python 大六壬 Kinliuren 堅大六壬 堅六壬**
 [![Python](https://img.shields.io/pypi/pyversions/kinliuren)](https://pypi.org/project/kinliuren/)
 [![PIP](https://img.shields.io/pypi/v/kinliuren)](https://pypi.org/project/kinliuren/)
 [![Downloads](https://img.shields.io/pypi/dm/kinliuren)](https://pypi.org/project/kinliuren/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
+[![TG Channel](https://img.shields.io/badge/chat-on%20telegram-red)](https://t.me/numerology_coding)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
-![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf/page568-428px-%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf.jpg "六壬軍帳神機")
 
+![alt text](https://github.com/kentang2017/kinliuren/blob/master/pic/Untitled-33.png)
 ## 1. 導讀 Introduction
 大六壬，或稱六壬神課，簡稱六壬，是中國古老三大占卜術之一。大六壬與奇門遁甲、太乙神數並稱三式。大六壬盛行於漢朝、三國、魏晉南北朝，文人名士多有以此為休閒，常以懷中藏物互相占卜猜測，名曰「射覆」。唐宋以來，明清相繼，相承至今。然六壬演式繁雜，主要在士大夫之間流傳，在民間社會中漸被文王卦所代替。當今社會，在中國大陸、香港和台灣均有一部分人在研習六壬。六壬術傳至日本後，在平安時代由陰陽師安倍晴明發揚光大。為現代算命相術之一。
 
+堅六壬排盤 https://kinliuren.streamlit.app/
+
 Da Liu Ren is a form of Chinese calendrical astrology dating from the later Warring States period. It is also a member of the Three Styles (三式; sānshì; 'three rites') of divination, along with Qi Men Dun Jia (奇门遁甲) and Taiyi (太乙).
 
 In the words of a contemporary Chinese master of Da Liu Ren, the six rén indicate an entire movement of the sexagenary cycle, during which an something may appear, rise to maturity and then decline and disappear. Thus the six rén indicate the life cycle of phenomena. There is a homonym in the Chinese language which carries the meaning of pregnancy and so the six rén also carry the meaning of the birth of a phenomenon.
 
-
 ## 2. 安裝套件 Installation
 ```python
 	pip install kinliuren
 ```
 ## 3. 起課方式 Quickstart
 ```python
 	from kinliuren import kinliuren
-	kinliuren.Liuren( 節氣, 日干支, 時干支).result(0)
-	例如 Liuren("冬至", "丁未", "乙巳")
-{'節氣': '冬至', '日期': '丁未日乙巳時', '格局': ['賊尅', '元首'], '三傳': {'初傳': ['卯', '勾陳', '父母', '空'], '中傳': ['亥', '貴人', '官鬼', '辛'], '末傳': ['未', '太常', '子孫', '丁']}, '四課': {'四課': ['亥卯', '貴人'], '三課': ['卯未', '勾陳'], '二課': ['亥卯', '貴人'], '一課': ['卯丁', '勾陳']}, '天地盤': {'天盤': ['丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌', '亥', '子'], '地盤': ['巳', '午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰'], '天將': ['朱雀', '六合', '勾陳', '青龍', '天空', '白虎', '太常', '玄武', '太陰', '天后', '貴人', '螣蛇']}, '地轉天盤': {'巳': '丑', '午': '寅', '未': '卯', '申': '辰', '酉': '巳', '戌': '午', '亥': '未', '子': '申', '丑': '酉', '寅': '戌', '卯': '亥', '辰': '子'}, '地轉天將': {'巳': '朱雀', '午': '六合', '未': '勾陳', '申': '青龍', '酉': '天空', '戌': '白虎', '亥': '太常', '子': '玄武', '丑': '太陰', '寅': '天后', '卯': '貴人', '辰': '螣蛇'}}
+	kinliuren.Liuren( 節氣, 農曆月份, 日干支, 時干支).result(0)
+	例如 Liuren("驚蟄","二","己未","甲午").result(0)
+{'節氣': '驚蟄', '日期': '己未日甲午時', '格局': ['賊尅', '重審'], '日馬': '巳', '三傳': {'初傳': ['巳', '虎', '父', '丁'], '中傳': ['戌', '雀', '兄', '壬'], '末傳': ['卯', '玄', '官', '乙']}, '四課': {'四課': ['巳子', '虎'], '三課': ['子未', '貴'], '二課': ['巳子', '虎'], '一課': ['子己', '貴']}, '天地盤': {'天盤': ['亥', '子', '丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌'], '地盤': ['午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰', '巳'], '天將': ['蛇', '貴', '后', '陰', '玄', '常', '虎', '空', '龍', '勾', '合', '雀']}, '地轉天盤': {'午': '亥', '未': '子', '申': '丑', '酉': '寅', '戌': '卯', '亥': '辰', '子': '巳', '丑': '午', '寅': '未', '卯': '申', '辰': '酉', '巳': '戌'}, '地轉天將': {'午': '蛇', '未': '貴', '申': '后', '酉': '陰', '戌': '玄', '亥': '常', '子': '虎', '丑': '空', '寅': '龍', '卯': '勾', '辰': '合', '巳': '雀'}, '神煞': {'天城': '申', '天吏': '寅', '皇書': '寅', '天喜': '戌', '天耳': '申', '戲神': '巳', '遊神': '丑', '天車': '巳', '月馬': '辰', '日馬': '巳', '丁馬': '巳', '日德': '寅', '日祿': '午', '賢貴': '丑', '進神': '卯', '進神二': '酉', '五合': '寅', '支德': '午', '將星': '卯', '六合': '午', '天馬': '申', '聖心': '巳', '天恩': '酉', '天財': '午', '飛廉': '巳', '會神': '戌', '成神': '申', '生氣': '丑', '月合': '戌', '閃電': '丑'}}
 ```
+
+
```

### Comparing `kinliuren-0.1.2.6/kinliuren/kinliuren.py` & `kinliuren-0.1.2.7/kinliuren/kinliuren.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,17 +403,18 @@
             elif  sike_list[7][2][0] != sike_list[7][2][1]:
                 findtrue =   "不適用，或試他法" 
             return findtrue 
         elif sike_list[0].count("上尅下") == 1 and sike_list[9] == '天地盤沒有返吟':
             findtrue =  ["返吟","無依", self.find_three_pass(sike[sike_list[0].index("上尅下")][0])]
             return findtrue
         elif sike_list[0].count("上尅下") == 1 and sike_list[9] == '天地盤返吟':
-            findtrue =  ["返吟","無依", [self.chong2.get(sike[sike_list[0].index("上尅下")][0]), self.chong2.get(sike[sike_list[0].index("上尅下")][1]), self.chong2.get(sike[sike_list[0].index("上尅下")][0])]]
+            findtrue =  ["伏吟","無依", [self.chong2.get(self.chong2.get(sike[sike_list[0].index("上尅下")][0])), self.chong2.get(self.hourgangzhi[1]), self.chong2.get(sike[sike_list[0].index("上尅下")][0])]]
             return findtrue
 
+
     def biyung(self):
         relation = self.find_sike_relations()
         filter_list = self.find_sike_relations()[7]
         filter_list_four_ke = self.find_sike_relations()[7][2]
         filter_list_yy = self.find_sike_relations()[7][5]
         dayganzhi_yy = self.find_sike_relations()[8]
         if filter_list[0] == "試賊尅":
@@ -670,58 +671,56 @@
                 result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][1])]
                 return result
         
         elif shangke.count("下賊上") == 3 and shangke.count("上尅下") == 1: 
           
             if self.find_sike_relations()[2].count("被尅") == 1 and self.find_sike_relations()[2].count("尅") == 1:
                 if self.find_sike_relations()[5] == "尅" or self.find_sike_relations()[5] ==  "被尅":
-                    result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][2][0])]
+                    result = ["涉害", "涉害", self.find_three_pass( self.daygangzhi[1])]
                     return result
                 elif self.find_sike_relations()[5] != "尅" or self.find_sike_relations()[5] !=   "被尅":
                     result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                     return result
             elif self.find_sike_relations()[2].count("被尅") == 1 and self.find_sike_relations()[2].count("尅") == 0:
                 result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][1])]
                 return result
             elif self.find_sike_relations()[2].count("被尅") == 0 and self.find_sike_relations()[2].count("尅") == 1:
                 result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                 return result
-            
-            
             else:
-                result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][2][0])]
+                result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                 return result
             
   
         elif shangke.count("下賊上") == 3 and self.find_sike_relations()[9] == "天地盤沒有返吟" and self.find_sike_relations()[2].count("被尅") == 1 and  self.find_sike_relations()[2].count("尅") == 1:
             result = ["涉害", "涉害", self.find_three_pass(self.find_sike_relations()[7][2][1][0])]
             return result
         
         elif shangke.count("下賊上") == 3 and self.find_sike_relations()[9] == "天地盤沒有返吟" and self.find_sike_relations()[2].count("尅") >= 1:
             result = ["涉害", "涉害", self.find_three_pass(self.find_sike_relations()[7][2][2][0])]
             return result
      
-       
-        
         elif shangke.count("下賊上") == 4:
             if self.find_sike_relations()[2].count("被尅") == 1 and self.find_sike_relations()[2].count("尅") == 1:
                 if self.find_sike_relations()[5] == "被尅" or "尅":
                     result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                     return result
                 else:   
                     result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][2][0])]
                     return result
             elif self.find_sike_relations()[2].count("被尅") == 1 and self.find_sike_relations()[2].count("尅") == 0:
                 result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                 return result
             elif self.find_sike_relations()[2].count("被尅") == 0 and self.find_sike_relations()[2].count("尅") == 1:
                 result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
                 return result
+            else:
+                result = ["涉害", "涉害", self.find_three_pass( self.find_sike_relations()[7][2][0][0])]
+                return result
             
-        
         elif shangke.count("下賊上") == 2 and self.find_sike_relations()[9] == "天地盤沒有返吟" and self.find_sike_relations()[2].count("尅") == 0 and self.find_sike_relations()[2].count("被尅") == 0:
             result = ["涉害", "涉害", self.find_three_pass(self.find_sike_relations()[7][2][0][0])]
             return result
         elif shangke.count("下賊上") == 2 and self.find_sike_relations()[9] == "天地盤沒有返吟" and self.find_sike_relations()[2].count("尅") == 0 and self.find_sike_relations()[2].count("被尅") >= 1:
             if  self.find_sike_relations()[5] != "尅":
                 
                 if self.find_sike_relations()[2].count("被尅") > 1 :
@@ -938,14 +937,17 @@
                         else:
                              name = "見機"
                     elif convert_result_v[1][1] == "仲":
                         name = "察微" 
                 chuchuan = convert_result_k[1][0]
                 result = ["涉害", name, self.find_three_pass(chuchuan)]
                 return result
+            else:
+                result = "不適用，或試他法"
+                return result
            
     def yaoke(self):
         if self.find_sike_relations()[3] == "日干支同位":
             chuchuan = "不適用，或試他法" 
             return chuchuan
         elif self.find_sike_relations()[4] == "伏吟":
             chuchuan = "不適用，或試他法" 
@@ -993,47 +995,49 @@
             else:
                 chuchuan = ["遙尅","彈射", self.find_three_pass(sike[self.find_sike_relations()[2].index("被尅")][0] )]
                 return chuchuan
         elif self.find_sike_relations()[2].count("被尅") == 0 and self.find_sike_relations()[2].count("尅") == 0:
             chuchuan = "不適用，或試他法"  
             return chuchuan
     
+    
     def maosing(self):
         sike = self.all_sike()
         sike_list = self.find_sike_relations()[0]
         dayganzhi_yy = self.gangzhi_yinyang(self.daygangzhi[0])
         sikehead = [b[0] for b in sike]
         d =  Counter(sikehead)
         res = [k for k, v in d.items() if v > 1]
-        if len(set(sike)) <4:
-            chuchuan = "不適用，或試他法" 
+        if len(set(sike)) <4 and self.find_sike_relations()[2].count("尅") > 1:
+            chuchuan =  ["昴星", "虎視", [self.sky_n_earth_list().get("酉"), self.sky_n_earth_list().get(self.daygangzhi[1]), self.all_sike()[3][0]]]
             return chuchuan
         elif self.find_sike_relations()[2].count("尅") >0:
             chuchuan = "不適用，或試他法" 
             return chuchuan
         elif sike_list.count("下賊上") == 0 and sike_list.count("上尅下") == 0 :
             if dayganzhi_yy == "陽":
                 try:
                     if len(res[0]) >= 1:
-                        chuchuan = "不適用，或試他法" 
+                        chuchuan =  ["昴星", "虎視", [self.sky_n_earth_list().get("酉"), self.sky_n_earth_list().get(self.daygangzhi[1]), self.all_sike()[3][0]]]
                         return chuchuan
                 except IndexError:
                     if self.find_sike_relations()[6] == "反吟":
                         chuchuan = ["返吟", "無親", [self.yima_dict.get(self.daygangzhi[1]), self.sky_n_earth_list().get(self.daygangzhi[1]), self.sky_n_earth_list().get(self.shigangjigong.get(self.daygangzhi[0])) ]]
                         return chuchuan
                     elif self.find_sike_relations()[6] == "反吟八專":
                         chuchuan = "不適用，或試他法" 
                         return chuchuan
                     else:
                         chuchuan = ["昴星", "虎視", [self.sky_n_earth_list().get("酉"), self.sky_n_earth_list().get(self.daygangzhi[1]), self.all_sike()[3][0]]]
                         return chuchuan
             if dayganzhi_yy == "陰":
                 try:
                     if len(res[0]) >= 1:
-                        chuchuan = "不適用，或試他法"  
+                        ganlivezhi = self.shigangjigong
+                        chuchuan = ["昴星","冬蛇掩目", [self.earth_n_sky_list().get("酉"), self.sky_n_earth_list().get(ganlivezhi.get(self.daygangzhi[0])), self.all_sike()[1][0]]]
                         return chuchuan
                 except IndexError:
                     if self.find_sike_relations()[6] == "反吟":
                         chuchuan = ["返吟","無親", [self.yima_dict.get(self.daygangzhi[1]), self.sky_n_earth_list().get(self.daygangzhi[1]), self.sky_n_earth_list().get(self.shigangjigong.get(self.daygangzhi[0])) ]]
                         return chuchuan
                     elif self.find_sike_relations()[6] == "反吟八專":
                         chuchuan = "不適用，或試他法" 
@@ -1087,15 +1091,15 @@
                 if self.find_sike_relations()[6] == "反吟八專":
                     chuchuan = "不適用，或試他法" 
                     return chuchuan
                 elif self.find_sike_relations()[4] == "伏吟":
                     chuchuan =  "不適用，或試他法" 
                     return chuchuan
                 else:
-                    chuchuan = ["別責", "別責", [a, self.sky_n_earth_list().get(self.shigangjigong.get(self.daygangzhi[0])), self.sky_n_earth_list().get(self.shigangjigong.get(self.daygangzhi[0]))]]
+                    chuchuan = ["別責", "別責", [self.sky_n_earth_list().get(a), self.shigangjigong.get(self.daygangzhi[0]), self.sky_n_earth_list().get(self.shigangjigong.get(self.daygangzhi[0]))]]
                     return chuchuan
         elif self.find_sike_relations()[4] == "伏吟":
             chuchuan =  "不適用，或試他法" 
             return chuchuan
         if sike_list.count("下賊上") + sike_list.count("上尅下") >= 1 :
             chuchuan =  "不適用，或試他法" 
             return chuchuan
@@ -1153,15 +1157,15 @@
             unique_list = [] 
             for x in list1: 
                 if x not in unique_list: 
                     unique_list.append(x) 
                 return x
         sike_list = self.find_sike_relations()
         dayganzhi_yy = self.gangzhi_yinyang(self.daygangzhi[0])
-        if sike_list[4] == "非伏吟":
+        if sike_list[4] == "非伏吟" or len(self.zeike())> 2:
             chuchuan = "不適用，或試他法" 
             return chuchuan
         elif sike_list[4] == "伏吟":
             if sike_list[0].count("上尅下") == 1 or sike_list[0].count("下賊上") == 1:
                 chuchuan = ["伏吟", "不虞",  [unique(sike_list[1])[0], self.ying.get(unique(sike_list[1])[0]), self.ying.get(self.ying.get(unique(sike_list[1])[0])) ]]
                 return chuchuan
             elif sike_list[0].count("上尅下") == 0 and sike_list[0].count("下賊上") == 0:
@@ -1288,8 +1292,8 @@
     tic = time.perf_counter()
     print(d +"     " + h)
     print(Liuren(j, m, d, h).result(0))
     print("    ")
     print(Liuren(j, m, d, h).guiren_order_list(0))
     toc = time.perf_counter()
     print(f"{toc - tic:0.4f} seconds")
-    
+
```

### Comparing `kinliuren-0.1.2.6/kinliuren.egg-info/PKG-INFO` & `kinliuren-0.1.2.7/kinliuren.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: kinliuren
-Version: 0.1.2.6
+Version: 0.1.2.7
 Summary: Dailiuren (大六壬) is one of the three greatest Chinese Divination systems ever.
 Home-page: https://github.com/kentang2017/kinliuren
 Author: Ken Tang
 Author-email: kinyeah@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-﻿# **Python 大六壬 Kinliuren 堅大六壬**
+﻿# **Python 大六壬 Kinliuren 堅大六壬 堅六壬**
 [![Python](https://img.shields.io/pypi/pyversions/kinliuren)](https://pypi.org/project/kinliuren/)
 [![PIP](https://img.shields.io/pypi/v/kinliuren)](https://pypi.org/project/kinliuren/)
 [![Downloads](https://img.shields.io/pypi/dm/kinliuren)](https://pypi.org/project/kinliuren/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
+[![TG Channel](https://img.shields.io/badge/chat-on%20telegram-red)](https://t.me/numerology_coding)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
-![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf/page568-428px-%E7%BA%8C%E4%BF%AE%E5%9B%9B%E5%BA%AB%E5%85%A8%E6%9B%B8%E7%AC%AC1057%E5%86%8A.pdf.jpg "六壬軍帳神機")
 
+![alt text](https://github.com/kentang2017/kinliuren/blob/master/pic/Untitled-33.png)
 ## 1. 導讀 Introduction
 大六壬，或稱六壬神課，簡稱六壬，是中國古老三大占卜術之一。大六壬與奇門遁甲、太乙神數並稱三式。大六壬盛行於漢朝、三國、魏晉南北朝，文人名士多有以此為休閒，常以懷中藏物互相占卜猜測，名曰「射覆」。唐宋以來，明清相繼，相承至今。然六壬演式繁雜，主要在士大夫之間流傳，在民間社會中漸被文王卦所代替。當今社會，在中國大陸、香港和台灣均有一部分人在研習六壬。六壬術傳至日本後，在平安時代由陰陽師安倍晴明發揚光大。為現代算命相術之一。
 
+堅六壬排盤 https://kinliuren.streamlit.app/
+
 Da Liu Ren is a form of Chinese calendrical astrology dating from the later Warring States period. It is also a member of the Three Styles (三式; sānshì; 'three rites') of divination, along with Qi Men Dun Jia (奇门遁甲) and Taiyi (太乙).
 
 In the words of a contemporary Chinese master of Da Liu Ren, the six rén indicate an entire movement of the sexagenary cycle, during which an something may appear, rise to maturity and then decline and disappear. Thus the six rén indicate the life cycle of phenomena. There is a homonym in the Chinese language which carries the meaning of pregnancy and so the six rén also carry the meaning of the birth of a phenomenon.
 
-
 ## 2. 安裝套件 Installation
 ```python
 	pip install kinliuren
 ```
 ## 3. 起課方式 Quickstart
 ```python
 	from kinliuren import kinliuren
-	kinliuren.Liuren( 節氣, 日干支, 時干支).result(0)
-	例如 Liuren("冬至", "丁未", "乙巳")
-{'節氣': '冬至', '日期': '丁未日乙巳時', '格局': ['賊尅', '元首'], '三傳': {'初傳': ['卯', '勾陳', '父母', '空'], '中傳': ['亥', '貴人', '官鬼', '辛'], '末傳': ['未', '太常', '子孫', '丁']}, '四課': {'四課': ['亥卯', '貴人'], '三課': ['卯未', '勾陳'], '二課': ['亥卯', '貴人'], '一課': ['卯丁', '勾陳']}, '天地盤': {'天盤': ['丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌', '亥', '子'], '地盤': ['巳', '午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰'], '天將': ['朱雀', '六合', '勾陳', '青龍', '天空', '白虎', '太常', '玄武', '太陰', '天后', '貴人', '螣蛇']}, '地轉天盤': {'巳': '丑', '午': '寅', '未': '卯', '申': '辰', '酉': '巳', '戌': '午', '亥': '未', '子': '申', '丑': '酉', '寅': '戌', '卯': '亥', '辰': '子'}, '地轉天將': {'巳': '朱雀', '午': '六合', '未': '勾陳', '申': '青龍', '酉': '天空', '戌': '白虎', '亥': '太常', '子': '玄武', '丑': '太陰', '寅': '天后', '卯': '貴人', '辰': '螣蛇'}}
+	kinliuren.Liuren( 節氣, 農曆月份, 日干支, 時干支).result(0)
+	例如 Liuren("驚蟄","二","己未","甲午").result(0)
+{'節氣': '驚蟄', '日期': '己未日甲午時', '格局': ['賊尅', '重審'], '日馬': '巳', '三傳': {'初傳': ['巳', '虎', '父', '丁'], '中傳': ['戌', '雀', '兄', '壬'], '末傳': ['卯', '玄', '官', '乙']}, '四課': {'四課': ['巳子', '虎'], '三課': ['子未', '貴'], '二課': ['巳子', '虎'], '一課': ['子己', '貴']}, '天地盤': {'天盤': ['亥', '子', '丑', '寅', '卯', '辰', '巳', '午', '未', '申', '酉', '戌'], '地盤': ['午', '未', '申', '酉', '戌', '亥', '子', '丑', '寅', '卯', '辰', '巳'], '天將': ['蛇', '貴', '后', '陰', '玄', '常', '虎', '空', '龍', '勾', '合', '雀']}, '地轉天盤': {'午': '亥', '未': '子', '申': '丑', '酉': '寅', '戌': '卯', '亥': '辰', '子': '巳', '丑': '午', '寅': '未', '卯': '申', '辰': '酉', '巳': '戌'}, '地轉天將': {'午': '蛇', '未': '貴', '申': '后', '酉': '陰', '戌': '玄', '亥': '常', '子': '虎', '丑': '空', '寅': '龍', '卯': '勾', '辰': '合', '巳': '雀'}, '神煞': {'天城': '申', '天吏': '寅', '皇書': '寅', '天喜': '戌', '天耳': '申', '戲神': '巳', '遊神': '丑', '天車': '巳', '月馬': '辰', '日馬': '巳', '丁馬': '巳', '日德': '寅', '日祿': '午', '賢貴': '丑', '進神': '卯', '進神二': '酉', '五合': '寅', '支德': '午', '將星': '卯', '六合': '午', '天馬': '申', '聖心': '巳', '天恩': '酉', '天財': '午', '飛廉': '巳', '會神': '戌', '成神': '申', '生氣': '丑', '月合': '戌', '閃電': '丑'}}
 ```
+
+
```

### Comparing `kinliuren-0.1.2.6/setup.py` & `kinliuren-0.1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
    
 setuptools.setup(
     name="kinliuren",
-    version="0.1.2.6",
+    version="0.1.2.7",
     author="Ken Tang",
     author_email="kinyeah@gmail.com",
     install_requires=[            
       ],
 	description="Dailiuren (大六壬) is one of the three greatest Chinese Divination systems ever.",
 	long_description=long_description,
     long_description_content_type="text/markdown",
```

