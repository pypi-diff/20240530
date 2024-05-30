# Comparing `tmp/ampel_nuclear-0.8.4a0.tar.gz` & `tmp/ampel_nuclear-0.8.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_nuclear-0.8.4a0.tar", max compression
+gzip compressed data, was "ampel_nuclear-0.8.4a1.tar", max compression
```

## Comparing `ampel_nuclear-0.8.4a0.tar` & `ampel_nuclear-0.8.4a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1512 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/LICENSE
--rw-r--r--   0        0        0     2786 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/README.md
--rw-r--r--   0        0        0    10051 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/flexfit/flex_metrics.py
--rw-r--r--   0        0        0    28332 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/flexfit/flexfit.py
--rwxr-xr-x   0        0        0     9511 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t0/GaiaVeto.py
--rwxr-xr-x   0        0        0    25594 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t0/NuclearFilter.py
--rw-r--r--   0        0        0     6245 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t2/T2FlexFit.py
--rw-r--r--   0        0        0    13370 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t2/T2SimpleMetrics.py
--rwxr-xr-x   0        0        0    17392 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3MetricsPlots.py
--rwxr-xr-x   0        0        0    26001 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3PlotNeoWISE.py
--rwxr-xr-x   0        0        0    38822 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3Ranking.py
--rwxr-xr-x   0        0        0    29466 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3SummaryPlots.py
--rwxr-xr-x   0        0        0     5353 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/classifyme.py
--rw-r--r--   0        0        0    11053 2023-08-08 13:23:42.482451 ampel_nuclear-0.8.4a0/ampel/nuclear/t3/dropboxIO.py
--rw-r--r--   0        0        0  1288340 2023-08-08 13:23:42.486451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaaaflr_transientview.pickle
--rw-r--r--   0        0        0    15731 2023-08-08 13:23:42.486451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_flexresult.json
--rw-r--r--   0        0        0     2003 2023-08-08 13:23:42.486451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_simpleresult.json
--rw-r--r--   0        0        0  2446167 2023-08-08 13:23:42.490451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_transientview.pickle
--rw-r--r--   0        0        0     1815 2023-08-08 13:23:42.490451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_wisedump.json
--rw-r--r--   0        0        0     2021 2023-08-08 13:23:42.490451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/test_T2_units.py
--rw-r--r--   0        0        0     5152 2023-08-08 13:23:42.490451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/test_T3_units.py
--rw-r--r--   0        0        0      422 2023-08-08 13:23:42.490451 ampel_nuclear-0.8.4a0/ampel/nuclear/test/test_config.py
--rw-r--r--   0        0        0 30246128 2023-08-08 13:23:42.610453 ampel_nuclear-0.8.4a0/ampel/nuclear/test/transientview_list.pickle
--rw-r--r--   0        0        0     3451 2023-08-08 13:23:42.610453 ampel_nuclear-0.8.4a0/conf/ampel-nuclear/channel/TDE_RANKING.yaml
--rw-r--r--   0        0        0      226 2023-08-08 13:23:42.610453 ampel_nuclear-0.8.4a0/conf/ampel-nuclear/unit.yaml
--rw-r--r--   0        0        0     2269 2023-08-08 13:23:42.610453 ampel_nuclear-0.8.4a0/pyproject.toml
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 ampel_nuclear-0.8.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/LICENSE
+-rw-r--r--   0        0        0     4697 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/README.md
+-rw-r--r--   0        0        0    10051 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/ampel/nuclear/flexfit/flex_metrics.py
+-rw-r--r--   0        0        0    28332 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/ampel/nuclear/flexfit/flexfit.py
+-rwxr-xr-x   0        0        0     9511 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/ampel/nuclear/t0/GaiaVeto.py
+-rwxr-xr-x   0        0        0    25594 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/ampel/nuclear/t0/NuclearFilter.py
+-rw-r--r--   0        0        0     6245 2024-05-30 14:15:46.227177 ampel_nuclear-0.8.4a1/ampel/nuclear/t2/T2FlexFit.py
+-rw-r--r--   0        0        0    13370 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t2/T2SimpleMetrics.py
+-rwxr-xr-x   0        0        0    17390 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3MetricsPlots.py
+-rwxr-xr-x   0        0        0    25993 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3PlotNeoWISE.py
+-rwxr-xr-x   0        0        0    38725 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3Ranking.py
+-rwxr-xr-x   0        0        0    29367 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3SummaryPlots.py
+-rwxr-xr-x   0        0        0     5353 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/classifyme.py
+-rw-r--r--   0        0        0    11265 2024-05-30 14:15:46.231177 ampel_nuclear-0.8.4a1/ampel/nuclear/t3/dropboxIO.py
+-rw-r--r--   0        0        0  1288340 2024-05-30 14:15:46.235177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaaaflr_transientview.pickle
+-rw-r--r--   0        0        0    15731 2024-05-30 14:15:46.235177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_flexresult.json
+-rw-r--r--   0        0        0     2003 2024-05-30 14:15:46.235177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_simpleresult.json
+-rw-r--r--   0        0        0  2446167 2024-05-30 14:15:46.239177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_transientview.pickle
+-rw-r--r--   0        0        0     1815 2024-05-30 14:15:46.239177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_wisedump.json
+-rw-r--r--   0        0        0     2021 2024-05-30 14:15:46.239177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/test_T2_units.py
+-rw-r--r--   0        0        0     5152 2024-05-30 14:15:46.239177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/test_T3_units.py
+-rw-r--r--   0        0        0      422 2024-05-30 14:15:46.239177 ampel_nuclear-0.8.4a1/ampel/nuclear/test/test_config.py
+-rw-r--r--   0        0        0 30246128 2024-05-30 14:15:46.343178 ampel_nuclear-0.8.4a1/ampel/nuclear/test/transientview_list.pickle
+-rw-r--r--   0        0        0     3451 2024-05-30 14:15:46.343178 ampel_nuclear-0.8.4a1/conf/ampel-nuclear/channel/TDE_RANKING.yaml
+-rw-r--r--   0        0        0      226 2024-05-30 14:15:46.343178 ampel_nuclear-0.8.4a1/conf/ampel-nuclear/unit.yaml
+-rw-r--r--   0        0        0     2258 2024-05-30 14:15:46.343178 ampel_nuclear-0.8.4a1/pyproject.toml
+-rw-r--r--   0        0        0     5689 1970-01-01 00:00:00.000000 ampel_nuclear-0.8.4a1/PKG-INFO
```

### Comparing `ampel_nuclear-0.8.4a0/LICENSE` & `ampel_nuclear-0.8.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/flexfit/flex_metrics.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/flexfit/flex_metrics.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/flexfit/flexfit.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/flexfit/flexfit.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t0/GaiaVeto.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t0/GaiaVeto.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t0/NuclearFilter.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t0/NuclearFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t2/T2FlexFit.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t2/T2FlexFit.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t2/T2SimpleMetrics.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t2/T2SimpleMetrics.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3MetricsPlots.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3MetricsPlots.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     )
             else:
                 self.logger.warn(
                     "empty simple metrics for source {}".format(tran_name)
                 )
             
             self.maybe_commit()
