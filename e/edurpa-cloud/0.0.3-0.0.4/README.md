# Comparing `tmp/edurpa_cloud-0.0.3-py3-none-any.whl.zip` & `tmp/edurpa_cloud-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11190 bytes, number of entries: 14
+Zip file size: 10963 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-17 16:24 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat    13103 b- defN 24-Apr-18 09:37 EduRPA/Google/Classroom.py
 -rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-23 16:12 EduRPA/Google/CustomOAuth.py
--rw-rw-rw-  2.0 fat    11964 b- defN 24-Apr-18 09:38 EduRPA/Google/Form.py
+-rw-rw-rw-  2.0 fat    10019 b- defN 24-May-30 11:50 EduRPA/Google/Form.py
 -rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-21 05:45 EduRPA/Google/Utils.py
 -rw-rw-rw-  2.0 fat      469 b- defN 24-Apr-21 13:23 EduRPA/Google/__init__.py
 -rw-rw-rw-  2.0 fat     1603 b- defN 24-May-28 12:25 EduRPA/Storage/S3Storage.py
 -rw-rw-rw-  2.0 fat     1575 b- defN 24-Apr-28 06:10 EduRPA/Storage/Storage.py
 -rw-rw-rw-  2.0 fat      312 b- defN 24-May-25 13:07 EduRPA/Storage/__init__.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      716 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1136 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/RECORD
-14 files, 33890 bytes uncompressed, 9300 bytes compressed:  72.6%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-30 11:51 edurpa_cloud-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      716 b- defN 24-May-30 11:51 edurpa_cloud-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-30 11:51 edurpa_cloud-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-30 11:51 edurpa_cloud-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1136 b- defN 24-May-30 11:51 edurpa_cloud-0.0.4.dist-info/RECORD
+14 files, 31945 bytes uncompressed, 9073 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: EduRPA/Storage/Storage.py
 Comment: 
 
 Filename: EduRPA/Storage/__init__.py
 Comment: 
 
-Filename: edurpa_cloud-0.0.3.dist-info/LICENSE
+Filename: edurpa_cloud-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_cloud-0.0.3.dist-info/METADATA
+Filename: edurpa_cloud-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_cloud-0.0.3.dist-info/WHEEL
+Filename: edurpa_cloud-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_cloud-0.0.3.dist-info/top_level.txt
+Filename: edurpa_cloud-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_cloud-0.0.3.dist-info/RECORD
+Filename: edurpa_cloud-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Google/Form.py

