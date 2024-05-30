# Comparing `tmp/pytest_cleanslate-1.0.3.tar.gz` & `tmp/pytest_cleanslate-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_cleanslate-1.0.3.tar", last modified: Tue May 28 19:49:40 2024, max compression
+gzip compressed data, was "pytest_cleanslate-1.0.4.tar", last modified: Thu May 30 16:28:21 2024, max compression
```

## Comparing `pytest_cleanslate-1.0.3.tar` & `pytest_cleanslate-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.843793 pytest_cleanslate-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.843793 pytest_cleanslate-1.0.3/src/pytest_cleanslate/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 19:49:40.000000 pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:49:40.847792 pytest_cleanslate-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/tests/test_cleanslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-28 19:49:31.000000 pytest_cleanslate-1.0.3/tests/test_reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/src/pytest_cleanslate/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:28:21.000000 pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:28:21.134407 pytest_cleanslate-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/tests/test_cleanslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-30 16:28:12.000000 pytest_cleanslate-1.0.4/tests/test_reduce.py
```

### Comparing `pytest_cleanslate-1.0.3/LICENSE` & `pytest_cleanslate-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.3/PKG-INFO` & `pytest_cleanslate-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.3
+Version: 1.0.4
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
 Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
+Requires-Dist: tqdm
 
 # pytest-cleanslate: work around or find test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
```

### Comparing `pytest_cleanslate-1.0.3/README.md` & `pytest_cleanslate-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.3/pyproject.toml` & `pytest_cleanslate-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 authors = [
     { name="Juan Altmayer Pizzorno", email="juan@altmayer.com" },
 ]
 dependencies = [
     "pytest",
     "py",
     "pytest-forked",
+    "tqdm",
 ]
 
 [project.urls]
 "Repository" = "https://github.com/plasma-umass/pytest_cleanslate"
 
 [project.entry-points.pytest11]
 pytest_cleanslate = "pytest_cleanslate.plugin"
```

### Comparing `pytest_cleanslate-1.0.3/src/pytest_cleanslate/plugin.py` & `pytest_cleanslate-1.0.4/src/pytest_cleanslate/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.3/src/pytest_cleanslate/reduce.py` & `pytest_cleanslate-1.0.4/src/pytest_cleanslate/reduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 from _pytest.pathlib import Path
 import typing as T
 import json
 import sys
 from .__version__ import __version__
+import tqdm
+import math
 
 
 PYTEST_ARGS = ('-qq', '-p', 'pytest_cleanslate.reduce')
 MODULE_LIST_ARG = '--module-list-from'
 TEST_LIST_ARG = '--test-list-from'
 RESULTS_ARG = '--results-to'
 
@@ -124,26 +126,29 @@
 
     def get_tests(self) -> T.List[str]:
         return [r['id'] for r in self._results['run']]
 
     def get_first_failed(self) -> T.Union[None, str]:
         return next(iter(o['id'] for o in self._results['collect'] + self._results['run'] if o['outcome'] == 'failed'), None)
 
-    def get_module(self, testid: str) -> str:
-        return testid.split('::')[0]
 
-    def is_module(self, testid: str) -> bool:
-        return '::' not in testid
+def _get_module(testid: str) -> str:
+    return testid.split('::')[0]
+
+
+def _is_module(testid: str) -> bool:
+    return '::' not in testid
 
 
 def _run_pytest(tests_path: Path, extra_args=(), *,
                 modules: T.List[Path] = None, tests: T.List[str] = None, trace: bool = False) -> dict:
     import tempfile
     import subprocess
 
+    # Specifying dir='.' here works around weird failures running tests on MacOS
     with tempfile.TemporaryDirectory(dir='.') as tmpdir:
         tmpdir = Path(tmpdir)
 
         results = tmpdir / "results.json"
 
         if modules:
             modulelist = tmpdir / "modules.txt"