-        self.commit()
+        self.done()
         return None
 
     def get_ps1(self, simple, ps1_match, filepath):
         metrics, plot_info = simple["metrics"], simple["plot_info"]
         ps1_ra, ps1_dec = ps1_match["RA"], ps1_match["Dec"]
         dra_ps1 = (np.array(metrics["ra"]) - ps1_ra) * 3600  # mean dra
         ddec_ps1 = (np.array(metrics["dec"]) - ps1_dec) * 3600  # mean dec
```

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3PlotNeoWISE.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3PlotNeoWISE.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
             )
             ax.set_title(titstr, fontsize=11)
             ax.legend()
             fig.tight_layout()
 
             plot_fname = f"{filebase}-neoWISE.pdf"
             buf = io.BytesIO()
-            ax.figure.savefig(buf, format="pdf")
+            fig.savefig(buf, format="pdf")
             buf.seek(0)
             self.put(plot_fname, buf.read())
             self.logger.debug(f"plotting {tran_name}")
             ax.clear()
 
             self.maybe_commit()
 
@@ -544,15 +544,15 @@
             )
 
             buf = io.BytesIO()
             buf.write(bytes(json.dumps(data_log, indent=3), "utf-8"))
             buf.seek(0)
             self.put(self.save_location + "/neowise_log.json", buf.read())
 
-            self.commit()
+            self.done()
         return None
 
     def binthem(
         self,
         x,
         y,
         yerr=None,
```

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3Ranking.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3Ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,21 +615,15 @@
             (1, 0.3, 0.5, 0.8, 0.8, 0.5, None, 0.9),
             ("d", ".", "s", "o", None, "x"),
         )
         mew = 0.6
         lw = 0.6
         ms = 2
 
