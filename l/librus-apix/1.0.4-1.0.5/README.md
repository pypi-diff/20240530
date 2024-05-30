# Comparing `tmp/librus_apix-1.0.4.tar.gz` & `tmp/librus_apix-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.4.tar", last modified: Tue May 28 21:25:40 2024, max compression
+gzip compressed data, was "librus_apix-1.0.5.tar", last modified: Thu May 30 07:47:16 2024, max compression
```

## Comparing `librus_apix-1.0.4.tar` & `librus_apix-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.104798 librus_apix-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 21:25:37.000000 librus_apix-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 21:25:40.104798 librus_apix-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-28 21:25:37.000000 librus_apix-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.100798 librus_apix-1.0.4/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.104798 librus_apix-1.0.4/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 21:25:37.000000 librus_apix-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-28 21:25:40.104798 librus_apix-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:25:37.000000 librus_apix-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:47:12.000000 librus_apix-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 07:47:16.023748 librus_apix-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-30 07:47:12.000000 librus_apix-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-30 07:47:16.000000 librus_apix-1.0.5/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 07:47:12.000000 librus_apix-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-30 07:47:16.023748 librus_apix-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:47:12.000000 librus_apix-1.0.5/setup.py
```

### Comparing `librus_apix-1.0.4/LICENSE` & `librus_apix-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/README.md` & `librus_apix-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/__init__.py` & `librus_apix-1.0.5/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/announcements.py` & `librus_apix-1.0.5/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/attendance.py` & `librus_apix-1.0.5/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/client.py` & `librus_apix-1.0.5/librus_apix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,23 @@
 #Alternatively, you can use the classes directly:
 my_token = Token(API_Key="your_api_key")
 my_client = Client(token=my_token)
 ```
 """
 
 
-from typing import Optional, Dict
-from requests.models import Response
+from typing import Dict, Optional
+
 from requests import Session
+from requests.models import Response
 from requests.sessions import RequestsCookieJar
 from requests.utils import cookiejar_from_dict, dict_from_cookiejar
+
 import librus_apix.urls as urls
-from librus_apix.exceptions import (
-    AuthorizationError,
-    MaintananceError,
-    TokenKeyError,
-)
+from librus_apix.exceptions import AuthorizationError, MaintananceError, TokenKeyError
 
 
 class Token:
     """
      A class to manage and store API tokens.
 
     The API key should be formatted as "{DZIENNIKSID}:{SDZIENNIKSID}".
@@ -165,14 +163,15 @@
         timetable_url: str = urls.TIMETABLE_URL,
         announcements_url: str = urls.ANNOUNCEMENTS_URL,
         message_url: str = urls.MESSAGE_URL,
         send_message_url: str = urls.SEND_MESSAGE_URL,
         attendance_url: str = urls.ATTENDANCE_URL,
         attendance_details_url: str = urls.ATTENDANCE_DETAILS_URL,
         schedule_url: str = urls.SCHEDULE_URL,
+        recent_schedule_url: str = urls.RECENT_SCHEDULE_URL,
         homework_url: str = urls.HOMEWORK_URL,
         homework_details_url: str = urls.HOMEWORK_DETAILS_URL,
         info_url: str = urls.INFO_URL,
         recipients_url: str = urls.RECIPIENTS_URL,
         recipient_groups_url: str = urls.RECIPIENT_GROUPS_URL,
         completed_lessons_url: str = urls.COMPLETED_LESSONS_URL,
         gateway_api_attendance: str = urls.GATEWAY_API_ATTENDANCE,
@@ -189,14 +188,15 @@
         self.TIMETABLE_URL = timetable_url
         self.ANNOUNCEMENTS_URL = announcements_url
         self.MESSAGE_URL = message_url
         self.SEND_MESSAGE_URL = send_message_url
         self.ATTENDANCE_URL = attendance_url
         self.ATTENDANCE_DETAILS_URL = attendance_details_url
         self.SCHEDULE_URL = schedule_url
+        self.RECENT_SCHEDULE_URL = recent_schedule_url
         self.HOMEWORK_URL = homework_url
         self.HOMEWORK_DETAILS_URL = homework_details_url
         self.INFO_URL = info_url
         self.COMPLETED_LESSONS_URL = completed_lessons_url
         self.GATEWAY_API_ATTENDANCE = gateway_api_attendance
         self.RECIPIENTS_URL = recipients_url
         self.RECIPIENT_GROUPS_URL = recipient_groups_url
@@ -350,14 +350,15 @@
     timetable_url: str = urls.TIMETABLE_URL,
     announcements_url: str = urls.ANNOUNCEMENTS_URL,
     message_url: str = urls.MESSAGE_URL,
     send_message_url: str = urls.SEND_MESSAGE_URL,
     attendance_url: str = urls.ATTENDANCE_URL,
     attendance_details_url: str = urls.ATTENDANCE_DETAILS_URL,
     schedule_url: str = urls.SCHEDULE_URL,
+    recent_schedule_url: str = urls.RECENT_SCHEDULE_URL,
     homework_url: str = urls.HOMEWORK_URL,
     homework_details_url: str = urls.HOMEWORK_DETAILS_URL,
     info_url: str = urls.INFO_URL,
     recipients_url: str = urls.RECIPIENTS_URL,
     recipient_groups_url: str = urls.RECIPIENT_GROUPS_URL,
     completed_lessons_url: str = urls.COMPLETED_LESSONS_URL,
     gateway_api_attendance: str = urls.GATEWAY_API_ATTENDANCE,
@@ -404,14 +405,15 @@
         timetable_url,
         announcements_url,
         message_url,
         send_message_url,
         attendance_url,
         attendance_details_url,
         schedule_url,
+        recent_schedule_url,
         homework_url,
         homework_details_url,
         info_url,
         recipients_url,
         recipient_groups_url,
         completed_lessons_url,
         gateway_api_attendance,
```

