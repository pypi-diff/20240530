# Comparing `tmp/kinqimen-0.0.6.5.tar.gz` & `tmp/kinqimen-0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinqimen-0.0.6.5.tar", last modified: Mon Oct  9 04:32:31 2023, max compression
+gzip compressed data, was "kinqimen-0.0.6.6.tar", last modified: Thu May 30 06:15:05 2024, max compression
```

## Comparing `kinqimen-0.0.6.5.tar` & `kinqimen-0.0.6.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-10-09 04:32:31.644031 kinqimen-0.0.6.5/
--rw-rw-rw-   0        0        0     4428 2023-10-09 04:32:31.645028 kinqimen-0.0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     3977 2020-06-01 09:52:28.000000 kinqimen-0.0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-10-09 04:32:31.591061 kinqimen-0.0.6.5/kinqimen/
--rw-rw-rw-   0        0        0        3 2019-08-16 07:28:34.000000 kinqimen-0.0.6.5/kinqimen/__init__.py
--rw-rw-rw-   0        0        0    16433 2023-10-04 08:27:16.000000 kinqimen-0.0.6.5/kinqimen/config.py
--rw-rw-rw-   0        0        0    13682 2023-10-04 08:27:16.000000 kinqimen-0.0.6.5/kinqimen/kinqimen.py
-drwxrwxrwx   0        0        0        0 2023-10-09 04:32:31.641031 kinqimen-0.0.6.5/kinqimen.egg-info/
--rw-rw-rw-   0        0        0     4428 2023-10-09 04:32:31.000000 kinqimen-0.0.6.5/kinqimen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-10-09 04:32:31.000000 kinqimen-0.0.6.5/kinqimen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-09 04:32:31.000000 kinqimen-0.0.6.5/kinqimen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-10-09 04:32:31.000000 kinqimen-0.0.6.5/kinqimen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-09 04:32:31.000000 kinqimen-0.0.6.5/kinqimen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-09 04:32:31.648026 kinqimen-0.0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-10-09 04:32:12.000000 kinqimen-0.0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:15:05.555318 kinqimen-0.0.6.6/
+-rw-rw-rw-   0        0        0     4942 2024-05-30 06:15:05.553316 kinqimen-0.0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4433 2024-05-30 01:34:36.000000 kinqimen-0.0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:15:05.513691 kinqimen-0.0.6.6/kinqimen/
+-rw-rw-rw-   0        0        0        3 2019-08-16 07:28:34.000000 kinqimen-0.0.6.6/kinqimen/__init__.py
+-rw-rw-rw-   0        0        0    34604 2024-05-30 01:40:48.000000 kinqimen-0.0.6.6/kinqimen/config.py
+-rw-rw-rw-   0        0        0    31768 2024-05-30 01:34:36.000000 kinqimen-0.0.6.6/kinqimen/kinqimen.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:15:05.550670 kinqimen-0.0.6.6/kinqimen.egg-info/
+-rw-rw-rw-   0        0        0     4942 2024-05-30 06:15:05.000000 kinqimen-0.0.6.6/kinqimen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-30 06:15:05.000000 kinqimen-0.0.6.6/kinqimen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:15:05.000000 kinqimen-0.0.6.6/kinqimen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-30 06:15:05.000000 kinqimen-0.0.6.6/kinqimen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 06:15:05.000000 kinqimen-0.0.6.6/kinqimen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:15:05.555318 kinqimen-0.0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-30 06:14:48.000000 kinqimen-0.0.6.6/setup.py
```

### Comparing `kinqimen-0.0.6.5/PKG-INFO` & `kinqimen-0.0.6.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: kinqimen
-Version: 0.0.6.5
+Version: 0.0.6.6
 Summary: Qimendunjia (奇門遁甲) is one of the three greatest Chinese Divination systems ever.
 Home-page: https://github.com/kentang2017/kinqimen
 Author: Ken Tang
 Author-email: kinyeah@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: sxtwl==2.0.6
+Requires-Dist: ephem==4.1.3
 
 ﻿# **Python Qimendunjia Kinqimen Python 奇門遁甲 堅奇門**
 