-        # ---
-
-        # ----
-        # color maps obsession
-        # cmap = mpl.cm.get_cmap('magma')
-
-        cmap = mpl.cm.get_cmap("viridis")
+        cmap = mpl.colormaps.get_cmap("viridis")
         manual_colors = [cmap(0.1)] + [
             cmap(0.65),
             cmap(0.65),
             cmap(0.65),
             cmap(0.35),
             cmap(0.92),
         ]
```

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/T3SummaryPlots.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/T3SummaryPlots.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,21 +306,15 @@
             (1, 0.3, 0.5, 0.8, 0.8, 0.5, None, 0.9),
             ("d", ".", "s", "o", None, "x"),
         )
         mew = 0.6
         lw = 0.6
         ms = 2
 
-        # ---
-
-        # ----
-        # color maps obsession
-        # cmap = mpl.cm.get_cmap('magma')
-
-        cmap = mpl.cm.get_cmap("viridis")
+        cmap = mpl.colormaps.get_cmap("viridis")
         manual_colors = [cmap(0.1)] + [
             cmap(0.65),
             cmap(0.65),
             cmap(0.65),
             cmap(0.35),
             cmap(0.92),
         ]
@@ -738,15 +732,15 @@
         )
         self.plt2box(plt, plot_fname)
 
         # as a bonus: write a file with the names of TDE candidates (based on some boxing)
         # for each of the plots (requested by Suvi)
         self.put(plot_dir + "/boxed.txt", bytes(finfo, "utf-8"))
 
-        self.commit()
+        self.done()
 
     def collect_metrics(self, transients):
         """ """
         jd_today = self.night.jd
 
         alert_name = "/mampel/alerts"
         alert_folders = self.get_files(alert_name)
```

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/classifyme.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/classifyme.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/t3/dropboxIO.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/t3/dropboxIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,16 @@
     def process(
         self, gen: Generator[TransientView, T3Send, None], t3s: Optional[T3Store] = None
     ) -> Union[UBson, UnitResult]:
         """ """
         return None
 
     def done(self):
-        self.commit()
+        if not self.commit():
+            raise RuntimeError("upload failed")
         self.logger.info(
             f"Wrote {self.stats['bytes']/2**20:.3f} MB in {self.stats['files']} files"
         )
 
     @handle_disconnects
     def create_folder(self, path):
         if self.dryRun:
@@ -160,17 +161,18 @@
         else:
             self._payloads.append((payload, path, len(payload)))
         self.stats["bytes"] += len(payload)
         self.stats["files"] += 1
 
     def maybe_commit(self) -> None:
         if sum(size for _, _, size in self._payloads) >= self.buffer_size_mb * (1<<20):
-            return self.commit() 
+            self.commit() 
 
-    def commit(self) -> None:
+    @backoff.on_predicate(backoff.expo, factor=10, max_tries=5)
+    def commit(self) -> bool:
 
         # Dropbox cannot handle queues containing more than 1000 files
         payload_subsets = [
             self._payloads[i : i + 1000] for i in range(0, len(self._payloads), 1000)
         ]
         self._payloads.clear()
 
@@ -199,15 +201,15 @@
                         ),
                         commit=dropbox.files.CommitInfo(
                             path=path, mode=dropbox.files.WriteMode.overwrite
                         ),
                     )
                 )
             if not entries:
-                return
+                continue
 
             self.logger.info(f"committing {len(entries)} uploads")
             launch_result = handle_disconnects(
                 self.dbx.files_upload_session_finish_batch
             )(entries)
             if not launch_result.is_complete():
                 status = backoff.on_predicate(
@@ -215,21 +217,22 @@
                     predicate=lambda job_status: job_status.is_in_progress(),
                     max_time=300,
                     max_value=5,
                 )(handle_disconnects(self.dbx.files_upload_session_finish_batch_check))(
                     launch_result.get_async_job_id()
                 )
                 assert status.is_complete()
-                for future, result in zip(
-                    list(futures.keys()), status.get_complete().entries
+                for future, result, item in zip(
+                    list(futures.keys()), status.get_complete().entries, payload_subset
                 ):
-                    if result.is_success():
-                        del futures[future]
-                    else:
-                        raise RuntimeError(str(result.get_failure()))
+                    del futures[future]
+                    if result.is_failure():
+                        self._payloads.append(item)
+                        self.logger.error(f"{result.get_failure()} for {item[1]}")
+        return len(self._payloads) == 0
 
     @lru_cache(maxsize=1024)
     @handle_disconnects
     def get_files(self, path):
         if not self.dbx:
             self.dbx = dbx
         entries = []
```

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaaaflr_transientview.pickle` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaaaflr_transientview.pickle`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_flexresult.json` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_flexresult.json`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_simpleresult.json` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_simpleresult.json`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_transientview.pickle` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_transientview.pickle`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/ZTF20aaadtjq_wisedump.json` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/ZTF20aaadtjq_wisedump.json`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/test_T2_units.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/test_T2_units.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/test_T3_units.py` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/test_T3_units.py`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/ampel/nuclear/test/transientview_list.pickle` & `ampel_nuclear-0.8.4a1/ampel/nuclear/test/transientview_list.pickle`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/conf/ampel-nuclear/channel/TDE_RANKING.yaml` & `ampel_nuclear-0.8.4a1/conf/ampel-nuclear/channel/TDE_RANKING.yaml`

 * *Files identical despite different names*

### Comparing `ampel_nuclear-0.8.4a0/pyproject.toml` & `ampel_nuclear-0.8.4a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-nuclear"
-version = "0.8.4a0"
+version = "0.8.4a1"
 license = "BSD-3-Clause"
 readme = "README.md"
 description = "Astronomy units for the Ampel system to analyze nuclear events like TDEs"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-nuclear"
 authors = [
     "Valery Brinnel",
@@ -30,30 +30,30 @@
     'conf/*/*/*.yaml',
     'conf/*/*.yml',
     'conf/*/*/*.yml',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-ampel-interface = "^0.8.7"
-ampel-ztf = {version = ">=0.8.5,<0.8.6", source = "pypi"}
-ampel-hu-astro = {version = ">=0.8.3a10,<0.8.4", source = "pypi", extras = ["slack", "sncosmo"]}
+ampel-interface = ">=0.8.7,<0.9"
+ampel-ztf = {version = ">=0.8.5,<0.9", source = "pypi"}
+ampel-hu-astro = {version = ">=0.8.3a10,<0.9", source = "pypi", extras = ["slack", "sncosmo"]}
 dropbox = "^11.36.0"
 corner = "^2.2.1"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.3.0"
-pytest = "^7.3.1"
-pytest-cov = "^4.1.0"
+pytest = "^8.0.2"
+pytest-cov = "^5.0.0"
 pytest-mock = "^3.10.0"
 types-requests = "^2.25.9"
 types-pytz = "^2022.1.2"
 pre-commit = "^3.3.2"
 # duplicate to add a dev extra
-ampel-ztf = {version = ">=0.8.5,<0.8.6", source = "pypi", extras = ["kafka"]}
+ampel-ztf = {version = "*", source = "pypi", extras = ["kafka"]}
 
 [tool.conda-lock]
 channels = ["conda-forge"]
 platforms = ["linux-64", "osx-64", "osx-arm64"]
 
 [tool.conda-lock.dependencies]
 python-confluent-kafka = "1.7"
```