```diff
@@ -3,16 +3,15 @@
 import json
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from robot.api.deco import keyword, not_keyword
 from googleapiclient.http import MediaIoBaseDownload
-from PyPDF2 import PdfReader
-import gdown
+import random
 
 class Form:
     def __init__(self):
         self.creds=None
     
     @keyword("Set Up Form Connection")
     def authenticate(self, token_file_path: str=None):
@@ -66,19 +65,15 @@
                             "updateMask": "quizSettings.isQuiz",
                         }
                     }
                 ]
             }
 
             # Converts the form into a quiz
-            question_setting = (
-                service.forms()
-                .batchUpdate(formId=result["formId"], body=update)
-                .execute()
-            )
+            service.forms().batchUpdate(formId=result["formId"], body=update).execute()
 
             # Print the result to see it's now a quiz
             getresult = service.forms().get(formId=result["formId"]).execute()
             return getresult["formId"]
         
         except HttpError as error:
             return {'error': str(error), 'error_details': error.error_details}
@@ -117,44 +112,49 @@
         pattern = r'Câu (\d+)\.\s*(.*?)\s*A\.\s*(.*?)\s*B\.\s*(.*?)\s*C\.\s*(.*?)\s*D\.\s*(.*?)(?=\s*Câu|\Z)'
         matches = re.findall(pattern, content, re.DOTALL)
         if not matches:
             return None  # Return None or an empty list if no matches are found
         
         questions = []
         for match in matches:
+            if len(match) < 6:
+                continue
             title = 'Câu ' + match[0] + '. ' + ' '.join(match[1].split())
             question = {
                 'title': title,
                 'options': [' '.join(option.split()) for option in match[2:]]
             }
-            questions.insert(0, question)
+            questions.append(question)
         return questions
     
     @not_keyword
     def parse_answer_keys(self, answers_content):
         pattern = r'(\d+)\.([A-D])'
-        answer_matches = re.findall(pattern, answers_content, re.DOTALL)
-        return {num: ans for num, ans in answer_matches}
+        answer_matches = re.findall(pattern, answers_content)
+        answer_keys = {num: ans for num, ans in answer_matches}
+        return answer_keys
         
     @keyword("Read Google Doc Content And Answers")
     def read_google_doc_content_and_answers(self, doc_id):
         content = self.read_google_doc_content(doc_id)
     
         if 'error' in content:
             return content  # Return error if reading failed
 
         # Use regex to split the content based on variations of the delimiter
-        parts = re.split(r'-{1,}Hết-{1,}', content, flags=re.IGNORECASE)
+        parts = re.split(r'-{1,}HẾT-{1,}', content, flags=re.IGNORECASE)
         doc_content = parts[0].strip() if len(parts) > 0 else ""
         answers_content = parts[1].strip() if len(parts) > 1 else ""
         
+        
         questions = self.parse_questions(doc_content)
         # Parse the answer keys
         answer_keys = self.parse_answer_keys(answers_content)
-        
+    
+                
         return questions, answer_keys
 
     @not_keyword
     def convertCorrectOptionToIndex(self, option):
         if option == 'A':
             return 0
         elif option == 'B':
@@ -173,34 +173,45 @@
 
         if not questions:  # Check if there are no questions to add
             return {'error': 'No questions parsed from the document'}
 
         try:
             service = build('forms', 'v1', credentials=self.creds)
             requests = []
-            for question in questions:
-                correct_option_index = self.convertCorrectOptionToIndex(question['correct_answer'])
-                
+            for question in reversed(questions):
+                if 'correct_answer' not in question or question['correct_answer'] is None:
+                    # Randomly assign a correct answer if none is specified
+                    correct_option_index = random.randint(0, len(question['options']) - 1)
+                else:
+                    correct_option_index = self.convertCorrectOptionToIndex(question['correct_answer'])
+
+                unique_options = list(set(question['options']))  # Remove duplicate options
+                if len(unique_options) != len(question['options']):
+                    continue  # Skip adding this question if duplicates were removed
+
                 choiceQuestion = {
                     'type': 'RADIO',
-                    'options': [{'value': choice} for choice in question['options']],
+                    'options': [{'value': choice} for choice in unique_options],
                 }
 
+                if correct_option_index < 0 or correct_option_index >= len(unique_options):
+                    continue
+
                 new_question = {
                     'createItem': {
                         'item': {
                             'title': question['title'],
                             'questionItem': {
                                 'question': {
                                     'required': True,
                                     'choiceQuestion': choiceQuestion,
                                     "grading": {
                                         "pointValue": 1,
                                         "correctAnswers": {
-                                            "answers":  choiceQuestion['options'][correct_option_index]
+                                            "answers": [choiceQuestion['options'][correct_option_index]]
                                         },
                                         "whenRight": {"text": "You got it!"},
                                         "whenWrong": {"text": "Sorry, that's wrong"}
                                     },
                                 }
                             }
                         },
@@ -212,93 +223,31 @@
                 requests.append(new_question)
 
             if requests:  # Proceed only if there are requests to add
                 body = {'requests': requests}
                 service.forms().batchUpdate(formId=form_id, body=body).execute()
                 return f"https://docs.google.com/forms/d/{form_id}/edit"
             else:
-                return {'error': 'No valid questions were generated to add to the form'}
+                return {'error': 'Error payload', 'questions': questions}
         except HttpError as error:
             return {'error': str(error), 'error_details': error.error_details}
 
+
     @keyword("Add Questions And Answers From Google Doc To Form")
     def add_questions_and_answers_from_google_doc_to_form(self, doc_id, form_id):
         # Read content and answers from Google Doc
         questions, answer_keys = self.read_google_doc_content_and_answers(doc_id)
-
-        # Check if there are no questions or answers to add
-        if not questions or not answer_keys:
-            return {'error': 'No questions or answers parsed from the document'}
-
-        # Map the correct answers to the questions
-        for question in questions:
-            question_num = str(question['title'].split()[1].replace(".", ""))
-            if question_num in answer_keys:
-                question['correct_answer'] = answer_keys[question_num]
-                
-        return self.add_questions_to_form(form_id, questions)
-
-    @not_keyword
-    def read_pdf_content(self, pdf_url):
-        """Reads content from a PDF file."""
-        try:
-            # Download the PDF file from the provided URL
-            pdf_file = "temp_pdf_file.pdf"
-            gdown.download(pdf_url, pdf_file, quiet=False)
-            
-            # Read the content from the downloaded PDF file
-            with open(pdf_file, 'rb') as file:
-                reader = PdfReader(file)
-                text = ''
-                for page in reader.pages:
-                    text += page.extract_text()
-            
-            # Return the extracted text
-            return text
-        except EOFError:
-            return {'error': 'EOF marker not found. The PDF file may be corrupted or incomplete.'}
-        except Exception as e:
-            return {'error': f'An error occurred while reading the PDF file: {str(e)}'}
         
-    @not_keyword
-    def parse_pdf_content_and_answers(self, content):
-        pattern = r'Câu (\d+)\.\s*(.*?)\s*A\.\s*(.*?)\s*B\.\s*(.*?)\s*C\.\s*(.*?)\s*D\.\s*(.*?)(?=\s*Câu|\Z)'
-        matches = re.findall(pattern, content, re.DOTALL)
-        if not matches:
-            return None, None
         
-        questions = []
-        answer_keys = {}
-        for match in matches:
-            title = 'Câu ' + match[0] + '. ' + ' '.join(match[1].split())
-            question = {
-                'title': title,
-                'options': [' '.join(option.split()) for option in match[2:]]
-            }
-            questions.append(question)
-            answer_keys[match[0]] = match[6].strip()
-        
-        return questions, answer_keys
-
-    @keyword("Add Questions And Answers From PDF To Form")
-    def add_questions_and_answers_from_pdf_to_form(self, pdf_file, form_id):
-        # Read content and answers from PDF
-        content = self.read_pdf_content(pdf_file)
-
-        # Check if there is content to parse
-        if 'error' in content:
-            return content
-
-        # Parse content and add questions to form
-        questions, answer_keys = self.parse_pdf_content_and_answers(content)
-
         # Check if there are no questions or answers to add
-        if not questions or not answer_keys:
-            return {'error': 'No questions or answers parsed from the document'}
+        if not questions:
+            return {'error': 'No questions or answers parsed from the document', 'questions': questions, 'answers': answer_keys}
 
         # Map the correct answers to the questions
         for question in questions:
             question_num = str(question['title'].split()[1].replace(".", ""))
             if question_num in answer_keys:
                 question['correct_answer'] = answer_keys[question_num]
-
+            else:
+                question['correct_answer'] = None
+                
         return self.add_questions_to_form(form_id, questions)
```