@@ -169,137 +174,158 @@
         if p.returncode not in (pytest.ExitCode.OK, pytest.ExitCode.TESTS_FAILED,
                                 pytest.ExitCode.INTERRUPTED, pytest.ExitCode.NO_TESTS_COLLECTED):
             p.check_returncode()
 
         return Results(results)
 
 
-def _bisect_items(items: T.List[str], failing: str, fails: T.Callable[[T.List[str], str], bool]) -> T.List[str]:
+def _bisect_items(items: T.List[str], failing: str, fails: T.Callable[[T.List[str], str], bool],
+                  *, bar: "tqdm") -> T.List[str]:
     assert failing not in items
 
     while len(items) > 1:
-        print(f"    {len(items)}")
         middle = len(items) // 2
 
+        bar.refresh() # for when using --trace
+        bar.set_postfix({"remaining": len(items)})
+        bar.update()
+
         if fails(items[:middle]+[failing]):
             items = items[:middle]
             continue
 
         if fails(items[middle:]+[failing]):
             items = items[middle:]
             continue
 
         # TODO could do the rest of delta debugging here
         break
 
     if len(items) == 1 and fails([failing]):
         items = []
 
-    print(f"    {len(items)}")
+    bar.refresh() # for when using --trace
+    bar.set_postfix({"remaining": len(items)})
+    bar.update()
+
     return items
 
 
-def _reduce_tests(tests_path: Path, tests: T.List[str], failing_test: str, *, trace=None) -> T.List[str]:
+def _reduce_tests(tests_path: Path, tests: T.List[str], failing_test: str, modules: T.List[str],
+                  *, trace: bool = False, pytest_args: T.List[str] = ()) -> T.List[str]:
     def fails(test_set: T.List[str]):
-        trial = _run_pytest(tests_path, ('-x',), tests=test_set, trace=trace)
+        trial = _run_pytest(tests_path, (*pytest_args, '--continue-on-collection-errors'),
+                            tests=test_set, modules=modules, trace=trace)
         return trial.get_outcome(failing_test) == 'failed'
 
-    return _bisect_items(tests, failing_test, fails)
+    module_set = {*modules}
+    tests = [t for t in tests if t != failing_test and _get_module(t) in module_set]
+    if not tests:
+        return tests
+
+    steps=math.ceil(math.log(len(tests), 2))
+    with tqdm.tqdm(desc="Trying to reduce tests.....", total=steps) as bar:
+        return _bisect_items(tests, failing_test, fails, bar=bar)
 
 
-def _reduce_modules(tests_path: Path, tests: T.List[str], failing_test: str,
-                    modules: T.List[str], failing_module: str, *, trace=None) -> T.List[str]:
-    def fails(module_set: T.List[str]):
-        trial = _run_pytest(tests_path, ('-x',), tests=tests, modules=module_set, trace=trace)
-        return trial.get_outcome(failing_test) == 'failed'
+def _reduce_modules(tests_path: Path, tests: T.List[str], failing_id: str,
+                    modules: T.List[str], failing_module: str,
+                    *, trace: bool = False, pytest_args: T.List[str] = ()) -> T.List[str]:
 
-    return _bisect_items(modules, failing_module, fails)
+    def fails(module_set: T.List[str]):
+        trial = _run_pytest(tests_path, (*pytest_args, '--continue-on-collection-errors',),
+                            tests=tests, modules=module_set, trace=trace)
+        return trial.get_outcome(failing_id) == 'failed'
+
+    modules = [m for m in modules if m != failing_module]
+    if not modules:
+        return modules
+
+    steps = math.ceil(math.log(len(modules), 2))
+    with tqdm.tqdm(desc="Trying to reduce modules...", total=steps) as bar:
+        return _bisect_items(modules, failing_module, fails, bar=bar)
 
 
 def _parse_args():
     import argparse
 
     bool_action = argparse.BooleanOptionalAction if sys.version_info[:2] >= (3,9) else "store_true"
 
     ap = argparse.ArgumentParser()
     ap.add_argument('--trace', default=False, action=bool_action, help='show pytest outputs, etc.')
     ap.add_argument('--save-to', type=Path, help='file where to save results (JSON)')
