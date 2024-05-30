# Comparing `tmp/mystbin_py-7.0.0.tar.gz` & `tmp/mystbin_py-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystbin_py-7.0.0.tar", max compression
+gzip compressed data, was "mystbin_py-7.0.1.tar", max compression
```

## Comparing `mystbin_py-7.0.0.tar` & `mystbin_py-7.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1063 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/LICENSE
--rwxr-xr-x   0        0        0     2886 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/README.md
--rwxr-xr-x   0        0        0     1567 2024-05-10 18:34:33.796132 mystbin_py-7.0.0/mystbin/__init__.py
--rwxr-xr-x   0        0        0     4384 2024-05-10 18:24:40.008954 mystbin_py-7.0.0/mystbin/client.py
--rwxr-xr-x   0        0        0     1750 2024-05-10 18:36:14.572675 mystbin_py-7.0.0/mystbin/errors.py
--rwxr-xr-x   0        0        0     9753 2024-05-10 18:33:49.139891 mystbin_py-7.0.0/mystbin/http.py
--rwxr-xr-x   0        0        0     5239 2024-05-10 18:21:46.436019 mystbin_py-7.0.0/mystbin/paste.py
--rwxr-xr-x   0        0        0        0 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/mystbin/py.typed
--rwxr-xr-x   0        0        0     1149 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/mystbin/types/__init__.py
--rwxr-xr-x   0        0        0     1663 2024-05-10 18:05:26.194657 mystbin_py-7.0.0/mystbin/types/responses.py
--rw-r--r--   0        0        0     1451 2024-05-10 18:13:19.229246 mystbin_py-7.0.0/mystbin/utils.py
--rwxr-xr-x   0        0        0     3154 2024-05-10 18:36:19.088700 mystbin_py-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 mystbin_py-7.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1063 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/LICENSE
+-rwxr-xr-x   0        0        0     2461 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/README.md
+-rwxr-xr-x   0        0        0     1567 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/__init__.py
+-rwxr-xr-x   0        0        0     4416 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/client.py
+-rwxr-xr-x   0        0        0     1750 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/errors.py
+-rwxr-xr-x   0        0        0     9753 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/http.py
+-rwxr-xr-x   0        0        0     5641 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/paste.py
+-rwxr-xr-x   0        0        0        0 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/py.typed
+-rwxr-xr-x   0        0        0     1149 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/types/__init__.py
+-rwxr-xr-x   0        0        0     1663 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/types/responses.py
+-rw-r--r--   0        0        0     1451 2024-05-30 09:40:04.595974 mystbin_py-7.0.1/mystbin/utils.py
+-rwxr-xr-x   0        0        0     3154 2024-05-30 09:40:04.599974 mystbin_py-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 mystbin_py-7.0.1/PKG-INFO
```

### Comparing `mystbin_py-7.0.0/LICENSE` & `mystbin_py-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/README.md` & `mystbin_py-7.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,25 @@
     </a>
     <a href='https://github.com/PythonistaGuild/mystbin.py/actions/workflows/build.yaml'>
         <img src='https://github.com/PythonistaGuild/mystbin.py/workflows/Build/badge.svg' alt='Build status' />
     </a>
 </div>
 <br>
 