### Comparing `librus_apix-1.0.4/librus_apix/completed_lessons.py` & `librus_apix-1.0.5/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/exceptions.py` & `librus_apix-1.0.5/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/grades.py` & `librus_apix-1.0.5/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/helpers.py` & `librus_apix-1.0.5/librus_apix/helpers.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/homework.py` & `librus_apix-1.0.5/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/messages.py` & `librus_apix-1.0.5/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/notifications.py` & `librus_apix-1.0.5/librus_apix/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from librus_apix.attendance import Attendance, get_attendance
 from librus_apix.client import Client
 from librus_apix.exceptions import ParseError
 from librus_apix.grades import Grade, get_grades
 from librus_apix.helpers import no_access_check
 from librus_apix.homework import Homework, get_homework
 from librus_apix.messages import Message, get_received
-from librus_apix.schedule import Event
+from librus_apix.schedule import RecentEvent, get_recently_added_schedule
 
 
 @dataclass
 class NotificationAmount:
     """
     Represents a notification with a destination identifier name and an amount.
 
@@ -60,15 +60,27 @@
     soup = no_access_check(BeautifulSoup(client.get(client.INDEX_URL).text, "lxml"))
     notifications = []
     circles = soup.select("div#graphic-menu > ul > li > a[class!='button counter']")
     for circle in circles:
         name = circle.text.replace("\n", "").strip()
         destination = circle.attrs.get("href", "/")
         amount = 0
-        if name == "Widok alternatywny" or "javascript" in destination:
+        if (
+            name == "Widok alternatywny"
+            or "javascript" in destination
+            or destination
+            not in [
+                "/ogloszenia",
+                "/moje_zadania",
+                "/wiadomosci",
+                "/przegladaj_oceny/uczen",
+                "/przegladaj_nb/uczen",
+                "/terminarz",
+            ]
+        ):
             continue
 
         if isinstance(circle.parent, Tag):
             counter = circle.parent.select_one("a.button.counter")
             if isinstance(counter, Tag):
                 try:
                     amount = int(counter.text)
@@ -115,15 +127,15 @@
         href = message.href
         if _compare_hrefs(href, seen_ids):
             break
         if message.unread == False:
             continue
         new_ids.append(href)
         new_messages.append(message)
-    if len(messages) > 0 and len(new_ids) == 0:
+    if len(messages) > 0 and len(seen_ids) == 0:
         seen_ids.append(messages[0].href)
     else:
         seen_ids.extend(new_ids)
     return new_messages, seen_ids
 
 
 def _parse_attendance_notification(
@@ -171,33 +183,31 @@
         case "/przegladaj_nb/uczen":
             attendance = get_attendance(client, "last_login")
             return _parse_attendance_notification(attendance)
         case "/wiadomosci":
             messages = get_received(client, 0)
             top_two_msgs = messages[:2]
             if len(top_two_msgs) == 0:
-                newest = [messages[0]]
-                _, ids = _parse_messages_notification(newest)
-                return [], ids
+                return [], []
             else:
                 return _parse_messages_notification(top_two_msgs)
-            return _parse_messages_notification(top_two_msgs)
+
         case "/ogloszenia":
             announcements = get_announcements(client)
             newest = announcements[: amount.amount]
             if len(newest) == 0:
                 newest = [announcements[0]]
                 _, ids = _parse_announcements_notification(newest)
                 return [], ids
             else:
                 return _parse_announcements_notification(newest)
 
         case "/terminarz":
-            # TODO implement the last_login one when I get the chance to see it's html
-            return [], []
+            schedule = get_recently_added_schedule(client)
+            return schedule, []
         case "/moje_zadania":
             today = datetime.now()
             hw_amount = -amount.amount
             if hw_amount == 0:
                 hw_amount = -1
             homework = get_homework(
                 client,
@@ -220,23 +230,23 @@
     Represents data of various notifications.
 
     Attributes:
         grades (List[Grade]): A list of grade notifications.
         attendance (List[Attendance]): A list of attendance notifications.
         messages (List[Message]): A list of message notifications.
         announcements (List[Announcement]): A list of announcement notifications.
-        schedule (List[Event]): A list of schedule notifications.
+        schedule (List[RecentEvent]): A list of schedule notifications.
         homework (List[Homework]): A list of homework notifications.
     """
 
     grades: List[Grade]
     attendance: List[Attendance]
     messages: List[Message]
     announcements: List[Announcement]