## Comparing `edurpa_cloud-0.0.3.dist-info/LICENSE` & `edurpa_cloud-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_cloud-0.0.3.dist-info/METADATA` & `edurpa_cloud-0.0.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-cloud
-Version: 0.0.3
+Version: 0.0.4
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edurpa-google
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `edurpa_cloud-0.0.3.dist-info/RECORD` & `edurpa_cloud-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 EduRPA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 EduRPA/Google/Classroom.py,sha256=ZUMo0Dlc46bFwAUnUHKrbOl_RzvOvVHWAQtfa3hJPqQ,13103
 EduRPA/Google/CustomOAuth.py,sha256=zyN2Iq8wwoXtwI9bBAtgecA7R9aZr3rfzswlsf8Bf4o,1511
-EduRPA/Google/Form.py,sha256=K4SdXFT6VKbreHnNebTjGtEDuJoPC7JnKD4t1xSB55Y,11964
+EduRPA/Google/Form.py,sha256=Qg1R8fxJNsh7cw1RAEtrciD9QJ69y0elioZzarjfamk,10019
 EduRPA/Google/Utils.py,sha256=oELOV-TFTQz_NDf9i0usZfXC9kbY4Xa_Kb1T7D8ssOw,314
 EduRPA/Google/__init__.py,sha256=q9wb2yVj8rKIsGf7UelAixwVKWk9CCKsQCzmUtCVzDM,469
 EduRPA/Storage/S3Storage.py,sha256=5c0cvfvJmM-qp3huholxdM8Bzc9iH1b7lEYwnoZdhdE,1603
 EduRPA/Storage/Storage.py,sha256=TIhaD373yDdHms9OANPhSUx0b5xLOp2IUru8t1Voeok,1575
 EduRPA/Storage/__init__.py,sha256=6QsHQApuwUyuN1yU9O87eeU0ai7frQScebeBuZoQLpk,312
-edurpa_cloud-0.0.3.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_cloud-0.0.3.dist-info/METADATA,sha256=EdpgPdaoNJ5BOwvj31KX4MsdJqvVT761GN20t-NesSo,716
-edurpa_cloud-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_cloud-0.0.3.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_cloud-0.0.3.dist-info/RECORD,,
+edurpa_cloud-0.0.4.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_cloud-0.0.4.dist-info/METADATA,sha256=8n8ZVrWvwFmqza_v_j3bYJofOFyr0xqNom7FEZl8uXs,716
+edurpa_cloud-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_cloud-0.0.4.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_cloud-0.0.4.dist-info/RECORD,,
```