-簡單時家奇門起盤 A simple Qimendunjia in Chinese hour-based system for prediction.
+![alt text](https://github.com/kentang2017/kinqimen/blob/master/pic/Untitled-22.png)
+簡單金函玉鏡、時家奇門、刻家奇門的奇門遁甲起盤 A simple python package of Qimendunjia in Chinese hour-based system, minute-based system and golden letter jade mirror style Qimendunjia for prediction.
+
+堅奇門排盤 https://kinqimen.streamlitapp.com
 
 [![Python](https://img.shields.io/pypi/pyversions/kinqimen)](https://pypi.org/project/kinqimen/)
 [![PIP](https://img.shields.io/pypi/v/kinqimen)](https://pypi.org/project/kinqimen/)
 [![Downloads](https://img.shields.io/pypi/dm/kinqimen)](https://pypi.org/project/kinqimen/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page123-452px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page104-444px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 
 
-
-
 ## **1. 導讀 Introduction**︰
 奇門遁甲與大六壬、太乙神數並稱三式。為中國神秘學中預測學的一個特有門類。乃利用洛書軌跡，九宮八卦以及五行相生相剋的道理，來預測地理方向的優劣，進而規劃一個人的行程，最終達到對自己最有利的目的，為算命相術所兼用。奇門遁甲以乙、丙、丁稱為三奇；以開、休、生、傷、杜、景、驚、死稱為八門，故名「奇門」。天干中「甲」最尊貴而不顯露，六甲(甲子、甲戌、甲申、甲午、甲辰、甲寅)常隱藏於「戊、己、庚、辛、壬、癸」六儀之內，三奇、六儀分布九宮，而甲不獨占一宮，故名「遁甲」。在古代民間流傳只有帝王附近如軍師、欽天監、國師等重要大臣才通曉奇門遁甲之術。
 
 Qimen Dunjia is an ancient form of divination from China. It is one of the Three Styles (三式; sānshì; 'three rites') of Chinese divination, with DaLiuRen and TaiYi Shen Shu. Over the centuries of Chinese history, Qimen Dunjia grew in popularity and was expanded to include a number of other types of divination, including medical divination, matchmaking, childbirth, travel, personal fortunes, and today includes contemporary applications, most notably that of business and finance. 
 
 Qimen Dunjia is based on astronomical observations, and consists of various aspects of Chinese metaphysics, including the doctrines of yin and yang, five elements, the eight trigrams, the ten Heavenly Stems and the twelve Earthly Branches, as well as the twenty-four solar terms. The Qimen Dunjia cosmic board consists of a 3 × 3 magic square of nine palaces (九宫), which includes a Heaven and Earth plate, a spirit plate, eight gates and a star plate. The various symbols rotate around the palaces with each double-hour of the day, making a total of 1,080 different configurations of the Qimen Dunjia cosmic board. These situations (局; jú) are recycled four times per year, and are divided between the Yin and Yang halves of the year. Qimen Dunjia is time-sensitive. The analyst makes reference to the configuration of the cosmic board at the time when a question is posed, or for birth times of individuals or corporate entities, such as businesses or nations. At times, the same or very similar configurations of the cosmic board will appear in relation to the same series of questions or problems.
 
 ## **2. 安裝套件 Installation**
 
 ```python
+	pip install sxtwl
 	pip install kinqimen
 ```
 
 ## **3. 起課方式 Quickstart**
 ```python
 	from kinqimen import kinqimen
-	kinqimen.Qimen(year, month, day, hour).pan()
+
+	kinqimen.Qimen(year, month, day, hour).pan(1) #1:拆補 2:置閏
+	kinqimenQimen(year, month, day, hour).gpan() (金函日家)
+	kinqimen.Qimen(year, month, day, hour).overall() (時家奇門 + 金函日家)
 	
 ```
```

### Comparing `kinqimen-0.0.6.5/README.md` & `kinqimen-0.0.6.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 ﻿# **Python Qimendunjia Kinqimen Python 奇門遁甲 堅奇門**
 
-簡單時家奇門起盤 A simple Qimendunjia in Chinese hour-based system for prediction.
+![alt text](https://github.com/kentang2017/kinqimen/blob/master/pic/Untitled-22.png)
+簡單金函玉鏡、時家奇門、刻家奇門的奇門遁甲起盤 A simple python package of Qimendunjia in Chinese hour-based system, minute-based system and golden letter jade mirror style Qimendunjia for prediction.
+
+堅奇門排盤 https://kinqimen.streamlitapp.com
 
 [![Python](https://img.shields.io/pypi/pyversions/kinqimen)](https://pypi.org/project/kinqimen/)
 [![PIP](https://img.shields.io/pypi/v/kinqimen)](https://pypi.org/project/kinqimen/)
 [![Downloads](https://img.shields.io/pypi/dm/kinqimen)](https://pypi.org/project/kinqimen/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page123-452px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page104-444px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 
 
-
-
 ## **1. 導讀 Introduction**︰
 奇門遁甲與大六壬、太乙神數並稱三式。為中國神秘學中預測學的一個特有門類。乃利用洛書軌跡，九宮八卦以及五行相生相剋的道理，來預測地理方向的優劣，進而規劃一個人的行程，最終達到對自己最有利的目的，為算命相術所兼用。奇門遁甲以乙、丙、丁稱為三奇；以開、休、生、傷、杜、景、驚、死稱為八門，故名「奇門」。天干中「甲」最尊貴而不顯露，六甲(甲子、甲戌、甲申、甲午、甲辰、甲寅)常隱藏於「戊、己、庚、辛、壬、癸」六儀之內，三奇、六儀分布九宮，而甲不獨占一宮，故名「遁甲」。在古代民間流傳只有帝王附近如軍師、欽天監、國師等重要大臣才通曉奇門遁甲之術。
 
 Qimen Dunjia is an ancient form of divination from China. It is one of the Three Styles (三式; sānshì; 'three rites') of Chinese divination, with DaLiuRen and TaiYi Shen Shu. Over the centuries of Chinese history, Qimen Dunjia grew in popularity and was expanded to include a number of other types of divination, including medical divination, matchmaking, childbirth, travel, personal fortunes, and today includes contemporary applications, most notably that of business and finance. 
 
 Qimen Dunjia is based on astronomical observations, and consists of various aspects of Chinese metaphysics, including the doctrines of yin and yang, five elements, the eight trigrams, the ten Heavenly Stems and the twelve Earthly Branches, as well as the twenty-four solar terms. The Qimen Dunjia cosmic board consists of a 3 × 3 magic square of nine palaces (九宫), which includes a Heaven and Earth plate, a spirit plate, eight gates and a star plate. The various symbols rotate around the palaces with each double-hour of the day, making a total of 1,080 different configurations of the Qimen Dunjia cosmic board. These situations (局; jú) are recycled four times per year, and are divided between the Yin and Yang halves of the year. Qimen Dunjia is time-sensitive. The analyst makes reference to the configuration of the cosmic board at the time when a question is posed, or for birth times of individuals or corporate entities, such as businesses or nations. At times, the same or very similar configurations of the cosmic board will appear in relation to the same series of questions or problems.
 
 ## **2. 安裝套件 Installation**
 
 ```python
+	pip install sxtwl
 	pip install kinqimen
 ```
 
 ## **3. 起課方式 Quickstart**
 ```python
 	from kinqimen import kinqimen
-	kinqimen.Qimen(year, month, day, hour).pan()
+
+	kinqimen.Qimen(year, month, day, hour).pan(1) #1:拆補 2:置閏
+	kinqimenQimen(year, month, day, hour).gpan() (金函日家)
+	kinqimen.Qimen(year, month, day, hour).overall() (時家奇門 + 金函日家)
 	
 ```
```

### Comparing `kinqimen-0.0.6.5/kinqimen.egg-info/PKG-INFO` & `kinqimen-0.0.6.6/kinqimen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: kinqimen
-Version: 0.0.6.5
+Version: 0.0.6.6
 Summary: Qimendunjia (奇門遁甲) is one of the three greatest Chinese Divination systems ever.
 Home-page: https://github.com/kentang2017/kinqimen
 Author: Ken Tang
 Author-email: kinyeah@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: sxtwl==2.0.6
+Requires-Dist: ephem==4.1.3
 
 ﻿# **Python Qimendunjia Kinqimen Python 奇門遁甲 堅奇門**
 
-簡單時家奇門起盤 A simple Qimendunjia in Chinese hour-based system for prediction.
+![alt text](https://github.com/kentang2017/kinqimen/blob/master/pic/Untitled-22.png)
+簡單金函玉鏡、時家奇門、刻家奇門的奇門遁甲起盤 A simple python package of Qimendunjia in Chinese hour-based system, minute-based system and golden letter jade mirror style Qimendunjia for prediction.
+
+堅奇門排盤 https://kinqimen.streamlitapp.com
 
 [![Python](https://img.shields.io/pypi/pyversions/kinqimen)](https://pypi.org/project/kinqimen/)
 [![PIP](https://img.shields.io/pypi/v/kinqimen)](https://pypi.org/project/kinqimen/)
 [![Downloads](https://img.shields.io/pypi/dm/kinqimen)](https://pypi.org/project/kinqimen/)
-[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
+[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/haizhonggum)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;
 
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page123-452px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu/page104-444px-CADAL06056497_%E9%81%81%E7%94%B2%E6%BC%94%E7%BE%A9%C2%B7%E5%8D%B7%E4%B8%89~%E5%8D%B7%E5%9B%9B.djvu.jpg "遁甲演義陰遁七局排盤")
 
 
-
-
 ## **1. 導讀 Introduction**︰
 奇門遁甲與大六壬、太乙神數並稱三式。為中國神秘學中預測學的一個特有門類。乃利用洛書軌跡，九宮八卦以及五行相生相剋的道理，來預測地理方向的優劣，進而規劃一個人的行程，最終達到對自己最有利的目的，為算命相術所兼用。奇門遁甲以乙、丙、丁稱為三奇；以開、休、生、傷、杜、景、驚、死稱為八門，故名「奇門」。天干中「甲」最尊貴而不顯露，六甲(甲子、甲戌、甲申、甲午、甲辰、甲寅)常隱藏於「戊、己、庚、辛、壬、癸」六儀之內，三奇、六儀分布九宮，而甲不獨占一宮，故名「遁甲」。在古代民間流傳只有帝王附近如軍師、欽天監、國師等重要大臣才通曉奇門遁甲之術。
 
 Qimen Dunjia is an ancient form of divination from China. It is one of the Three Styles (三式; sānshì; 'three rites') of Chinese divination, with DaLiuRen and TaiYi Shen Shu. Over the centuries of Chinese history, Qimen Dunjia grew in popularity and was expanded to include a number of other types of divination, including medical divination, matchmaking, childbirth, travel, personal fortunes, and today includes contemporary applications, most notably that of business and finance. 
 
 Qimen Dunjia is based on astronomical observations, and consists of various aspects of Chinese metaphysics, including the doctrines of yin and yang, five elements, the eight trigrams, the ten Heavenly Stems and the twelve Earthly Branches, as well as the twenty-four solar terms. The Qimen Dunjia cosmic board consists of a 3 × 3 magic square of nine palaces (九宫), which includes a Heaven and Earth plate, a spirit plate, eight gates and a star plate. The various symbols rotate around the palaces with each double-hour of the day, making a total of 1,080 different configurations of the Qimen Dunjia cosmic board. These situations (局; jú) are recycled four times per year, and are divided between the Yin and Yang halves of the year. Qimen Dunjia is time-sensitive. The analyst makes reference to the configuration of the cosmic board at the time when a question is posed, or for birth times of individuals or corporate entities, such as businesses or nations. At times, the same or very similar configurations of the cosmic board will appear in relation to the same series of questions or problems.
 
 ## **2. 安裝套件 Installation**
 
 ```python
+	pip install sxtwl
 	pip install kinqimen
 ```
 
 ## **3. 起課方式 Quickstart**
 ```python
 	from kinqimen import kinqimen
-	kinqimen.Qimen(year, month, day, hour).pan()
+
+	kinqimen.Qimen(year, month, day, hour).pan(1) #1:拆補 2:置閏
+	kinqimenQimen(year, month, day, hour).gpan() (金函日家)
+	kinqimen.Qimen(year, month, day, hour).overall() (時家奇門 + 金函日家)
 	
 ```
```

### Comparing `kinqimen-0.0.6.5/setup.py` & `kinqimen-0.0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
    
 setuptools.setup(
     name="kinqimen",
-    version="0.0.6.5",
+    version="0.0.6.6",
     author="Ken Tang",
     author_email="kinyeah@gmail.com",
     install_requires=["sxtwl==2.0.6", "ephem==4.1.3",
       ],
 	description="Qimendunjia (奇門遁甲) is one of the three greatest Chinese Divination systems ever.",
 	long_description=long_description,
     long_description_content_type="text/markdown",
```