+    ap.add_argument('--pytest-args', type=str, default='', help='extra arguments to pass to pytest')
     ap.add_argument('--version', action='version',
                     version=f"%(prog)s v{__version__} (Python {'.'.join(map(str, sys.version_info[:3]))})")
     ap.add_argument('tests_path', type=Path, help='tests file or directory')
 
     return ap.parse_args()
 
 
 def main():
     args = _parse_args()
+    pytest_args = args.pytest_args.split()
 
     print("Running tests...", flush=True)
-    results = _run_pytest(args.tests_path, ('-x',), trace=args.trace)
+    results = _run_pytest(args.tests_path, (*pytest_args, '-x'), trace=args.trace)
 
-    failed = results.get_first_failed()
-    if failed is None:
+    failed_id = results.get_first_failed()
+    if failed_id is None:
         print("No tests failed!", flush=True)
         if args.save_to:
             with args.save_to.open("w") as f:
                 json.dump({
-                    'failed': failed,
+                    'failed': failed_id,
                     'error': 'No tests failed',
                 }, f)
         return 1
 
-    is_module = results.is_module(failed)
-
-    if is_module:
+    failed_is_module = _is_module(failed_id)
+    if failed_is_module:
         if args.trace: print()
-        print(f"Module \"{failed}\"'s collection failed; trying it by itself...", flush=True)
-        failed_module = failed
-        solo = _run_pytest(args.tests_path, ('-x',), modules=[failed_module], trace=args.trace)
+        print(f"Module \"{failed_id}\"'s collection failed; trying it by itself...", flush=True)
+        failed_module = failed_id
+        tests = None
     else:
         if args.trace: print()
-        print(f"Test \"{failed}\" failed; trying it by itself...", flush=True)
-        failed_module = results.get_module(failed)
-
-        solo = _run_pytest(args.tests_path, ('-x',), modules=[failed_module], tests=[failed], trace=args.trace)
+        print(f"Test \"{failed_id}\" failed; trying it by itself...", flush=True)
+        failed_module = _get_module(failed_id)
+        tests = [failed_id]
 
-    if solo.get_outcome(failed) != 'passed':
+    solo = _run_pytest(args.tests_path, pytest_args, modules=[failed_module], tests=tests, trace=args.trace)
+    if solo.get_outcome(failed_id) != 'passed':
         print("That also fails by itself!", flush=True)
         if args.save_to:
             with args.save_to.open("w") as f:
                 json.dump({
-                    'failed': failed,
-                    'error': f'{"Module" if is_module else "Test"} also fails by itself',
+                    'failed': failed_id,
+                    'error': f'{"Module" if failed_is_module else "Test"} also fails by itself',
                 }, f)
         return 1
 
     tests = results.get_tests()
-    if not is_module:
-        assert tests[-1] == failed
-        tests = tests[:-1]
-
-        if args.trace: print()
-        print("Trying to reduce test set...", flush=True)
-        tests = _reduce_tests(args.tests_path, tests, failed)
 
     if args.trace: print()
-    print("Trying to reduce module set...", flush=True)
+    modules = _reduce_modules(args.tests_path, tests, failed_id, results.get_modules(), failed_module,
+                              trace=args.trace, pytest_args=pytest_args)
 
-    modules = [m for m in results.get_modules() if m != failed_module]
-    modules = _reduce_modules(args.tests_path, tests if is_module else tests + [failed], failed, modules, failed_module)
+    if args.trace: print()
+    tests = _reduce_tests(args.tests_path, tests, failed_id, [*modules, failed_module],
+                          trace=args.trace, pytest_args=pytest_args)
 
     if args.trace: print()
     print("Reduced failure set:")
     print(f"    modules: {modules}")
     print(f"    tests: {tests}")
     print(flush=True)
 
     if args.save_to:
         with args.save_to.open("w") as f:
             json.dump({
-                'failed': failed,
+                'failed': failed_id,
                 'modules': modules,
                 'tests': tests,
             }, f)
 
     return 0
 
 if __name__ == "__main__":
