# Comparing `tmp/playwrightcapture-1.24.8.tar.gz` & `tmp/playwrightcapture-1.24.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.8.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.9.tar", max compression
```

## Comparing `playwrightcapture-1.24.8.tar` & `playwrightcapture-1.24.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/LICENSE
--rw-r--r--   0        0        0     1441 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/README.md
--rw-r--r--   0        0        0      511 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    65183 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1543 2024-05-03 09:38:34.205199 playwrightcapture-1.24.8/pyproject.toml
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 playwrightcapture-1.24.8/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/LICENSE
+-rw-r--r--   0        0        0     1441 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/README.md
+-rw-r--r--   0        0        0      511 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    65604 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:22:33.738474 playwrightcapture-1.24.9/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1521 2024-05-17 12:22:33.742473 playwrightcapture-1.24.9/pyproject.toml
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 playwrightcapture-1.24.9/PKG-INFO
```

### Comparing `playwrightcapture-1.24.8/LICENSE` & `playwrightcapture-1.24.9/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.8/README.md` & `playwrightcapture-1.24.9/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.8/playwrightcapture/capture.py` & `playwrightcapture-1.24.9/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from io import BytesIO
 from logging import LoggerAdapter, Logger
 from tempfile import NamedTemporaryFile
 from typing import Any, TypedDict, Literal, TYPE_CHECKING, MutableMapping
 from urllib.parse import urlparse, unquote, urljoin
 from zipfile import ZipFile
 
+import aiohttp
 import dateparser
-import requests
 import urllib3
 
-
+from aiohttp_socks import ProxyConnector  # type: ignore[import-untyped]
 from bs4 import BeautifulSoup
 from charset_normalizer import from_bytes
 from playwright._impl._errors import TargetClosedError
 from playwright.async_api import async_playwright, Frame, Error, Page, Download, Request
 from playwright.async_api import TimeoutError as PlaywrightTimeoutError
 from playwright_stealth import stealth_async  # type: ignore[import-untyped]
 from puremagic import PureError, from_string  # type: ignore[import-untyped]
@@ -634,15 +634,15 @@
                                         self._requests[request.url] = body
                                 except PureError:
                                     # unable to identify the mimetype
                                     pass
                         except Exception:
                             pass
             except Exception as e:
-                self.logger.warning(f'Unable to store request: {e}')
+                self.logger.info(f'Unable to store request: {e}')
 
         if page is not None:
             capturing_sub = True
         else:
             capturing_sub = False
             page = await self.context.new_page()
             if allow_tracking:
@@ -654,15 +654,15 @@
                 await self.__dialog_complianz_clickthrough(page)
                 await self.__dialog_yahoo_clickthrough(page)
                 await self.__dialog_ppms_clickthrough(page)
                 await self.__dialog_alert_dialog_clickthrough(page)
                 await self.__dialog_clickthrough(page)
 
             await stealth_async(page)
-            page.set_default_timeout(self._capture_timeout * 1000)
+            page.set_default_timeout((self._capture_timeout - 2) * 1000)
             # trigger a callback on each request to store it in a dict indexed by URL to get it back from the favicon fetcher
             page.on("requestfinished", store_request)
 
         try:
             # Parse the URL. If there is a fragment, we need to scroll to it manually
             parsed_url = urlparse(url, allow_fragments=True)
 
@@ -805,15 +805,15 @@
                 await self._safe_wait(page)
                 self.logger.debug('Done with instrumentation, done with waiting.')
 
                 if content := await self._failsafe_get_content(page):
                     to_return['html'] = content
 
                 if 'html' in to_return and to_return['html'] is not None and with_favicon:
-                    to_return['potential_favicons'] = self.get_favicons(page.url, to_return['html'])
+                    to_return['potential_favicons'] = await self.get_favicons(page.url, to_return['html'])
                     got_favicons = True
 
                 to_return['last_redirected_url'] = page.url
                 to_return['png'] = await self._failsafe_get_screenshot(page)
 
                 self._already_captured.add(url)
                 if depth > 0 and to_return.get('html') and to_return['html']:
