# Comparing `tmp/alibabacloud_green20220302-2.2.6.tar.gz` & `tmp/alibabacloud_green20220302-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-2.2.6.tar", last modified: Mon May 27 08:14:21 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-2.2.7.tar", last modified: Thu May 30 17:13:35 2024, max compression
```

## Comparing `alibabacloud_green20220302-2.2.6.tar` & `alibabacloud_green20220302-2.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63849 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   125248 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63849 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   138529 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-05-30 17:13:35.000000 alibabacloud_green20220302-2.2.7/setup.py
```

### Comparing `alibabacloud_green20220302-2.2.6/ChangeLog.md` & `alibabacloud_green20220302-2.2.7/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-05-27 Version: 2.2.6
+- Update API TextModerationPlus: update response param.
+
+
 2024-05-11 Version: 2.2.5
 - Update API ImageModeration: update response param.
 
 
 2024-04-19 Version: 2.2.4
 - Update API ImageModeration: update response param.
```

### Comparing `alibabacloud_green20220302-2.2.6/LICENSE` & `alibabacloud_green20220302-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.6/PKG-INFO` & `alibabacloud_green20220302-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 2.2.6
+Version: 2.2.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.6/README-CN.md` & `alibabacloud_green20220302-2.2.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.6/README.md` & `alibabacloud_green20220302-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-2.2.7/alibabacloud_green20220302/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1713,14 +1713,181 @@
         if m.get('Service') is not None:
             self.service = m.get('Service')
         if m.get('ServiceParameters') is not None:
             self.service_parameters = m.get('ServiceParameters')
         return self
 
 