```

### Comparing `pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/PKG-INFO` & `pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.3
+Version: 1.0.4
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
 Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
+Requires-Dist: tqdm
 
 # pytest-cleanslate: work around or find test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
```

### Comparing `pytest_cleanslate-1.0.3/src/pytest_cleanslate.egg-info/SOURCES.txt` & `pytest_cleanslate-1.0.4/src/pytest_cleanslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.3/tests/test_cleanslate.py` & `pytest_cleanslate-1.0.4/tests/test_cleanslate.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,24 @@
     'exception': 'raise RuntimeError("test")',
     'kill': 'os.kill(os.getpid(), 9)',
     'exit': 'pytest.exit("goodbye")',
     'interrupt': 'raise KeyboardInterrupt()'
 }
 
 def make_polluted_suite(tests_dir: Path, *, pollute_in_collect: bool = True, fail_collect: bool = False,
-                        fail_kind: str = 'assert'):
+                        fail_kind: str = 'assert', polluter_seq: int = None, failing_seq: int = None):
     """in a suite with 10 tests, 'polluter' doesn't fail, but causes 'failing' to fail."""
-    tests = list(range(10))
-
     # note the polluter must run before the failing test
+    N_TESTS = 10
+
+    assert (polluter_seq is None and failing_seq is None) or (failing_seq > polluter_seq)
+
+    if polluter_seq is None:
+        polluter_seq = random.choice(range(N_TESTS-1))
 
-    polluter_seq = tests.pop(random.choice(tests[:-1]))
     polluter = seq2p(tests_dir, polluter_seq)
     if pollute_in_collect:
         polluter.write_text(dedent("""\
             import sys
             sys.foobar=True
 
             def test_bar():
@@ -47,15 +50,18 @@
                 assert True
 
             def test_bar():
                 assert True
             """))
         polluter = f"{polluter}::test_polluter"
 
-    failing = seq2p(tests_dir, tests.pop(random.choice(range(polluter_seq, len(tests)))))
+    if failing_seq is None:
+        failing_seq = random.choice(range(polluter_seq+1, N_TESTS))
+
+    failing = seq2p(tests_dir, failing_seq)
     if fail_collect:
         failing.write_text(dedent(f"""\
             import sys
             import os
             import pytest
 
             if getattr(sys, 'foobar', False):
@@ -75,14 +81,15 @@
                     {FAILURES[fail_kind]}
 
             def test_ok():
                 assert True
             """))
         failing = f"{failing}::test_failing"
 
+    tests = [seq for seq in range(N_TESTS) if seq not in (polluter_seq, failing_seq)]
     for seq in tests:
         seq2p(tests_dir, seq).write_text('def test_foo(): pass')
 
     return str(failing), str(polluter), tests
 
 
 @pytest.fixture
@@ -248,7 +255,29 @@
 
     # --stepwise sets session.shouldstop upon a test failure.
     p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', '--stepwise', '-s', tests_dir], check=False,
                        capture_output=True)
     assert p.returncode == pytest.ExitCode.INTERRUPTED
     assert not Path('litmus.txt').exists()
     assert 'CRASHED' not in str(p.stdout, 'utf-8')
+
+
+def test_polluter_test_in_single_module(tests_dir):
+    test = seq2p(tests_dir, 0)
+    test.write_text(dedent("""\
+        import sys
+
+        def test_polluter():
+            sys.needs_this = True
+            assert True
+
+        def test_nothing():
+            assert True
+
+        def test_failing():
+            assert not hasattr(sys, 'needs_this')
+        """))
+
+    reduction_file = tests_dir.parent / "reduction.json"
+
+    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', tests_dir], check=False)
+    assert p.returncode == pytest.ExitCode.OK
```