@@ -945,14 +945,15 @@
                     to_return['cookies'] = await self.context.cookies()
                     self.logger.debug('Done with cookies.')
                 except Exception as e:
                     if 'error' not in to_return:
                         to_return['error'] = f'Unable to get the cookies: {e}'
                 # frames_tree = self.make_frame_tree(page.main_frame)
                 try:
+                    page.remove_listener("requestfinished", store_request)
                     await page.close()
                     await self.context.close()  # context needs to be closed to generate the HAR
                     self.logger.debug('Context closed.')
                     with open(self._temp_harfile.name) as _har:
                         to_return['har'] = json.load(_har)
                     self.logger.debug('Got HAR.')
                 except Exception as e:
@@ -1092,44 +1093,52 @@
 
         main_frame = page.frame(name=recaptcha_testframename)
         if not main_frame:
             return False
 
         # click on audio challenge button
         await main_frame.get_by_role("button", name="Get an audio challenge").click()
-        while True:
-            try:
-                href = await main_frame.get_by_role("link", name="Alternatively, download audio as MP3").get_attribute("href")
-            except Exception as e:
-                self.logger.warning(f'Google caught the browser as a robot, sorry: {e}')
-                return False
-            if not href:
-                self.logger.warning('Unable to find download link for captcha.')
-                return False
-            r = requests.get(href, allow_redirects=True)
-            with NamedTemporaryFile() as mp3_file, NamedTemporaryFile() as wav_file:
-                mp3_file.write(r.content)
-                pydub.AudioSegment.from_mp3(mp3_file.name).export(wav_file.name, format="wav")
-                recognizer = Recognizer()
-                recaptcha_audio = AudioFile(wav_file.name)
-                with recaptcha_audio as source:
-                    audio = recognizer.record(source)
-                text = recognizer.recognize_google(audio)
-            await main_frame.get_by_role("textbox", name="Enter what you hear").fill(text)
-            await main_frame.get_by_role("button", name="Verify").click()
-            await self._safe_wait(page, 5)
-            await self._wait_for_random_timeout(page, random.randint(3, 6))
-            try:
-                if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").first.is_checked(timeout=5000):
-                    self.logger.info('Captcha solved successfully')
-                    return True
-                elif await main_frame.get_by_role("textbox", name="Enter what you hear").is_editable(timeout=5000):
-                    self.logger.info('Unable to find checkbox, needs to solve more captchas')
-            except PlaywrightTimeoutError as e:
-                self.logger.info(f'Unexpected timeout: {e}')
+
+        connector = None
+        if self.proxy and self.proxy.get('server'):
+            connector = ProxyConnector.from_url(self.proxy['server'])
+
+        async with aiohttp.ClientSession(connector=connector) as session:
+            while True:
+                try:
+                    href = await main_frame.get_by_role("link", name="Alternatively, download audio as MP3").get_attribute("href")
+                except Exception as e:
+                    self.logger.warning(f'Google caught the browser as a robot, sorry: {e}')
+                    return False
+                if not href:
+                    self.logger.warning('Unable to find download link for captcha.')
+                    return False
+                async with session.get(href, timeout=10, ssl=False) as response:
+                    response.raise_for_status()
+                    mp3_content = await response.read()
+                with NamedTemporaryFile() as mp3_file, NamedTemporaryFile() as wav_file:
+                    mp3_file.write(mp3_content)
+                    pydub.AudioSegment.from_mp3(mp3_file.name).export(wav_file.name, format="wav")
+                    recognizer = Recognizer()
+                    recaptcha_audio = AudioFile(wav_file.name)
+                    with recaptcha_audio as source:
+                        audio = recognizer.record(source)
+                    text = recognizer.recognize_google(audio)
+                await main_frame.get_by_role("textbox", name="Enter what you hear").fill(text)
+                await main_frame.get_by_role("button", name="Verify").click()
+                await self._safe_wait(page, 5)
+                await self._wait_for_random_timeout(page, random.randint(3, 6))
+                try:
+                    if await recaptcha_init_frame.locator("//span[@id='recaptcha-anchor']").first.is_checked(timeout=5000):
+                        self.logger.info('Captcha solved successfully')
+                        return True
+                    elif await main_frame.get_by_role("textbox", name="Enter what you hear").is_editable(timeout=5000):
+                        self.logger.info('Unable to find checkbox, needs to solve more captchas')
+                except PlaywrightTimeoutError as e:
+                    self.logger.info(f'Unexpected timeout: {e}')
 
     def _update_exceptions(self, exception: Error) -> None:
         if '\n' in exception.message:
             name, _ = exception.message.split('\n', maxsplit=1)
             if ' at ' in name:
                 name, _ = name.split(' at ', maxsplit=1)
             elif '; ' in name:
@@ -1271,67 +1280,60 @@
                     else:
                         # NOTE: This urn can be a path without the domain part. We need to urljoin
                         favicons_urls.add(icon_url)
             else:
                 self.logger.info(f'Not processing {tag}')
         return favicons_urls, favicons
 
-    def get_favicons(self, rendered_url: str, rendered_content: str) -> set[bytes]:
+    async def get_favicons(self, rendered_url: str, rendered_content: str) -> set[bytes]:
         """This method will be deprecated as soon as Playwright will be able to fetch favicons (https://github.com/microsoft/playwright/issues/7493).
         In the meantime, we try to get all the potential ones in this method.
         Method inspired by https://github.com/ail-project/ail-framework/blob/master/bin/lib/crawlers.py
         """
+        connector = None
+        if self.proxy and self.proxy.get('server'):
+            # NOTE 2024-05-17: switch to async to fetch, the lib uses socks5h by default
+            connector = ProxyConnector.from_url(self.proxy['server'])
+
         extracted_favicons = self.__extract_favicons(rendered_content)
         if not extracted_favicons:
             return set()
         to_fetch, to_return = extracted_favicons
         to_fetch.add('/favicon.ico')
-        session = requests.session()
-        session.verify = False
-        session.headers['user-agent'] = self.user_agent
-        if self.proxy and self.proxy.get('server'):
-            proxy_server = self.proxy['server']
-            # Make sure the DNS desolution is done remotely
-            # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
-            if proxy_server.startswith('socks5://'):
-                proxy_server = proxy_server.replace('socks5://', 'socks5h://')
-            if proxy_server.startswith('socks4://'):
-                proxy_server = proxy_server.replace('socks4://', 'socks4a://')
-
-            proxies = {'http': proxy_server, 'https': proxy_server}
-            session.proxies.update(proxies)
-        for u in to_fetch:
-            try:
-                self.logger.debug(f'Attempting to fetch favicon from {u}.')
-                url_to_fetch = urljoin(rendered_url, u)
-                favicon = b''
-                if url_to_fetch in self._requests:
-                    favicon = self._requests[url_to_fetch]
-                if not favicon:
-                    favicon_response = session.get(url_to_fetch, timeout=5)
-                    favicon_response.raise_for_status()
-                    favicon = favicon_response.content
-                if favicon:
-                    try:
-                        mimetype = from_string(favicon, mime=True)
-                    except PureError:
-                        # unable to identify the mimetype
-                        self.logger.debug(f'Unable to identify the mimetype for favicon from {u}')
-                    else:
-                        if not mimetype:
-                            # empty, ignore
-                            pass
-                        elif mimetype.startswith('image'):
-                            to_return.add(favicon)
-                        elif mimetype.startswith('text'):
-                            # Just ignore, it's probably a 404 page
-                            pass
+        async with aiohttp.ClientSession(connector=connector) as session:
+            session.headers['user-agent'] = self.user_agent
+            for u in to_fetch:
+                try:
+                    self.logger.debug(f'Attempting to fetch favicon from {u}.')
+                    url_to_fetch = urljoin(rendered_url, u)
+                    favicon = b''
+                    if url_to_fetch in self._requests:
+                        favicon = self._requests[url_to_fetch]
+                    if not favicon:
+                        async with session.get(url_to_fetch, timeout=5, ssl=False) as favicon_response:
+                            favicon_response.raise_for_status()
+                            favicon = await favicon_response.read()
+                    if favicon:
+                        try:
+                            mimetype = from_string(favicon, mime=True)
+                        except PureError:
+                            # unable to identify the mimetype
+                            self.logger.debug(f'Unable to identify the mimetype for favicon from {u}')
                         else:
-                            self.logger.warning(f'Unexpected mimetype for favicon from {u}: {mimetype}')
-                self.logger.debug(f'Done with favicon from {u}.')
-            except requests.HTTPError as e:
-                self.logger.debug(f'Unable to fetch favicon from {u}: {e}')
-            except Exception as e:
-                self.logger.info(f'Unexpectedly unable to fetch favicon from {u}: {e}')
+                            if not mimetype:
+                                # empty, ignore
+                                pass
+                            elif mimetype.startswith('image'):
+                                to_return.add(favicon)
+                            elif mimetype.startswith('text'):
+                                # Just ignore, it's probably a 404 page
+                                pass
+                            else:
+                                self.logger.warning(f'Unexpected mimetype for favicon from {u}: {mimetype}')
+                    self.logger.debug(f'Done with favicon from {u}.')
+                except aiohttp.ClientError as e:
+                    self.logger.debug(f'Unable to fetch favicon from {u}: {e}')
+                except Exception as e:
+                    self.logger.info(f'Unexpectedly unable to fetch favicon from {u}: {e}')
         return to_return
 
     # END FAVICON EXTRACTOR
```

### Comparing `playwrightcapture-1.24.8/playwrightcapture/helpers.py` & `playwrightcapture-1.24.9/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.8/pyproject.toml` & `playwrightcapture-1.24.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.8"
+version = "1.24.9"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -19,35 +19,35 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "^1.43.0"
 dateparser = "^1.2.0"
 beautifulsoup4 = {version= "^4.12.3", extras = ["lxml", "charset_normalizer"]}
 w3lib = "^2.1.2"
-requests = {extras = ["socks"], version = "^2.31.0"}
 pydub = {version = "^0.25.1", optional = true}
-SpeechRecognition = {version = "^3.10.3", optional = true}
+SpeechRecognition = {version = "^3.10.4", optional = true}
 pytz = {"version" = "^2024.1", python = "<3.9"}
 tzdata = "^2024.1"
 playwright-stealth = "^1.0.6"
 setuptools = "^69.5.1"
-puremagic = "^1.22"
+puremagic = "^1.23"
 async-timeout = {version = "^4.0.3", python = "<3.11"}
+aiohttp = {extras = ["speedups"], version = "^3.9.5"}
+aiohttp-socks = "^0.8.4"
 
 [tool.poetry.extras]
-recaptcha = ["requests", "pydub", "SpeechRecognition"]
+recaptcha = ["pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-types-beautifulsoup4 = "^4.12.0.20240229"
+types-beautifulsoup4 = "^4.12.0.20240511"
 pytest = "^8.2.0"
 mypy = "^1.10.0"
 types-dateparser = "^1.2.0.20240420"
-types-requests = "^2.31.0.20240406"
 types-pytz = "^2024.1.0.20240417"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playwrightcapture-1.24.8/PKG-INFO` & `playwrightcapture-1.24.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.8
+Version: 1.24.9
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -16,24 +16,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
-Requires-Dist: SpeechRecognition (>=3.10.3,<4.0.0) ; extra == "recaptcha"
+Requires-Dist: SpeechRecognition (>=3.10.4,<4.0.0) ; extra == "recaptcha"
+Requires-Dist: aiohttp-socks (>=0.8.4,<0.9.0)
+Requires-Dist: aiohttp[speedups] (>=3.9.5,<4.0.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: beautifulsoup4[charset-normalizer,lxml] (>=4.12.3,<5.0.0)
 Requires-Dist: dateparser (>=1.2.0,<2.0.0)
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: playwright-stealth (>=1.0.6,<2.0.0)
-Requires-Dist: puremagic (>=1.22,<2.0)
+Requires-Dist: puremagic (>=1.23,<2.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2024.1,<2025.0) ; python_version < "3.9"
-Requires-Dist: requests[socks] (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: tzdata (>=2024.1,<2025.0)
 Requires-Dist: w3lib (>=2.1.2,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
 
 # Playwright Capture
```