+class ImageModerationResponseBodyDataExtCustomImage(TeaModel):
+    def __init__(
+        self,
+        image_id: str = None,
+        lib_id: str = None,
+        lib_name: str = None,
+    ):
+        self.image_id = image_id
+        self.lib_id = lib_id
+        self.lib_name = lib_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
+        if self.lib_id is not None:
+            result['LibId'] = self.lib_id
+        if self.lib_name is not None:
+            result['LibName'] = self.lib_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
+        if m.get('LibId') is not None:
+            self.lib_id = m.get('LibId')
+        if m.get('LibName') is not None:
+            self.lib_name = m.get('LibName')
+        return self
+
+
+class ImageModerationResponseBodyDataExtLogoDataLocation(TeaModel):
+    def __init__(
+        self,
+        h: int = None,
+        w: int = None,
+        x: int = None,
+        y: int = None,
+    ):
+        self.h = h
+        self.w = w
+        self.x = x
+        self.y = y
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.h is not None:
+            result['H'] = self.h
+        if self.w is not None:
+            result['W'] = self.w
+        if self.x is not None:
+            result['X'] = self.x
+        if self.y is not None:
+            result['Y'] = self.y
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('H') is not None:
+            self.h = m.get('H')
+        if m.get('W') is not None:
+            self.w = m.get('W')
+        if m.get('X') is not None:
+            self.x = m.get('X')
+        if m.get('Y') is not None:
+            self.y = m.get('Y')
+        return self
+
+
+class ImageModerationResponseBodyDataExtLogoDataLogo(TeaModel):
+    def __init__(
+        self,
+        confidence: float = None,
+        label: str = None,
+        name: str = None,
+    ):
+        self.confidence = confidence
+        self.label = label
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.confidence is not None:
+            result['Confidence'] = self.confidence
+        if self.label is not None:
+            result['Label'] = self.label
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Confidence') is not None:
+            self.confidence = m.get('Confidence')
+        if m.get('Label') is not None:
+            self.label = m.get('Label')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class ImageModerationResponseBodyDataExtLogoData(TeaModel):
+    def __init__(
+        self,
+        location: ImageModerationResponseBodyDataExtLogoDataLocation = None,
+        logo: List[ImageModerationResponseBodyDataExtLogoDataLogo] = None,
+    ):
+        self.location = location
+        self.logo = logo
+
+    def validate(self):
+        if self.location:
+            self.location.validate()
+        if self.logo:
+            for k in self.logo:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.location is not None:
+            result['Location'] = self.location.to_map()
+        result['Logo'] = []
+        if self.logo is not None:
+            for k in self.logo:
+                result['Logo'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Location') is not None:
+            temp_model = ImageModerationResponseBodyDataExtLogoDataLocation()
+            self.location = temp_model.from_map(m['Location'])
+        self.logo = []
+        if m.get('Logo') is not None:
+            for k in m.get('Logo'):
+                temp_model = ImageModerationResponseBodyDataExtLogoDataLogo()
+                self.logo.append(temp_model.from_map(k))
+        return self
+
+
 class ImageModerationResponseBodyDataExtOcrResultLocation(TeaModel):
     def __init__(
         self,
         h: int = None,
         w: int = None,
         x: int = None,
         y: int = None,
@@ -1793,14 +1960,47 @@
             temp_model = ImageModerationResponseBodyDataExtOcrResultLocation()
             self.location = temp_model.from_map(m['Location'])
         if m.get('Text') is not None:
             self.text = m.get('Text')
         return self
 
 
+class ImageModerationResponseBodyDataExtPublicFigure(TeaModel):
+    def __init__(
+        self,
+        figure_id: str = None,
+        figure_name: str = None,
+    ):
+        self.figure_id = figure_id
+        self.figure_name = figure_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.figure_id is not None:
+            result['FigureId'] = self.figure_id
+        if self.figure_name is not None:
+            result['FigureName'] = self.figure_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FigureId') is not None:
+            self.figure_id = m.get('FigureId')
+        if m.get('FigureName') is not None:
+            self.figure_name = m.get('FigureName')
+        return self
+
+
 class ImageModerationResponseBodyDataExtRecognition(TeaModel):
     def __init__(
         self,
         classification: str = None,
         confidence: float = None,
     ):
         self.classification = classification
@@ -1826,61 +2026,290 @@
         if m.get('Classification') is not None:
             self.classification = m.get('Classification')
         if m.get('Confidence') is not None:
             self.confidence = m.get('Confidence')
         return self
 
 
+class ImageModerationResponseBodyDataExtTextInImageCustomText(TeaModel):
+    def __init__(
+        self,
+        key_words: str = None,
+        lib_id: str = None,
+        lib_name: str = None,
+    ):
+        self.key_words = key_words
+        self.lib_id = lib_id
+        self.lib_name = lib_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key_words is not None:
+            result['KeyWords'] = self.key_words
+        if self.lib_id is not None:
+            result['LibId'] = self.lib_id
+        if self.lib_name is not None:
+            result['LibName'] = self.lib_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('KeyWords') is not None:
+            self.key_words = m.get('KeyWords')
+        if m.get('LibId') is not None:
+            self.lib_id = m.get('LibId')
+        if m.get('LibName') is not None:
+            self.lib_name = m.get('LibName')
+        return self
+
+
+class ImageModerationResponseBodyDataExtTextInImageOcrResultLocation(TeaModel):
+    def __init__(
+        self,
+        h: int = None,
+        w: int = None,
+        x: int = None,
+        y: int = None,
+    ):
+        self.h = h
+        self.w = w
+        self.x = x
+        self.y = y
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.h is not None:
+            result['H'] = self.h
+        if self.w is not None:
+            result['W'] = self.w
+        if self.x is not None:
+            result['X'] = self.x
+        if self.y is not None:
+            result['Y'] = self.y
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('H') is not None:
+            self.h = m.get('H')
+        if m.get('W') is not None:
+            self.w = m.get('W')
+        if m.get('X') is not None:
+            self.x = m.get('X')
+        if m.get('Y') is not None:
+            self.y = m.get('Y')
+        return self
+
+
+class ImageModerationResponseBodyDataExtTextInImageOcrResult(TeaModel):
+    def __init__(
+        self,
+        location: ImageModerationResponseBodyDataExtTextInImageOcrResultLocation = None,
+        text: str = None,
+    ):
+        self.location = location
+        self.text = text
+
+    def validate(self):
+        if self.location:
+            self.location.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.location is not None:
+            result['Location'] = self.location.to_map()
+        if self.text is not None:
+            result['Text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Location') is not None:
+            temp_model = ImageModerationResponseBodyDataExtTextInImageOcrResultLocation()
+            self.location = temp_model.from_map(m['Location'])
+        if m.get('Text') is not None:
+            self.text = m.get('Text')
+        return self
+
+
+class ImageModerationResponseBodyDataExtTextInImage(TeaModel):
+    def __init__(
+        self,
+        custom_text: List[ImageModerationResponseBodyDataExtTextInImageCustomText] = None,
+        ocr_result: List[ImageModerationResponseBodyDataExtTextInImageOcrResult] = None,
+        risk_word: List[str] = None,
+    ):
+        self.custom_text = custom_text
+        self.ocr_result = ocr_result
+        self.risk_word = risk_word
+
+    def validate(self):
+        if self.custom_text:
+            for k in self.custom_text:
+                if k:
+                    k.validate()
+        if self.ocr_result:
+            for k in self.ocr_result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CustomText'] = []
+        if self.custom_text is not None:
+            for k in self.custom_text:
+                result['CustomText'].append(k.to_map() if k else None)
+        result['OcrResult'] = []
+        if self.ocr_result is not None:
+            for k in self.ocr_result:
+                result['OcrResult'].append(k.to_map() if k else None)
+        if self.risk_word is not None:
+            result['RiskWord'] = self.risk_word
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.custom_text = []
+        if m.get('CustomText') is not None:
+            for k in m.get('CustomText'):
+                temp_model = ImageModerationResponseBodyDataExtTextInImageCustomText()
+                self.custom_text.append(temp_model.from_map(k))
+        self.ocr_result = []
+        if m.get('OcrResult') is not None:
+            for k in m.get('OcrResult'):
+                temp_model = ImageModerationResponseBodyDataExtTextInImageOcrResult()
+                self.ocr_result.append(temp_model.from_map(k))
+        if m.get('RiskWord') is not None:
+            self.risk_word = m.get('RiskWord')
+        return self
+
+
 class ImageModerationResponseBodyDataExt(TeaModel):
     def __init__(
         self,
+        custom_image: List[ImageModerationResponseBodyDataExtCustomImage] = None,
+        logo_data: List[ImageModerationResponseBodyDataExtLogoData] = None,
         ocr_result: List[ImageModerationResponseBodyDataExtOcrResult] = None,
+        public_figure: List[ImageModerationResponseBodyDataExtPublicFigure] = None,
         recognition: List[ImageModerationResponseBodyDataExtRecognition] = None,
+        text_in_image: ImageModerationResponseBodyDataExtTextInImage = None,
     ):
+        self.custom_image = custom_image
+        self.logo_data = logo_data
         self.ocr_result = ocr_result
+        self.public_figure = public_figure
         self.recognition = recognition
+        self.text_in_image = text_in_image
 
     def validate(self):
+        if self.custom_image:
+            for k in self.custom_image:
+                if k:
+                    k.validate()
+        if self.logo_data:
+            for k in self.logo_data:
+                if k:
+                    k.validate()
         if self.ocr_result:
             for k in self.ocr_result:
                 if k:
                     k.validate()
+        if self.public_figure:
+            for k in self.public_figure:
+                if k:
+                    k.validate()
         if self.recognition:
             for k in self.recognition:
                 if k:
                     k.validate()
+        if self.text_in_image:
+            self.text_in_image.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['CustomImage'] = []
+        if self.custom_image is not None:
+            for k in self.custom_image:
+                result['CustomImage'].append(k.to_map() if k else None)
+        result['LogoData'] = []
+        if self.logo_data is not None:
+            for k in self.logo_data:
+                result['LogoData'].append(k.to_map() if k else None)
         result['OcrResult'] = []
         if self.ocr_result is not None:
             for k in self.ocr_result:
                 result['OcrResult'].append(k.to_map() if k else None)
+        result['PublicFigure'] = []
+        if self.public_figure is not None:
+            for k in self.public_figure:
+                result['PublicFigure'].append(k.to_map() if k else None)
         result['Recognition'] = []
         if self.recognition is not None:
             for k in self.recognition:
                 result['Recognition'].append(k.to_map() if k else None)
+        if self.text_in_image is not None:
+            result['TextInImage'] = self.text_in_image.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.custom_image = []
+        if m.get('CustomImage') is not None:
+            for k in m.get('CustomImage'):
+                temp_model = ImageModerationResponseBodyDataExtCustomImage()
+                self.custom_image.append(temp_model.from_map(k))
+        self.logo_data = []
+        if m.get('LogoData') is not None:
+            for k in m.get('LogoData'):
+                temp_model = ImageModerationResponseBodyDataExtLogoData()
+                self.logo_data.append(temp_model.from_map(k))
         self.ocr_result = []
         if m.get('OcrResult') is not None:
             for k in m.get('OcrResult'):
                 temp_model = ImageModerationResponseBodyDataExtOcrResult()
                 self.ocr_result.append(temp_model.from_map(k))
+        self.public_figure = []
+        if m.get('PublicFigure') is not None:
+            for k in m.get('PublicFigure'):
+                temp_model = ImageModerationResponseBodyDataExtPublicFigure()
+                self.public_figure.append(temp_model.from_map(k))
         self.recognition = []
         if m.get('Recognition') is not None:
             for k in m.get('Recognition'):
                 temp_model = ImageModerationResponseBodyDataExtRecognition()
                 self.recognition.append(temp_model.from_map(k))
+        if m.get('TextInImage') is not None:
+            temp_model = ImageModerationResponseBodyDataExtTextInImage()
+            self.text_in_image = temp_model.from_map(m['TextInImage'])
         return self
 
 
 class ImageModerationResponseBodyDataResult(TeaModel):
     def __init__(
         self,
         confidence: float = None,
```

### Comparing `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-2.2.7/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 2.2.6
+Version: 2.2.7
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.6/setup.py` & `alibabacloud_green20220302-2.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 27/05/2024
+Created on 30/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```

