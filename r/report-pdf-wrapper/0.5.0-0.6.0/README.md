# Comparing `tmp/report_pdf_wrapper-0.5.0-py3-none-any.whl.zip` & `tmp/report_pdf_wrapper-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5375 bytes, number of entries: 7
+Zip file size: 5384 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       68 b- defN 24-May-24 17:55 report_pdf_wrapper/__init__.py
--rw-r--r--  2.0 unx    13193 b- defN 24-May-25 05:22 report_pdf_wrapper/report_pdf_wrapper.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-25 05:23 report_pdf_wrapper-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 24-May-25 05:23 report_pdf_wrapper-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-25 05:23 report_pdf_wrapper-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-25 05:23 report_pdf_wrapper-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      623 b- defN 24-May-25 05:23 report_pdf_wrapper-0.5.0.dist-info/RECORD
-7 files, 15775 bytes uncompressed, 4253 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx    13128 b- defN 24-May-30 01:33 report_pdf_wrapper/report_pdf_wrapper.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-30 01:34 report_pdf_wrapper-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 24-May-30 01:34 report_pdf_wrapper-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 01:34 report_pdf_wrapper-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-30 01:34 report_pdf_wrapper-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 24-May-30 01:34 report_pdf_wrapper-0.6.0.dist-info/RECORD
+7 files, 15710 bytes uncompressed, 4262 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: report_pdf_wrapper/__init__.py
 Comment: 
 
 Filename: report_pdf_wrapper/report_pdf_wrapper.py
 Comment: 
 
-Filename: report_pdf_wrapper-0.5.0.dist-info/LICENSE
+Filename: report_pdf_wrapper-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: report_pdf_wrapper-0.5.0.dist-info/METADATA
+Filename: report_pdf_wrapper-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: report_pdf_wrapper-0.5.0.dist-info/WHEEL
+Filename: report_pdf_wrapper-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: report_pdf_wrapper-0.5.0.dist-info/top_level.txt
+Filename: report_pdf_wrapper-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: report_pdf_wrapper-0.5.0.dist-info/RECORD
+Filename: report_pdf_wrapper-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## report_pdf_wrapper/report_pdf_wrapper.py

```diff
@@ -216,29 +216,28 @@
             point = Point(385, i)
             # add material item
             field = fitz.Widget()
             field.field_name = f"material_{line}_field"
             field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
             field.text_maxlen = 100
             field.rect = fitz.Rect(68, point.y - 2, 275, point.y + 15)
-            self.draw_line(Point(60, i - 3), Point(520, i - 3))
+            self.draw_line(Point(60, i - 3), Point(340, i - 3))
             self.page.add_widget(field)
             # add quantity item
             field = fitz.Widget()
             field.field_name = f"quantity_{line}_field"
             field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
             field.text_maxlen = 10
             field.rect = fitz.Rect(280, point.y - 2, 330, point.y + 15)
             self.page.add_widget(field)
-            self.page.insert_text(Point(350, point.y + 10), "Yes", fontsize=10)
-            self._add_checkbox_widget(Point(375, point.y + 2), f"completed_{line}_checkbox", (0, 0, 0))
-            self.page.insert_text(Point(430, point.y + 10), "More service", fontsize=10, color=getColor("red"))
-            self._add_checkbox_widget(Point(500, point.y + 2), f"service_{line}_checkbox", getColor("red"))
-
             line += 1
+        self.page.insert_text(Point(353, 622), "Yes", fontsize=10)
+        self._add_checkbox_widget(Point(378, 614), f"completed_checkbox", (0, 0, 0))
+        self.page.insert_text(Point(427, 622), "More service", fontsize=10, color=getColor("red"))
+        self._add_checkbox_widget(Point(497, 614), f"service_checkbox", getColor("red"))
 
     def draw_underline(self, rect):
         start = (rect.x0, rect.y1)
         end = (rect.x1, rect.y1)
         self.page.draw_line(start, end, color=getColor("black"), width=1)
 
     def draw_box(self, p1, p2, p3, p4):
```

## Comparing `report_pdf_wrapper-0.5.0.dist-info/LICENSE` & `report_pdf_wrapper-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `report_pdf_wrapper-0.5.0.dist-info/METADATA` & `report_pdf_wrapper-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-pdf-wrapper
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simple pip module for creating generic PDF reports.
 Home-page: https://github.com/nr-software/Report-PDF-Creation.git
 Author: Alex Nuccio
 Author-email: nrsoftwareservices@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `report_pdf_wrapper-0.5.0.dist-info/RECORD` & `report_pdf_wrapper-0.6.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 report_pdf_wrapper/__init__.py,sha256=bOUIDadGljW4JgkMxkcJnQ9guJ5BF_AgrA3tHNOr8y8,68
-report_pdf_wrapper/report_pdf_wrapper.py,sha256=3k3bcYWy2AG-ThIjaruo5QQ3VPGn-hHs8o7jrMhqYZc,13193
-report_pdf_wrapper-0.5.0.dist-info/LICENSE,sha256=J45dd5o-jpQZlgZvfs77QxFtQ9WxrpBY6OYYrpb_bKk,1068
-report_pdf_wrapper-0.5.0.dist-info/METADATA,sha256=_SErqwrq6RIKXq-8OB3eeVDZT7YsbdzKfL7P2Cx3_48,712
-report_pdf_wrapper-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-report_pdf_wrapper-0.5.0.dist-info/top_level.txt,sha256=7RK52XVFxPTqtewESdqMKt6-7wpBzJducMXUk4eeinc,19
-report_pdf_wrapper-0.5.0.dist-info/RECORD,,
+report_pdf_wrapper/report_pdf_wrapper.py,sha256=Lmn2vI6vXg8BVb2vgYiW64cd60hEYH8WtpCcB14p60U,13128
+report_pdf_wrapper-0.6.0.dist-info/LICENSE,sha256=J45dd5o-jpQZlgZvfs77QxFtQ9WxrpBY6OYYrpb_bKk,1068
+report_pdf_wrapper-0.6.0.dist-info/METADATA,sha256=hfpzL6iFLi41PneX_4ASWko4bjFGxbcm-dyFcgCxFpU,712
+report_pdf_wrapper-0.6.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+report_pdf_wrapper-0.6.0.dist-info/top_level.txt,sha256=7RK52XVFxPTqtewESdqMKt6-7wpBzJducMXUk4eeinc,19
+report_pdf_wrapper-0.6.0.dist-info/RECORD,,
```