-    schedule: List[Event]
+    schedule: List[RecentEvent]
     homework: List[Homework]
 
 
 @dataclass
 class NotificationIds:
     """
     Represents the IDs (mostly .href) of various notifications to track seen notifications.
@@ -273,14 +283,16 @@
     amounts = map(lambda amount: parse_basic_amount(client, amount), amounts)
     notify_data = []
     notify_ids = []
     for data, ids in amounts:
         notify_data.append(data)
         notify_ids.append(ids)
 
+    if len(notify_data) != 6:
+        raise ParseError("notification length doenst match expected 6")
     return NotificationData(*notify_data), NotificationIds(*notify_ids)
 
 
 def get_new_notification_data(client: Client, seen_notifications: NotificationIds):
     """
     Fetches and parses new notification data and updates seen notification IDs based on given NotificationIds.
 
@@ -298,14 +310,15 @@
     today = datetime.now()
     homework = get_homework(
         client,
         (today - timedelta(days=7)).strftime("%Y-%m-%d"),
         today.strftime("%Y-%m-%d"),
     )[::-1]
 
+    new_schedule = get_recently_added_schedule(client)
     new_grades, seen_grades = _parse_grades_notifications(
         grades, seen_notifications.grades
     )
     new_attendance, seen_attendance = _parse_attendance_notification(
         attendance, seen_notifications.attendance
     )
     new_messages, seen_messages = _parse_messages_notification(
@@ -313,28 +326,23 @@
     )
     new_announcements, seen_announcements = _parse_announcements_notification(
         announcements, seen_notifications.announcements
     )
     new_homework, seen_homework = _parse_homework_notification(
         homework, seen_notifications.homework
     )
-    # TODO TODO OTODODOOTFOFTOFTOOTODRTOTDODODTODOTO
-    new_schedule, seen_schedule = ([], [])
 
     return NotificationData(
         new_grades,
         new_attendance,
         new_messages,
         new_announcements,
         new_schedule,
         new_homework,
     ), NotificationIds(
         seen_grades,
         seen_attendance,
         seen_messages,
         seen_announcements,
-        seen_schedule,
+        [],
         seen_homework,
     )