-A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs can be found [here](https://api.mystb.in/docs).
+A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs can be found [here](https://mystb.in/api/documentation).
 
 Documentation for this wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/).
 If you want the docs for the `main` branch, those can be found [here](https://mystbinpy.readthedocs.io/en/latest/).
 
 ----------
 ### Features
 
 - [x] - Creating pastes.
-  - [ ] Supporting attachments.
-- [ ] - Editing pastes.
-    - Pending design work.
 - [x] - Deleting pastes.
 - [x] - Getting pastes.
-- [ ] - User endpoints.
 - [ ] - Sync client.
   - This one will take some time as I have no motivation to do it, but PRs are welcome if others want to do it.
 
 ### Installation
 This project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable release, you can always find that there.
 
 Installing via `pip`:
@@ -47,43 +43,29 @@
 
 ```py
 # async example - it will default to async
 import mystbin
 
 client = mystbin.Client()
 
-paste = await client.create_paste(filename="Hello.txt", content="Hello there!")
-# we also support passing a mystbin.File directly to the `file=` kwarg!
+file = mystbin.File(filename="File1.txt", content="Hello there!")
+file2 = mystbin.File(filename="test.py", content="print('hello!')")
+
+paste = await client.create_paste(files=[file, file2])
 
 str(paste)
 >>> 'https://mystb.in/<your generated ID>'
 
 get_paste = await client.get_paste("<your generated ID>")
 get_paste.files[0].content
 >>> "Hello there!"
 
 get_paste.created_at
 >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741)
 ```
 
-Or if you want to create a paste with multiple files...
-```py
-import mystbin
-
-file = mystbin.File(filename="File1.txt", content="Hello there!")
-file2 = mystbin.File(filename="test.py", content="print('hello!')")
-
-paste = await client.create_paste(files=[file, file2])
-
-for file in paste.files:
-    print(file.content)
-
->>> "Hello there!"
->>> "print('hello!')"
-```
-
 If you have any question please feel free to join the Pythonista Discord server:
 <div align="left">
     <a href="https://discord.gg/RAKc3HF">
         <img src="https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2" alt="Discord Server"/>
     </a>
 </div>
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
                            ************ MMyyssttbbiinn..ppyy!! ************
              _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_n_t_i_n_g_ _s_t_a_t_u_s_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]
 
 A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs
-can be found [here](https://api.mystb.in/docs). Documentation for this wrapper
-can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If you want
-the docs for the `main` branch, those can be found [here](https://
+can be found [here](https://mystb.in/api/documentation). Documentation for this
+wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If
+you want the docs for the `main` branch, those can be found [here](https://
 mystbinpy.readthedocs.io/en/latest/). ---------- ### Features - [x] - Creating
-pastes. - [ ] Supporting attachments. - [ ] - Editing pastes. - Pending design
-work. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - User endpoints.
-- [ ] - Sync client. - This one will take some time as I have no motivation to
-do it, but PRs are welcome if others want to do it. ### Installation This
-project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable
-release, you can always find that there. Installing via `pip`: ```shell python
--m pip install -U mystbin.py ``` Installing from source: ```shell python -m pip
-install git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage
-examples ```py # async example - it will default to async import mystbin client
-= mystbin.Client() paste = await client.create_paste(filename="Hello.txt",
-content="Hello there!") # we also support passing a mystbin.File directly to
-the `file=` kwarg! str(paste) >>> 'https://mystb.in/' get_paste = await
-client.get_paste("") get_paste.files[0].content >>> "Hello there!"
-get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741) ```
-Or if you want to create a paste with multiple files... ```py import mystbin
-file = mystbin.File(filename="File1.txt", content="Hello there!") file2 =
-mystbin.File(filename="test.py", content="print('hello!')") paste = await
-client.create_paste(files=[file, file2]) for file in paste.files: print
-(file.content) >>> "Hello there!" >>> "print('hello!')" ``` If you have any
-question please feel free to join the Pythonista Discord server:
+pastes. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - Sync client. -
+This one will take some time as I have no motivation to do it, but PRs are
+welcome if others want to do it. ### Installation This project will be on
+[PyPI](https://pypi.org/project/mystbin.py/) as a stable release, you can
+always find that there. Installing via `pip`: ```shell python -m pip install -
+U mystbin.py ``` Installing from source: ```shell python -m pip install
+git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage examples
+```py # async example - it will default to async import mystbin client =
+mystbin.Client() file = mystbin.File(filename="File1.txt", content="Hello
+there!") file2 = mystbin.File(filename="test.py", content="print('hello!')")
+paste = await client.create_paste(files=[file, file2]) str(paste) >>> 'https://
+mystb.in/' get_paste = await client.get_paste("") get_paste.files[0].content
+>>> "Hello there!" get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10,
+53, 57, 556741) ``` If you have any question please feel free to join the
+Pythonista Discord server:
 _[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]
```

### Comparing `mystbin_py-7.0.0/mystbin/__init__.py` & `mystbin_py-7.0.1/mystbin/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-__version__ = "7.0.0"
+__version__ = "7.0.1"
 
 from typing import Literal, NamedTuple
 
 from .client import Client as Client
 from .errors import *
 from .paste import File as File, Paste as Paste
 
@@ -35,10 +35,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=7, minor=0, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=7, minor=0, micro=1, releaselevel="final", serial=0)
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `mystbin_py-7.0.0/mystbin/client.py` & `mystbin_py-7.0.1/mystbin/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         Returns
         --------
         :class:`mystbin.Paste`
             The paste that was created.
         """
         data = await self.http.create_paste(files=files, password=password, expires=expires)
-        return Paste.from_create(data, files=files)
+        return Paste.from_create(data, files=files, http=self.http)
 
     async def delete_paste(self, security_token: str, /) -> None:
         """|coro|
 
         Delete a paste.
 
         Parameters
@@ -126,8 +126,8 @@
         --------
         Union[:class:`~mystbin.Paste`, List[:class:`str`]]
             The paste data returned.
         """
         data = await self.http.get_paste(paste_id=paste_id, password=password)
         if raw:
             return [item["content"] for item in data["files"]]
-        return Paste.from_get(data)
+        return Paste.from_get(data, http=self.http)
```

### Comparing `mystbin_py-7.0.0/mystbin/errors.py` & `mystbin_py-7.0.1/mystbin/errors.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/mystbin/http.py` & `mystbin_py-7.0.1/mystbin/http.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/mystbin/paste.py` & `mystbin_py-7.0.1/mystbin/paste.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from typing_extensions import Self
 
-    from mystbin.types.responses import CreatePasteResponse, FileResponse, GetPasteResponse
+    from .http import HTTPClient
+    from .types.responses import CreatePasteResponse, FileResponse, GetPasteResponse
 
 
 __all__ = (
     "File",
     "Paste",
 )
 
@@ -122,17 +123,19 @@
         "id",
         "author_id",
         "created_at",
         "files",
         "_security",
         "_expires",
         "_views",
+        "_http",
     )
 
-    def __init__(self, *, id: str, created_at: str, files: Sequence[File]) -> None:
+    def __init__(self, *, http: HTTPClient, id: str, created_at: str, files: Sequence[File]) -> None:
+        self._http: HTTPClient = http
         self.id: str = id
         self.created_at: datetime.datetime = datetime.datetime.fromisoformat(created_at)
         self.files: Sequence[File] = files
 
     def __str__(self) -> str:
         return self.url
 
@@ -152,17 +155,18 @@
         return self._views
 
     @property
     def security_token(self) -> str | None:
         return self._security
 
     @classmethod
-    def from_get(cls, payload: GetPasteResponse, /) -> Self:
+    def from_get(cls, payload: GetPasteResponse, /, *, http: HTTPClient) -> Self:
         files = [File.from_data(data) for data in payload["files"]]
         self = cls(
+            http=http,
             id=payload["id"],
             created_at=payload["created_at"],
             files=files,
         )
         self._views = payload["views"]
 
         expires = payload["expires"]
@@ -172,16 +176,17 @@
             self._expires = None
 
         self._security = None
 
         return self
 
     @classmethod
-    def from_create(cls, payload: CreatePasteResponse, files: Sequence[File]) -> Self:
+    def from_create(cls, payload: CreatePasteResponse, files: Sequence[File], *, http: HTTPClient) -> Self:
         self = cls(
+            http=http,
             id=payload["id"],
             created_at=payload["created_at"],
             files=files,
         )
         self._views = 0
 
         expires = payload["expires"]
@@ -189,7 +194,13 @@
             self._expires = datetime.datetime.fromisoformat(expires)
         else:
             self._expires = None
 
         self._security = payload["safety"]
 
         return self
+
+    async def delete(self) -> None:
+        if not self.security_token:
+            raise ValueError("Cannot delete a Paste with no Security Token set.")
+
+        await self._http.delete_paste(self.security_token)
```

### Comparing `mystbin_py-7.0.0/mystbin/types/__init__.py` & `mystbin_py-7.0.1/mystbin/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/mystbin/types/responses.py` & `mystbin_py-7.0.1/mystbin/types/responses.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/mystbin/utils.py` & `mystbin_py-7.0.1/mystbin/utils.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-7.0.0/pyproject.toml` & `mystbin_py-7.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mystbin-py"
-version = "7.0.0"
+version = "7.0.1"
 description = "A small simple wrapper around the mystb.in API."
 authors = ["AbstractUmbra <umbra@abstractumbra.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/PythonistaGuild/mystbin.py"
 repository = "https://github.com/PythonistaGuild/mystbin.py"
 keywords = ["mystbin", "paste"]
```

### Comparing `mystbin_py-7.0.0/PKG-INFO` & `mystbin_py-7.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystbin-py
-Version: 7.0.0
+Version: 7.0.1
 Summary: A small simple wrapper around the mystb.in API.
 Home-page: https://github.com/PythonistaGuild/mystbin.py
 License: MIT
 Keywords: mystbin,paste
 Author: AbstractUmbra
 Author-email: umbra@abstractumbra.dev
 Requires-Python: >=3.8,<4.0
@@ -42,29 +42,25 @@
     </a>
     <a href='https://github.com/PythonistaGuild/mystbin.py/actions/workflows/build.yaml'>
         <img src='https://github.com/PythonistaGuild/mystbin.py/workflows/Build/badge.svg' alt='Build status' />
     </a>
 </div>
 <br>
 
-A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs can be found [here](https://api.mystb.in/docs).
+A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs can be found [here](https://mystb.in/api/documentation).
 
 Documentation for this wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/).
 If you want the docs for the `main` branch, those can be found [here](https://mystbinpy.readthedocs.io/en/latest/).
 
 ----------
 ### Features
 
 - [x] - Creating pastes.
-  - [ ] Supporting attachments.
-- [ ] - Editing pastes.
-    - Pending design work.
 - [x] - Deleting pastes.
 - [x] - Getting pastes.
-- [ ] - User endpoints.
 - [ ] - Sync client.
   - This one will take some time as I have no motivation to do it, but PRs are welcome if others want to do it.
 
 ### Installation
 This project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable release, you can always find that there.
 
 Installing via `pip`:
@@ -81,44 +77,30 @@
 
 ```py
 # async example - it will default to async
 import mystbin
 
 client = mystbin.Client()
 
-paste = await client.create_paste(filename="Hello.txt", content="Hello there!")
-# we also support passing a mystbin.File directly to the `file=` kwarg!
+file = mystbin.File(filename="File1.txt", content="Hello there!")
+file2 = mystbin.File(filename="test.py", content="print('hello!')")
+
+paste = await client.create_paste(files=[file, file2])
 
 str(paste)
 >>> 'https://mystb.in/<your generated ID>'
 
 get_paste = await client.get_paste("<your generated ID>")
 get_paste.files[0].content
 >>> "Hello there!"
 
 get_paste.created_at
 >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741)
 ```
 
-Or if you want to create a paste with multiple files...
-```py
-import mystbin
-
-file = mystbin.File(filename="File1.txt", content="Hello there!")
-file2 = mystbin.File(filename="test.py", content="print('hello!')")
-
-paste = await client.create_paste(files=[file, file2])
-
-for file in paste.files:
-    print(file.content)
-
->>> "Hello there!"
->>> "print('hello!')"
-```
-
 If you have any question please feel free to join the Pythonista Discord server:
 <div align="left">
     <a href="https://discord.gg/RAKc3HF">
         <img src="https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2" alt="Discord Server"/>
     </a>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mystbin-py Version: 7.0.0 Summary: A small simple
+Metadata-Version: 2.1 Name: mystbin-py Version: 7.0.1 Summary: A small simple
 wrapper around the mystb.in API. Home-page: https://github.com/PythonistaGuild/
 mystbin.py License: MIT Keywords: mystbin,paste Author: AbstractUmbra Author-
 email: umbra@abstractumbra.dev Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -17,32 +17,27 @@
 https://github.com/PythonistaGuild/mystbin.py/issues Project-URL: Repository,
 https://github.com/PythonistaGuild/mystbin.py Description-Content-Type: text/
 markdown
                            ************ MMyyssttbbiinn..ppyy!! ************
              _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_n_t_i_n_g_ _s_t_a_t_u_s_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]
 
 A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs
-can be found [here](https://api.mystb.in/docs). Documentation for this wrapper
-can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If you want
-the docs for the `main` branch, those can be found [here](https://
+can be found [here](https://mystb.in/api/documentation). Documentation for this
+wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If
+you want the docs for the `main` branch, those can be found [here](https://
 mystbinpy.readthedocs.io/en/latest/). ---------- ### Features - [x] - Creating
-pastes. - [ ] Supporting attachments. - [ ] - Editing pastes. - Pending design
-work. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - User endpoints.
-- [ ] - Sync client. - This one will take some time as I have no motivation to
-do it, but PRs are welcome if others want to do it. ### Installation This
-project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable
-release, you can always find that there. Installing via `pip`: ```shell python
--m pip install -U mystbin.py ``` Installing from source: ```shell python -m pip
-install git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage
-examples ```py # async example - it will default to async import mystbin client
-= mystbin.Client() paste = await client.create_paste(filename="Hello.txt",
-content="Hello there!") # we also support passing a mystbin.File directly to
-the `file=` kwarg! str(paste) >>> 'https://mystb.in/' get_paste = await
-client.get_paste("") get_paste.files[0].content >>> "Hello there!"
-get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741) ```
-Or if you want to create a paste with multiple files... ```py import mystbin
-file = mystbin.File(filename="File1.txt", content="Hello there!") file2 =
-mystbin.File(filename="test.py", content="print('hello!')") paste = await
-client.create_paste(files=[file, file2]) for file in paste.files: print
-(file.content) >>> "Hello there!" >>> "print('hello!')" ``` If you have any
-question please feel free to join the Pythonista Discord server:
+pastes. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - Sync client. -
+This one will take some time as I have no motivation to do it, but PRs are
+welcome if others want to do it. ### Installation This project will be on
+[PyPI](https://pypi.org/project/mystbin.py/) as a stable release, you can
+always find that there. Installing via `pip`: ```shell python -m pip install -
+U mystbin.py ``` Installing from source: ```shell python -m pip install
+git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage examples
+```py # async example - it will default to async import mystbin client =
+mystbin.Client() file = mystbin.File(filename="File1.txt", content="Hello
+there!") file2 = mystbin.File(filename="test.py", content="print('hello!')")
+paste = await client.create_paste(files=[file, file2]) str(paste) >>> 'https://
+mystb.in/' get_paste = await client.get_paste("") get_paste.files[0].content
+>>> "Hello there!" get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10,
+53, 57, 556741) ``` If you have any question please feel free to join the
+Pythonista Discord server:
 _[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]
```