-
-
-# TODO https://synergia.librus.pl/terminarz/dodane_od_ostatniego_logowania
```

### Comparing `librus_apix-1.0.4/librus_apix/schedule.py` & `librus_apix-1.0.5/librus_apix/schedule.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 
     # Fetch detailed schedule information
     day_one = monthly_schedule[1].href
     prefix, suffix = day_one.split("/")
     detailed_schedule = schedule_detail(client, prefix, detail_url)
     ```
 """
+import re
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import DefaultDict, Dict, List, Union
+
 from bs4 import BeautifulSoup, NavigableString, Tag
+
 from librus_apix.client import Client
 from librus_apix.exceptions import ParseError
 from librus_apix.helpers import no_access_check
-from collections import defaultdict
-from dataclasses import dataclass
-import re
-from typing import DefaultDict, Union, List, Dict
 
 
 @dataclass
 class Event:
     """
     Represents an event in the schedule.
 
@@ -188,7 +190,62 @@
                 href = "/".join(href[2:])
             else:
                 href = ""
 
             event = Event(title, subject, additional_data, str(d), number, hour, href)
             schedule[d].append(event)
     return schedule
+
+
+@dataclass
+class RecentEvent:
+    """
+    The events inside recent_schedule differ a little bit
+    the .data should contain event name, date from to and duration
+    I might be able to extract into separate values if I get html
+    """
+
+    date_added: str
+    type: str
+    data: str
+
+
+def _sanitize_data(data: str) -> str:
+    return (
+        data.replace("&nbsp;", " ")
+        .replace("<br/>", "<br>")
+        .replace("<br>", "\n")
+        .strip()
+    )
+
+
+def get_recently_added_schedule(client: Client) -> List[RecentEvent]:
+    """
+    Events can be viewed only once here, any subsequent call won't have same events
+    Made blindly based on a screenshot, still untested...
+    """
+    events = []
+    soup = no_access_check(
+        BeautifulSoup(
+            client.get(client.RECENT_SCHEDULE_URL).text,
+            "lxml",
+        )
+    )
+    bg = soup.select_one("div.container-background")
+    if bg is None:
+        raise ParseError("Unable to locate recent schedule container-background")
+    table = soup.select_one("table")
+    if table is None:
+        return []
+    rows = table.select("tr")
+    for row in rows:
+        tds = row.select("td")
+        if len(tds) != 4:
+            continue
+        _, date_added, _type, data = tds
+        data = _sanitize_data(data.text)
+        # unsure about that so we'll check
+        if "czas dodania" in date_added and "rodzaj zdarzenia" in _type:
+            continue
+        event = RecentEvent(date_added.text.strip(), _type.text.strip(), data)
+        events.append(event)
+    return events
```

### Comparing `librus_apix-1.0.4/librus_apix/student_information.py` & `librus_apix-1.0.5/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/timetable.py` & `librus_apix-1.0.5/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/librus_apix/urls.py` & `librus_apix-1.0.5/librus_apix/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     - INFO_URL: URL for accessing information.
     - COMPLETED_LESSONS_URL: URL for accessing completed lessons.
     - GATEWAY_API_ATTENDANCE: URL for accessing attendance data via the gateway API.
     - REFRESH_OAUTH_URL: URL for refreshing OAuth tokens.
     ```
 """
 
-from typing import Union, Dict
-
+from typing import Dict, Union
 
 HEADERS: Dict[str, Union[str, bytes]] = {
     "User-Agent": "Mozilla/5.0 (Windows NT x.y; Win64; x64; rv:10.0) Gecko/20100101 Firefox/10.0",
     "Content-Type": "application/x-www-form-urlencoded",
 }
 BASE_URL = "https://synergia.librus.pl"
 API_URL = "https://api.librus.pl"
@@ -40,13 +39,14 @@
 MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/5"
 RECIPIENT_GROUPS_URL = f"{BASE_URL}/wiadomosci/2/6"
 RECIPIENTS_URL = f"{BASE_URL}/getRecipients"
 SEND_MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/6"
 ATTENDANCE_URL = f"{BASE_URL}/przegladaj_nb/uczen"
 ATTENDANCE_DETAILS_URL = f"{BASE_URL}/przegladaj_nb/szczegoly/"
 SCHEDULE_URL = f"{BASE_URL}/terminarz/"
+RECENT_SCHEDULE_URL = f"{BASE_URL}/terminarz/dodane_od_ostatniego_logowania"
 HOMEWORK_URL = f"{BASE_URL}/moje_zadania"
 HOMEWORK_DETAILS_URL = f"{BASE_URL}/moje_zadania/podglad/"
 INFO_URL = f"{BASE_URL}/informacja"
 COMPLETED_LESSONS_URL = f"{BASE_URL}/zrealizowane_lekcje"
 GATEWAY_API_ATTENDANCE = f"{BASE_URL}/gateway/api/2.0/Attendances"
 REFRESH_OAUTH_URL = f"{BASE_URL}/refreshToken"
```

### Comparing `librus_apix-1.0.4/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.5/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.4/setup.cfg` & `librus_apix-1.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.4
+version = v1.0.5
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

