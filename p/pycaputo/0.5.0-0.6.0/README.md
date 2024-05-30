# Comparing `tmp/pycaputo-0.5.0.tar.gz` & `tmp/pycaputo-0.6.0.tar.gz`

## Comparing `pycaputo-0.5.0.tar` & `pycaputo-0.6.0.tar`

### file list

```diff
@@ -1,106 +1,111 @@
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.broken.gitlab-ci.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.codespell-ignore
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 pycaputo-0.5.0/Makefile
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pycaputo-0.5.0/requirements-dev.txt
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pycaputo-0.5.0/requirements.txt
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.reuse/dep5
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 pycaputo-0.5.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pycaputo-0.5.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/Makefile
--rw-r--r--   0        0        0    60118 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-dark.svg
--rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-light.svg
--rw-r--r--   0        0        0    66576 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-dark.svg
--rw-r--r--   0        0        0    64378 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-light.svg
--rw-r--r--   0        0        0    67299 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/caputo-derivative-l1-dark.svg
--rw-r--r--   0        0        0    65147 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/caputo-derivative-l1-light.svg
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/changelog.rst
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/controllers.rst
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/differentiation.rst
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/fode.rst
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/history.rst
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/index.rst
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/integrate_fire.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/misc.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/operator.rst
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/quadrature.rst
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/references.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/timestepping.rst
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/tutorials.rst
--rw-r--r--   0        0        0   182839 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-dark.svg
--rw-r--r--   0        0        0   180507 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-light.svg
--rw-r--r--   0        0        0   233122 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-dark.svg
--rw-r--r--   0        0        0   230498 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-light.svg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/benchmarks/Linux-CPython-3.11-64bit/0001_561ba4947e7fa72377b82f411a1f0eb91929763c_20240408_123818.json
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/brusselator-predictor-corrector.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-derivative-l1.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-derivative-quadratic.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-gradient-spectral.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-custom-diff.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-custom-quad.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-lipschitz-weibull.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-ad-ex.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-eif.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-lif.py
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-pif.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/lorenz-weighted-euler.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/van-der-pol-adaptive-pece.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 pycaputo-0.5.0/scripts/benchmark-boxplot.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 pycaputo-0.5.0/scripts/generate-doc-figures.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/__init__.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/benchmark.py
--rw-r--r--   0        0        0    27855 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/controller.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/derivatives.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/events.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/finite_difference.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/generating_functions.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/grid.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/history.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/implicit.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/interpolation.py
--rw-r--r--   0        0        0    12371 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/jacobi.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/lagrange.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/lipschitz.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/logging.py
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/mittagleffler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/py.typed
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/stepping.py
--rw-r--r--   0        0        0    25864 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/utils.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/__init__.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/base.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/caputo.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/riemann_liouville.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/__init__.py
--rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/caputo.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/product_integration.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/__init__.py
--rw-r--r--   0        0        0    19297 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/ad_ex.py
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/base.py
--rw-r--r--   0        0        0    12039 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/eif.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/lif.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/pif.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/spikes.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/base.py
--rw-r--r--   0        0        0    15259 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/riemann_liouville.py
--rw-r--r--   0        0        0    37732 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/mittag_leffler_ref.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_diff_caputo.py
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_diff_riemann_liouville.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_finite_difference.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_fode.py
--rw-r--r--   0        0        0     7382 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_fode_caputo.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_generating_functions.py
--rw-r--r--   0        0        0    13909 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_integrate_fire.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_interpolation.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_jacobi.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_misc.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_mittag_leffler.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_points.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_quad_riemann_liouville.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/benchmarks/test_bench_diff.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.gitignore
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pycaputo-0.5.0/README.rst
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 pycaputo-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pycaputo-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pycaputo-0.6.0/.broken.gitlab-ci.yml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pycaputo-0.6.0/.codespell-ignore
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pycaputo-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 pycaputo-0.6.0/Makefile
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pycaputo-0.6.0/requirements-dev.txt
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pycaputo-0.6.0/requirements.txt
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pycaputo-0.6.0/.reuse/dep5
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 pycaputo-0.6.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pycaputo-0.6.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0    60118 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/brusselator-predictor-corrector-cycle-dark.svg
+-rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/brusselator-predictor-corrector-cycle-light.svg
+-rw-r--r--   0        0        0    66576 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/brusselator-predictor-corrector-dark.svg
+-rw-r--r--   0        0        0    64378 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/brusselator-predictor-corrector-light.svg
+-rw-r--r--   0        0        0    67299 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/caputo-derivative-l1-dark.svg
+-rw-r--r--   0        0        0    65147 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/caputo-derivative-l1-light.svg
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/controllers.rst
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/differentiation.rst
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/fode.rst
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/history.rst
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/integrate_fire.rst
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/literature.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/misc.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/operator.rst
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/quadrature.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/timestepping.rst
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/tutorials.rst
+-rw-r--r--   0        0        0   182839 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-eest-dark.svg
+-rw-r--r--   0        0        0   180507 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-eest-light.svg
+-rw-r--r--   0        0        0   233122 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-solution-dark.svg
+-rw-r--r--   0        0        0   230498 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-solution-light.svg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 pycaputo-0.6.0/docs/benchmarks/Linux-CPython-3.11-64bit/0001_561ba4947e7fa72377b82f411a1f0eb91929763c_20240408_123818.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/brusselator-predictor-corrector.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/caputo-derivative-l1.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/caputo-derivative-quadratic.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/caputo-gradient-spectral.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/example-custom-diff.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/example-custom-quad.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/example-lipschitz-weibull.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/integrate-and-fire-ad-ex.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/integrate-and-fire-eif.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/integrate-and-fire-lif.py
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/integrate-and-fire-pif.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/lorenz-weighted-euler.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/mittag-leffler-accuracy.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/mittag-leffler-function.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/trapezoidal-quadrature-error.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pycaputo-0.6.0/examples/van-der-pol-adaptive-pece.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 pycaputo-0.6.0/scripts/benchmark-boxplot.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 pycaputo-0.6.0/scripts/generate-doc-figures.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/__init__.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/benchmark.py
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/controller.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/derivatives.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/events.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/finite_difference.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/generating_functions.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/grid.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/history.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/implicit.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/interpolation.py
+-rw-r--r--   0        0        0    12371 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/jacobi.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/lagrange.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/lipschitz.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/logging.py
+-rw-r--r--   0        0        0    21253 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/mittagleffler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/py.typed
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/stepping.py
+-rw-r--r--   0        0        0    26452 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/utils.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/differentiation/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/differentiation/base.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/differentiation/caputo.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/differentiation/riemann_liouville.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/fode/__init__.py
+-rw-r--r--   0        0        0    26524 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/fode/caputo.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/fode/product_integration.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/fode/special.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/__init__.py
+-rw-r--r--   0        0        0    19297 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/ad_ex.py
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/base.py
+-rw-r--r--   0        0        0    12039 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/eif.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/lif.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/pif.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/integrate_fire/spikes.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/quadrature/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/quadrature/base.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pycaputo-0.6.0/src/pycaputo/quadrature/riemann_liouville.py
+-rw-r--r--   0        0        0    46240 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/mittag_leffler_ref.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_diff_caputo.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_diff_riemann_liouville.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_finite_difference.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_fode.py
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_fode_caputo.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_generating_functions.py
+-rw-r--r--   0        0        0    13909 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_integrate_fire.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_interpolation.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_jacobi.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_lagrange.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_misc.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_mittag_leffler.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_points.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/test_quad_riemann_liouville.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pycaputo-0.6.0/tests/benchmarks/test_bench_diff.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pycaputo-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pycaputo-0.6.0/README.rst
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 pycaputo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 pycaputo-0.6.0/PKG-INFO
```

### Comparing `pycaputo-0.5.0/Makefile` & `pycaputo-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/LICENSES/CC0-1.0.txt` & `pycaputo-0.6.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/LICENSES/MIT.txt` & `pycaputo-0.6.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/Makefile` & `pycaputo-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-dark.svg` & `pycaputo-0.6.0/docs/brusselator-predictor-corrector-cycle-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-light.svg` & `pycaputo-0.6.0/docs/brusselator-predictor-corrector-cycle-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/brusselator-predictor-corrector-dark.svg` & `pycaputo-0.6.0/docs/brusselator-predictor-corrector-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/brusselator-predictor-corrector-light.svg` & `pycaputo-0.6.0/docs/brusselator-predictor-corrector-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/caputo-derivative-l1-dark.svg` & `pycaputo-0.6.0/docs/caputo-derivative-l1-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/caputo-derivative-l1-light.svg` & `pycaputo-0.6.0/docs/caputo-derivative-l1-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/changelog.rst` & `pycaputo-0.6.0/docs/changelog.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,64 @@
 Changelog
 =========
 
+pycaputo 0.6.0 (May 30, 2024)
+-----------------------------
+
+Features
+^^^^^^^^
+
+* Implement Riemann-Lioville quadrature based on high-order Lagrange polynomials
+  in :class:`~pycaputo.quadrature.riemann_liouville.SplineLagrange`. These methods
+  require knowledge of the function :math:`f` being integrated, but can obtain
+  high order :math:`> 3`.
+* Implement the implicit :class:`~pycaputo.fode.caputo.Trapezoidal` and
+  :class:`~pycaputo.fode.caputo.ExplicitTrapezoidal` methods. These methods are
+  closely related to the standard :class:`~pycaputo.fode.caputo.PECE` method.
+  The implicit method has better stability.
+* Implement the Mittag-Leffler algorithm from [Garrappa2015]_.
+* Added the :mod:`pycaputo.fode.special` module with some exact solutions. This
+  is subject to a lot of change, but in general it is desired to have some
+  examples for testing and demonstration.
+
+Changes
+^^^^^^^
+
+* The base :class:`~pycaputo.derivatives.FractionalOperator` no longer defines
+  an ``order`` attribute. This does not make sense for more complex operators
+  with multiple parameters.
+* :mod:`pycaputo.differentiation` no longer exports all the underlying methods.
+  It is not required to do e.g. ``from pycaputo.differentiation.caputo import L1``.
+* All the methods in :mod:`pycaputo.differentiation` have been renamed without the
+  derivative type, e.g ``CaputoL1Method`` becomes simply ``L1``.
+* The methods in :mod:`pycaputo.differentiation` no longer provide an order. This
+  was not well-defined, since e.g. the L1 method has different orders depending
+  on the smoothness of the operand.
+* The :mod:`pycaputo.quadrature` module went through similar changes to the
+  differentiation one.
+* The :mod:`pycaputo.fode.caputo` module went through similar changes to the
+  differentiation and quadrature ones.
+
 pycaputo 0.5.0 (April 19, 2024)
 -------------------------------
 
 Features
 ^^^^^^^^
 
 * Implement an implicit adaptive L1 type method for Integrate-and-Fire models
   in :mod:`pycaputo.integrate_fire`.
 * Implement PIF, LIF, EIF and AdEx models explicitly. These can be used to model
   neurons using fractional dynamics.
 
 Maintenance
 ^^^^^^^^^^^
 
-* Use [uv](https://github.com/astral-sh/uv) to handled pinning dependencies.
-* Use [hatchling](https://hatch.pypa.io) as the build backend instead of ``setuptools``.
-* Start using [pytest-benchmark](https://pytest-benchmark.readthedocs.io) to
+* Use `uv <https://github.com/astral-sh/uv>`__ to handled pinning dependencies.
+* Use `hatchling <https://hatch.pypa.io>`__ as the build backend instead of ``setuptools``.
+* Start using `pytest-benchmark <https://pytest-benchmark.readthedocs.io>`__ to
   benchmark the code. This still needs a lot of work.
 
 pycaputo 0.4.0 (February 6, 2024)
 ---------------------------------
 
 Features
 ^^^^^^^^
@@ -92,31 +129,31 @@
 ^^^^^^^^
 
 * Added an example with the fractional Lorenz system (:ghpr:`13`).
 * Add a guess for the number of corrector iterations
   for :class:`~pycaputo.fode.caputo.PECE` from [Garrappa2010]_.
 * Added a modified PECE method from [Garrappa2010]_ in the form of
   :class:`~pycaputo.fode.caputo.ModifiedPECE`.
-* Implement :class:`~pycaputo.quadrature.RiemannLiouvilleSimpsonMethod`, a
+* Implement :class:`~pycaputo.quadrature.riemann_liouville.Simpson`, a
   standard 3rd order method.
-* Implement :class:`~pycaputo.quadrature.RiemannLiouvilleCubicHermiteMethod`, a
+* Implement :class:`~pycaputo.quadrature.riemann_liouville.CubicHermite`, a
   standard 4th order method.
 * Implement differentiation methods for the Riemann-Liouville derivatives based
   on the Caputo derivative in
-  :class:`~pycaputo.differentiation.RiemannLiouvilleFromCaputoDerivativeMethod`.
+  :class:`~pycaputo.differentiation.riemann_liouville.RiemannLiouvilleFromCaputoDerivativeMethod`.
 * Support different fractional orders for FODE systems in
   :class:`~pycaputo.fode.caputo.ForwardEuler`,
   :class:`~pycaputo.fode.caputo.WeightedEuler` and others.
 * Add approximation for the Lipschitz constant (:ghpr:`18`).
 * Add a (rather slow) wrapper to compute a fractional gradient (:ghpr:`35`).
 
 Fixes
 ^^^^^
 
-* Fix :class:`~pycaputo.quadrature.RiemannLiouvilleTrapezoidalMethod` on
+* Fix :class:`~pycaputo.quadrature.riemann_liouville.Trapezoidal` on
   uniform grids (:ghissue:`3`).
 * Fix Jacobian construction for :class:`~pycaputo.fode.caputo.WeightedEuler`
   which gave incorrect results for systems of equations (:ghissue:`11`).
 * Add dark variants of plots to the documentation for nicer results.
 * Promoto history management to :mod:`pycaputo.history`.
 
 pycaputo 0.1.0 (June 12, 2023)
```

### Comparing `pycaputo-0.5.0/docs/conf.py` & `pycaputo-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/differentiation.rst` & `pycaputo-0.6.0/docs/differentiation.rst`

 * *Files 15% similar despite different names*

```diff
@@ -4,54 +4,66 @@
 ===============
 
 Computing the derivative of a function can be done in two ways. The recommended
 method (with included magic) is calling :func:`pycaputo.diff` as
 
 .. code:: python
 
-   df = diff(f, p, alpha)
+    df = diff(f, p, alpha)
 
 which will automatically select an appropriate method to use given the point set
-``p`` and the order ``alpha``. To manually select a method use e.g. the
-``method="CaputoL1Method"`` keyword. The lower level function call is given by
-:func:`pycaputo.differentiation.diff` which can be used as
+``p`` and the order ``alpha`` (see also
+:func:`pycaputo.differentiation.guess_method_for_order`). To manually call a
+specific method, use :func:`pycaputo.differentiation.diff` instead as
 
 .. code:: python
 
-   d = CaputoDerivative(order=alpha, side=Side.Left)
-   m = CaputoL1Method(d)
-   df = diff(m, f, p)
+    from pycaputo.differentiation import diff
+    from pycaputo.differentiation.caputo import L2C
+
+    m = L2C(alpha)
+    df = diff(m, f, p)
 
 This requires more setup, but gives more control over the method used to
 approximate the derivative. The :func:`pycaputo.differentiation.diff` method
 is based on the :func:`~functools.singledispatch` mechanism and can be easily
 extended to support additional methods.
 
 Example
 -------
 
 We give here the skeleton for implementing a new custom
 :class:`~pycaputo.differentiation.DerivativeMethod`.
 First, all subclasses must be a :func:`~dataclasses.dataclass` as
 
 .. literalinclude:: ../examples/example-custom-diff.py
-    :lines: 14-27
+    :lines: 14-24
     :language: python
     :linenos:
 
 Then, we can implement the :func:`~pycaputo.differentiation.diff` method by
 registering it with the :func:`~functools.singledispatch` mechanism as
 
 .. literalinclude:: ../examples/example-custom-diff.py
-    :lines: 30-37
+    :lines: 27-34
     :language: python
     :linenos:
 
 The complete example can be found in
 :download:`examples/example-custom-diff.py <../examples/example-custom-diff.py>`.
 
 API Reference
 -------------
 
 .. autofunction:: pycaputo.diff
 
 .. automodule:: pycaputo.differentiation
+
+Caputo Derivative
+^^^^^^^^^^^^^^^^^
+
+.. automodule:: pycaputo.differentiation.caputo
+
+Riemann-Liouville Derivative
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. automodule:: pycaputo.differentiation.riemann_liouville
```

### Comparing `pycaputo-0.5.0/docs/history.rst` & `pycaputo-0.6.0/docs/history.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/index.rst` & `pycaputo-0.6.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 pycaputo documentation
 ======================
 
 .. toctree::
-    :maxdepth: 2
+    :maxdepth: 1
     :hidden:
+    :caption: Getting started
 
     tutorials
+    changelog
+    literature
+
+.. toctree::
+    :maxdepth: 2
+    :hidden:
+    :caption: API Reference
+
     operator
     quadrature
     differentiation
     history
     controllers
     timestepping
     fode
     integrate_fire
     misc
-    references
-    changelog
 
 .. warning::
 
    This package is currently in development and very experimental (the API
    can and will change frequently for the foreseeable future). For more mature
    libraries see `differint <https://github.com/differint/differint>`__ in
    Python or `FractionalDiffEq.jl <https://github.com/SciFracX/FractionalDiffEq.jl>`__
    in Julia.
 
 This package provides tools to (numerically) compute fractional order
 derivatives and integrals. It offers functionality to (non-exhaustive)
 
 * Evaluate Caputo fractional-order derivatives of real orders.
 * Evaluate Riemann-Liouville fractional-order integrals of arbitrary real orders.
-* Solve single-term fractional-order ordinary differential equations.
+* Solve single-term systems of fractional-order ordinary differential equation.
 * Easily extend this functionality with new numerical methods.
 
 At the moment, performance is not an important focus, but fractional-order
 operators are generally more computationally intensive than their integer-order
 counterparts. Once a solid framework is worked out, more care will be given to
 this aspect as well.
```

### Comparing `pycaputo-0.5.0/docs/integrate_fire.rst` & `pycaputo-0.6.0/docs/integrate_fire.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/misc.rst` & `pycaputo-0.6.0/docs/misc.rst`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 .. automodule:: pycaputo.grid
 
 Special Functions
 -----------------
 
 .. automodule:: pycaputo.mittagleffler
 
+Lagrange Polynomials
+--------------------
+
+.. automodule:: pycaputo.lagrange
+
 Jacobi Polynomials
 ------------------
 
 .. automodule:: pycaputo.jacobi
 
-
 Finite Difference Approximations
 --------------------------------
 
 .. automodule:: pycaputo.finite_difference
 
 Interpolation
 -------------
@@ -50,8 +54,10 @@
 Misc
 ----
 
 .. class:: pycaputo.utils.P
 
     A generic invarint :class:`typing.ParamSpec`.
 
+    alias of ParamSpec('P')
+
 .. automodule:: pycaputo.utils
```

### Comparing `pycaputo-0.5.0/docs/references.rst` & `pycaputo-0.6.0/docs/literature.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-References
+Literature
 ==========
 
 .. [Lubich1986] C. Lubich,
     *Discretized Fractional Calculus*,
     SIAM Journal on Mathematical Analysis, Vol. 17, pp. 704--719, 1986,
     `DOI <https://doi.org/10.1137/0517050>`__.
 
@@ -84,7 +84,12 @@
     Journal of Computational Science, Vol. 47, pp. 101220--101220, 2020,
     `DOI <https://doi.org/10.1016/j.jocs.2020.101220>`__.
 
 .. [Naud2008] R. Naud, N. Marcille, C. Clopath, W. Gerstner,
     *Firing Patterns in the Adaptive Exponential Integrate-and-Fire Model*,
     Biological Cybernetics, Vol. 99, pp. 335--347, 2008,
     `DOI <https://doi.org/10.1007/s00422-008-0264-7>`__.
+
+.. [Cardone2021] A. Cardone, D. Conte, B. Paternoster,
+    *A MATLAB Implementation of Spline Collocation Methods for Fractional Differential Equations*,
+    Computational Science and Its Applications – ICCSA 2021, pp. 387--401, 2021,
+    `DOI <https://doi.org/10.1007/978-3-030-86653-2_29>`__.
```

### Comparing `pycaputo-0.5.0/docs/tutorials.rst` & `pycaputo-0.6.0/docs/tutorials.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,48 +15,50 @@
 
 where :math:`n = \lceil \alpha \rceil` is the smallest integer larger than
 :math:`\alpha`. In this example, we take :math:`\alpha \in (0, 1)`, so :math:`n = 1`,
 and use a simple test function
 
 .. math::
 
-    f(x) = \left(\frac{1}{2} + x\right)^4
+    f(x) = \left(\frac{1}{2} - x\right)^4
 
 and its Caputo fractional order derivative given by
 
 .. math::
 
     D^\alpha_C[f](x) =
         - \frac{x^{1 - \alpha}}{2 \Gamma(2 - \alpha)}
         + \frac{3 x^{2 - \alpha}}{\Gamma(3 - \alpha)}
         - \frac{12 x^{3 - \alpha}}{\Gamma(4 - \alpha)}
         + \frac{24 x^{4 - \alpha}}{\Gamma(5 - \alpha)}.
 
 In code, we can write them as below
 
 .. literalinclude:: ../examples/caputo-derivative-l1.py
-    :lines: 16-26
+    :lines: 22-32
     :lineno-match:
     :language: python
 
 To estimate the derivative, we use the classical L1 method (see Chapter 4.1 in
 [Li2020]_ or Chapter 3 in [Karniadakis2019]_). The methods are set up as
 follows
 
 .. literalinclude:: ../examples/caputo-derivative-l1.py
-    :lines: 29-35
+    :lines: 35-38
     :lineno-match:
     :language: python
 
-These methods are described by the :class:`~pycaputo.derivatives.CaputoDerivative`
-and :class:`~pycaputo.differentiation.CaputoL1Method` classes.
-We can then set up a grid and evaluate the derivative at all points
+The method uses the :class:`~pycaputo.derivatives.CaputoDerivative` operator
+and the :class:`~pycaputo.differentiation.caputo.L1` discretization. See
+:mod:`pycaputo.differentiation.caputo` for other methods for discretizing the
+Caputo derivative. We can then set up a grid and evaluate the derivative at
+all points
 
 .. literalinclude:: ../examples/caputo-derivative-l1.py
-    :lines: 37-40
+    :lines: 40-46
     :lineno-match:
     :language: python
 
 For the chosen number of points, this gives an error of about :math:`10^{-3}`.
 The resulting approximation can be see below
 
 .. image:: caputo-derivative-l1-light.svg
@@ -91,39 +93,39 @@
 
 where we take :math:`(a, \mu) = (1, 4)`, an order :math:`\alpha = 0.8`, and
 initial conditions :math:`(x_0, y_0) = (1, 2)`. For these parameters, the
 system has a stable limit cycle, which we can observe (see [Garrappa2015b]_).
 The right-hand side for this system can be implemented as
 
 .. literalinclude:: ../examples/brusselator-predictor-corrector.py
-    :lines: 16-20
+    :lines: 22-26
     :lineno-match:
     :language: python
 
 We can now start setting up our numerical solver based on the standard
 Predictor-Corrector method (PECE) described in [Diethelm2002]_ and implemented
 by :class:`~pycaputo.fode.caputo.PECE`. The solver is then set up as
 
 .. literalinclude:: ../examples/brusselator-predictor-corrector.py
-    :lines: 28-42
+    :lines: 34-48
     :lineno-match:
     :language: python
 
 We can see here that we have chosen to use a solver for the Caputo derivative
 an order :math:`\alpha`. The solver will use a fixed time step of :math:`10^{-2}`
 on the interval :math:`[0, 50]` to properly observe the limit cycle behavior. For
 Predictor-Corrector schemes, the corrector step can be repeated multiple times,
 but here we choose ``corrector_iterations=1`` to only use a single iteration.
 
 Now that the solver is set up, we can simply evolve the equation time step by
 time step to get all the solutions. This will use the :func:`pycaputo.stepping.evolve`
 iterator as follows
 
 .. literalinclude:: ../examples/brusselator-predictor-corrector.py
-    :lines: 44-61
+    :lines: 50-67
     :lineno-match:
     :language: python
 
 The solution as a function of time can be seen below.
 
 .. image:: brusselator-predictor-corrector-light.svg
     :class: only-light
@@ -170,59 +172,59 @@
 
 where :math:`\mu = 4`, :math:`\alpha = 0.8` and the initial condition is taken
 to be :math:`(x_0, y_0) = (1, 0)`. As we will see, this is close to a limit
 cycle of the oscillator (see e.g. [Jannelli2020]_). The right-hand side for this
 system is implemented as
 
 .. literalinclude:: ../examples/van-der-pol-adaptive-pece.py
-    :lines: 21-29
+    :lines: 32-40
     :lineno-match:
     :language: python
 
 We can now start setting up our numerical solver based on the standard
 Predictor-Corrector method (PECE) implemented in
 :class:`~pycaputo.fode.caputo.PECE`. The time adaptation is based on the
 results from [Jannelli2020]_ and implemented in
 :class:`~pycaputo.controller.JannelliIntegralController`. The controller is
 set up as follows
 
 .. literalinclude:: ../examples/van-der-pol-adaptive-pece.py
-    :lines: 37-48
+    :lines: 48-59
     :lineno-match:
     :language: python
 
 We can see here that we have chosen a time interval of :math:`[0, 4]` to see
 the start of the limit cycle. We have also used other parameters better described
 in [Jannelli2020]. Briefly, ``qmin`` and ``qmax`` are used to decrease or
 increase the time step by a fixed value, while ``chimin`` and ``chimax`` are
 used to normalize the Jannelli error estimator. Then, we can set up the solver
 itself
 
 .. literalinclude:: ../examples/van-der-pol-adaptive-pece.py
-    :lines: 50-59
+    :lines: 61-70
     :lineno-match:
     :language: python
 
 For the solver we set the desired order ``alpha`` and choose two corrector
 iterations, to be sure that the second-order accuracy is achieved. For an
 adaptive scheme, it is important to also get an estimate for the initial time
 step. This can be done using
 
 .. literalinclude:: ../examples/van-der-pol-adaptive-pece.py
-    :lines: 61-68
+    :lines: 72-79
     :lineno-match:
     :language: python
 
 Having set everything up, we can evolve our equation and gather any relevant data.
 For the adaptive case, we are interested also in showing the behavior of the
 error estimate and the time step in time. Here, we will only gather this information
 for accepted steps.
 
 .. literalinclude:: ../examples/van-der-pol-adaptive-pece.py
-    :lines: 87-98
+    :lines: 98-109
     :lineno-match:
     :language: python
 
 We can now look at the solution and the corresponding time steps below.
 
 .. image:: van-der-pol-adaptive-pece-solution-light.svg
     :class: only-light
```

### Comparing `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-dark.svg` & `pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-eest-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-light.svg` & `pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-eest-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-dark.svg` & `pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-solution-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-light.svg` & `pycaputo-0.6.0/docs/van-der-pol-adaptive-pece-solution-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/docs/benchmarks/Linux-CPython-3.11-64bit/0001_561ba4947e7fa72377b82f411a1f0eb91929763c_20240408_123818.json` & `pycaputo-0.6.0/docs/benchmarks/Linux-CPython-3.11-64bit/0001_561ba4947e7fa72377b82f411a1f0eb91929763c_20240408_123818.json`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/brusselator-predictor-corrector.py` & `pycaputo-0.6.0/examples/brusselator-predictor-corrector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
+r"""Solve the fractional Brusselator model for a standard choice of parameters
+where it exhibits a limit cycle.
+
+The example uses the PECE method with a fixed step size.
+"""
+
 from functools import partial
 
 import numpy as np
 
 from pycaputo.logging import get_logger
 from pycaputo.utils import Array
```

### Comparing `pycaputo-0.5.0/examples/caputo-derivative-l1.py` & `pycaputo-0.6.0/examples/caputo-derivative-l1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
+"""Compute the fractional Caputo derivative of a function using the L1
+method. This is a simple example showcasing how the API can be used.
+
+Other methods are available at :mod:`pycaputo.differentiation`.
+"""
+
 import math
 
 import numpy as np
 
 from pycaputo.logging import get_logger
 from pycaputo.utils import Array
 
@@ -22,28 +28,28 @@
         -0.5 * x ** (1 - alpha) / math.gamma(2 - alpha)
         + 3 * x ** (2 - alpha) / math.gamma(3 - alpha)
         - 12 * x ** (3 - alpha) / math.gamma(4 - alpha)
         + 24 * x ** (4 - alpha) / math.gamma(5 - alpha)
     )
 
 
-from pycaputo.derivatives import CaputoDerivative, Side
-
-d = CaputoDerivative(order=0.9, side=Side.Left)
+from pycaputo.differentiation.caputo import L1
 
-from pycaputo.differentiation import CaputoL1Method, diff
-
-method = CaputoL1Method(d)
+alpha = 0.9
+method = L1(alpha=alpha)
 
 from pycaputo.grid import make_uniform_points
 
 p = make_uniform_points(256, a=0.0, b=1.0)
+
+from pycaputo.differentiation import diff
+
 df_num = diff(method, f, p)
 
-df_ref = df(p.x, d.order)
+df_ref = df(p.x, alpha)
 logger.info(
     "Relative error: %.12e",
     np.linalg.norm(df_num[1:] - df_ref[1:]) / np.linalg.norm(df_ref[1:]),
 )
 
 
 # }}}
```

### Comparing `pycaputo-0.5.0/examples/example-custom-diff.py` & `pycaputo-0.6.0/examples/example-custom-diff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
+"""This example showcases how to create a new differentiation method.
+
+The definition is given by registering a new method using ``diff.register``.
+"""
+
 from dataclasses import dataclass
 
 import numpy as np
 
-from pycaputo.derivatives import RiemannLiouvilleDerivative
-from pycaputo.differentiation import DerivativeMethod, diff, make_method_from_name
+from pycaputo.derivatives import RiemannLiouvilleDerivative, Side
+from pycaputo.differentiation import DerivativeMethod, diff
 from pycaputo.grid import Points
 from pycaputo.utils import Array, ArrayOrScalarFunction
 
 
 @dataclass(frozen=True)
 class RiemannLiouvilleDerivativeMethod(DerivativeMethod):
-    d: RiemannLiouvilleDerivative
+    alpha: float
 
     @property
     def name(self) -> str:
         return "RLdiff"
 
     @property
-    def order(self) -> float:
-        return 1.0
-
-    def supports(self, alpha: float) -> bool:
-        return 0.0 < self.d.order < 1.0
+    def d(self) -> RiemannLiouvilleDerivative:
+        return RiemannLiouvilleDerivative(self.alpha, side=Side.Left)
 
 
 @diff.register(RiemannLiouvilleDerivativeMethod)
 def _diff_rl(
     m: RiemannLiouvilleDerivativeMethod,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     fx = f(p.x) if callable(f) else f
     return np.zeros_like(fx)
 
 
-m = make_method_from_name("RiemannLiouvilleDerivativeMethod", 0.5)
+m = RiemannLiouvilleDerivativeMethod(alpha=0.9)
```

### Comparing `pycaputo-0.5.0/examples/integrate-and-fire-ad-ex.py` & `pycaputo-0.6.0/examples/integrate-and-fire-ad-ex.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/integrate-and-fire-eif.py` & `pycaputo-0.6.0/examples/integrate-and-fire-eif.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/integrate-and-fire-lif.py` & `pycaputo-0.6.0/examples/integrate-and-fire-lif.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/integrate-and-fire-pif.py` & `pycaputo-0.6.0/examples/integrate-and-fire-pif.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/lorenz-weighted-euler.py` & `pycaputo-0.6.0/examples/lorenz-weighted-euler.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/examples/van-der-pol-adaptive-pece.py` & `pycaputo-0.6.0/examples/van-der-pol-adaptive-pece.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
-# NOTE: the parameters and general setup for this are taken from Jannelli2020
-# NOTE: the figures should be compared to Figure 6 and surrounding text
+"""
+This attempts to reproduce Figure 6 from [Jannelli2020]_ using the fractional
+van der Pol oscillator. The setup is not exactly the same as the error indicator
+is changed.
+
+This example uses the PECE method to solve the equation, while [Jannelli2020]_
+uses the implicit trapezoidal PI method.
+
+.. [Jannelli2020] A. Jannelli,
+    *A Novel Adaptive Procedure for Solving Fractional Differential Equations*,
+    Journal of Computational Science, Vol. 47, pp. 101220--101220, 2020,
+    `DOI <https://doi.org/10.1016/j.jocs.2020.101220>`__.
+"""
 
 from __future__ import annotations
 
 import numpy as np
 
 from pycaputo.controller import estimate_initial_time_step, make_jannelli_controller
 from pycaputo.fode import caputo
```

### Comparing `pycaputo-0.5.0/scripts/benchmark-boxplot.py` & `pycaputo-0.6.0/scripts/benchmark-boxplot.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/scripts/generate-doc-figures.py` & `pycaputo-0.6.0/scripts/generate-doc-figures.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/benchmark.py` & `pycaputo-0.6.0/src/pycaputo/benchmark.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/controller.py` & `pycaputo-0.6.0/src/pycaputo/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from functools import singledispatch
+from functools import cached_property, singledispatch
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
 from pycaputo.utils import Array, StateFunction, StateFunctionT
 
 if TYPE_CHECKING:
@@ -69,81 +69,14 @@
         tfinal = tstart + nsteps * dt
     else:
         raise ValueError("Must provide either 'tfinal' or 'nsteps' or both")
 
     return dt, tfinal, nsteps
 
 
-def make_fixed_controller(
-    dt: float,
-    tstart: float = 0.0,
-    tfinal: float | None = None,
-    nsteps: int | None = None,
-) -> FixedController:
-    """Create a controller with a fixed time step.
-
-    This ensures that the following relation holds for all given values
-
-    .. code:: python
-
-        tfinal = tstart + nsteps * dt
-
-    This is achieved by small modifications to either *nsteps*, *dt* or *tfinal*.
-    If both *nsteps* and *tfinal* are given, then the smallest of
-    ``tstart + nsteps * dt`` and ``tfinal`` is taken as the final time and the
-    values are recalculated.
-
-    :arg dt: desired time step (chosen time step may be slightly smaller).
-    :arg tstart: start of the time span.
-    :arg tfinal: end of the time span.
-    :arg nsteps: number of time steps in the span.
-    """
-    if tfinal is None and nsteps is None:
-        raise ValueError("Must provide either 'tfinal' or 'nsteps' or both")
-
-    dt, tfinal, nsteps = _normalize_time_span_triple(dt, tstart, tfinal, nsteps)
-    return FixedController(tstart=tstart, tfinal=tfinal, nsteps=nsteps, dt=dt)
-
-
-def make_graded_controller(
-    dt: float | None = None,
-    tstart: float = 0.0,
-    tfinal: float | None = None,
-    nsteps: int | None = None,
-    *,
-    alpha: float | None = None,
-    r: float | None = None,
-) -> GradedController:
-    """Create a controller with a graded time step (see :func:`make_fixed_controller`).
-
-    :arg alpha: order of the fractional operator. The order is used to choose an
-        optimal grading *r* according to [Stynes2017]_.
-    :arg r: the degree of grading in the time step (see :class:`GradedController`).
-    """
-    if tfinal is None and nsteps is None:
-        raise ValueError("Must provide either 'tfinal' or 'nsteps' or both")
-
-    if r is None and alpha is None:
-        raise ValueError("Must provide either 'alpha' or 'r' or both to define grading")
-
-    if r is None:
-        assert alpha is not None
-        if 0.0 < alpha <= 1.0:
-            r = (2 - alpha) / alpha
-        else:
-            raise ValueError("Grading estimate is only valid for 'alpha' in (0, 1)")
-
-    if dt is None:
-        if tfinal is None or nsteps is None:
-            raise ValueError("Must provide both 'tfinal' and 'nsteps' with no 'dt'")
-    else:
-        dt, tfinal, nsteps = _normalize_time_span_triple(dt, tstart, tfinal, nsteps)
-    return GradedController(tstart=tstart, tfinal=tfinal, nsteps=nsteps, r=r)
-
-
 def estimate_initial_time_step(
     t0: float,
     y0: Array,
     f: StateFunction,
     alpha: float,
     *,
     trunc: float | None = None,
@@ -338,22 +271,57 @@
 
 # {{{ non-adaptive controller
 
 
 # {{{ FixedController
 
 
+def make_fixed_controller(
+    dt: float,
+    tstart: float = 0.0,
+    tfinal: float | None = None,
+    nsteps: int | None = None,
+) -> FixedController:
+    """Create a controller with a fixed time step.
+
+    This ensures that the following relation holds for all given values
+
+    .. code:: python
+
+        tfinal = tstart + nsteps * dt
+
+    This is achieved by small modifications to either *nsteps*, *dt* or *tfinal*.
+    If both *nsteps* and *tfinal* are given, then the smallest of
+    ``tstart + nsteps * dt`` and ``tfinal`` is taken as the final time and the
+    values are recalculated.
+
+    :arg dt: desired time step (chosen time step may be slightly smaller).
+    :arg tstart: start of the time span.
+    :arg tfinal: end of the time span.
+    :arg nsteps: number of time steps in the span.
+    """
+    if tfinal is None and nsteps is None:
+        raise ValueError("Must provide either 'tfinal' or 'nsteps' or both")
+
+    dt, tfinal, nsteps = _normalize_time_span_triple(dt, tstart, tfinal, nsteps)
+    return FixedController(tstart=tstart, tfinal=tfinal, nsteps=nsteps, dt=dt)
+
+
 @dataclass(frozen=True)
 class FixedController(Controller):
     """A fake controller with a fixed time step."""
 
     dt: float
     """Fixed time step used by the controller."""
 
     @property
+    def dtinit(self) -> float:
+        return self.dt
+
+    @property
     def is_adaptive(self) -> bool:
         return False
 
 
 @evaluate_error_estimate.register(FixedController)
 def _evaluate_error_estimate_fixed(
     c: FixedController,
@@ -392,14 +360,50 @@
 
 # }}}
 
 
 # {{{ GradedController
 
 
+def make_graded_controller(
+    dt: float | None = None,
+    tstart: float = 0.0,
+    tfinal: float | None = None,
+    nsteps: int | None = None,
+    *,
+    alpha: float | None = None,
+    r: float | None = None,
+) -> GradedController:
+    """Create a controller with a graded time step (see :func:`make_fixed_controller`).
+
+    :arg alpha: order of the fractional operator. The order is used to choose an
+        optimal grading *r* according to [Stynes2017]_.
+    :arg r: the degree of grading in the time step (see :class:`GradedController`).
+    """
+    if tfinal is None and nsteps is None:
+        raise ValueError("Must provide either 'tfinal' or 'nsteps' or both")
+
+    if r is None and alpha is None:
+        raise ValueError("Must provide either 'alpha' or 'r' or both to define grading")
+
+    if r is None:
+        assert alpha is not None
+        if 0.0 < alpha <= 1.0:
+            r = (2 - alpha) / alpha
+        else:
+            raise ValueError("Grading estimate is only valid for 'alpha' in (0, 1)")
+
+    if dt is None:
+        if tfinal is None or nsteps is None:
+            raise ValueError("Must provide both 'tfinal' and 'nsteps' with no 'dt'")
+    else:
+        dt, tfinal, nsteps = _normalize_time_span_triple(dt, tstart, tfinal, nsteps)
+    return GradedController(tstart=tstart, tfinal=tfinal, nsteps=nsteps, r=r)
+
+
 @dataclass(frozen=True)
 class GradedController(Controller):
     r"""A :class:`Controller` with a variable graded time step.
 
     This graded grid of time steps is described in [Garrappa2015b]_. It
     essentially takes the form
 
@@ -432,14 +436,23 @@
 
             super().__post_init__()
 
     @property
     def is_adaptive(self) -> bool:
         return False
 
+    @property
+    def dtinit(self) -> float:
+        if self.tfinal is None or self.nsteps is None:
+            raise AttributeError(
+                f"type object '{type(self).__name__}' has no attribute 'dt'"
+            )
+
+        return (self.tfinal - self.tstart) / (self.nsteps - 1.0)
+
 
 @evaluate_error_estimate.register(GradedController)
 def _evaluate_error_estimate_graded(
     c: GradedController,
     m: FractionalDifferentialEquationMethod[StateFunctionT],
     trunc: Array,
     y: Array,
@@ -928,7 +941,118 @@
         eps = 5.0 * np.finfo(m.y0[0].dtype).eps
         dt = min(dt, c.tfinal - state["t"]) + eps
 
     return dt
 
 
 # }}}
+
+
+# {{{ random controller
+
+
+@dataclass(frozen=True)
+class RandomController(Controller):
+    r"""A time step controller with random time steps.
+
+    This controller is meant for testing and should not be used otherwise. The
+    time steps are uniformly sampled in :math:`[\Delta t_{\text{min}},
+    \Delta t_{\text{max}}]`.
+    """
+
+    dtmin: float
+    """A minimum allowable time step."""
+    dtmax: float
+    """A maximum allowable time step."""
+    rng: np.random.Generator
+    """A random number generator for the time steps."""
+
+    @cached_property
+    def times(self) -> Array:
+        assert self.tfinal is not None
+
+        n = int((self.tfinal - self.tstart) / self.dtmin) + 1
+        dt = self.rng.uniform(self.dtmin, self.dtmax, size=n)
+        ts = self.tstart + np.cumsum(np.hstack([[0.0], dt]))
+
+        ts = ts[ts < self.tfinal]
+        if abs(ts[-1] - self.tfinal) > 1.0e-14:
+            ts = np.hstack([ts, [self.tfinal]])
+
+        return np.array(ts)
+
+    @cached_property
+    def timesteps(self) -> Array:
+        return np.diff(self.times)
+
+    @property
+    def dtinit(self) -> float:
+        return float(self.timesteps[0])
+
+
+def make_random_controller(
+    tstart: float = 0.0,
+    tfinal: float | None = None,
+    *,
+    dtmin: float = 1.0e-6,
+    dtmax: float = 1.0e-2,
+    rng: np.random.Generator | None = None,
+) -> RandomController:
+    """Construct a :class:`RandomController`."""
+    if tfinal is None:
+        raise ValueError(f"Must provide 'tfinal': value '{tfinal}'")
+
+    if rng is None:
+        rng = np.random.default_rng()
+
+    return RandomController(
+        tstart=tstart,
+        tfinal=tfinal,
+        nsteps=None,
+        dtmin=dtmin,
+        dtmax=dtmax,
+        rng=rng,
+    )
+
+
+@evaluate_error_estimate.register(RandomController)
+def _evaluate_error_estimate_random(
+    c: RandomController,
+    m: FractionalDifferentialEquationMethod[StateFunctionT],
+    trunc: Array,
+    y: Array,
+    yprev: Array,
+) -> float:
+    return 0.0
+
+
+@evaluate_timestep_factor.register(RandomController)
+def _evaluate_timestep_factor_random(
+    c: RandomController,
+    m: FractionalDifferentialEquationMethod[StateFunctionT],
+    eest: float,
+) -> float:
+    return 1.0
+
+
+@evaluate_timestep_accept.register(RandomController)
+def _evaluate_timestep_accept_random(
+    c: RandomController,
+    m: FractionalDifferentialEquationMethod[StateFunctionT],
+    q: float,
+    dtprev: float,
+    state: dict[str, Any],
+) -> float:
+    n = state["n"]
+    if n >= c.timesteps.size - 1:
+        # NOTE: this time step is not going to get used
+        return 0.0
+
+    dt = c.timesteps[n + 1]
+    if c.tfinal is not None:
+        eps = 5.0 * np.finfo(m.y0[0].dtype).eps
+        dt = min(dt, c.tfinal - state["t"]) + eps
+
+    return float(dt)
+
+
+# }}}
```

### Comparing `pycaputo-0.5.0/src/pycaputo/events.py` & `pycaputo-0.6.0/src/pycaputo/events.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/finite_difference.py` & `pycaputo-0.6.0/src/pycaputo/finite_difference.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/generating_functions.py` & `pycaputo-0.6.0/src/pycaputo/generating_functions.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/grid.py` & `pycaputo-0.6.0/src/pycaputo/grid.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/history.py` & `pycaputo-0.6.0/src/pycaputo/history.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/implicit.py` & `pycaputo-0.6.0/src/pycaputo/implicit.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/interpolation.py` & `pycaputo-0.6.0/src/pycaputo/interpolation.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/jacobi.py` & `pycaputo-0.6.0/src/pycaputo/jacobi.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/lipschitz.py` & `pycaputo-0.6.0/src/pycaputo/lipschitz.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/logging.py` & `pycaputo-0.6.0/src/pycaputo/logging.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/stepping.py` & `pycaputo-0.6.0/src/pycaputo/stepping.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/utils.py` & `pycaputo-0.6.0/src/pycaputo/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,20 @@
 from pycaputo.logging import get_logger
 
 logger = get_logger(__name__)
 
 
 # {{{ typing
 
+P = ParamSpec("P")
+
 T = TypeVar("T")
 """A generic invariant :class:`typing.TypeVar`."""
 R = TypeVar("R")
 """A generic invariant :class:`typing.TypeVar`."""
-P = ParamSpec("P")
-"""A generic invariant :class:`typing.ParamSpec`."""
-
 PathLike = Union[pathlib.Path, str]
 """A union of types supported as paths."""
 
 if TYPE_CHECKING:
     Array = np.ndarray[Any, Any]
     Scalar = Union[np.generic, Array]
 else:
@@ -103,31 +102,14 @@
     def __call__(self, t: float, y: Array, /) -> float:
         """
         :arg t: time at which to evaluate the function.
         :arg y: state vector value at which to evaluate the function.
         """
 
 
-class CallbackFunction(Protocol):
-    """A generic callback for evolution equations that can be used to modify
-    the state.
-
-    .. automethod:: __call__
-    """
-
-    def __call__(self, t: float, y: Array, /) -> bool:
-        """
-        :arg t: time at which to evaluate the function.
-        :arg y: state vector value at which to evaluate the function.
-
-        :returns: if *True*, hint to the algorithm that the evolution should be
-            stopped.
-        """
-
-
 @runtime_checkable
 class DifferentiableScalarFunction(Protocol):
     """A :class:`ScalarFunction` that can also compute its integer order derivatives.
 
     By default no derivatives are implemented, so subclasses can handle any such
     cases.
     """
@@ -299,22 +281,24 @@
         lines.append((f"{h[i]:.3e}", *values))
 
     lines.append((
         "Overall",
         *flatten([("", f"{eoc.estimated_order:.3f}") for eoc in eocs]),
     ))
 
-    expected = flatten([
-        ("", f"{eoc.order:.3f}") for eoc in eocs if eoc.order is not None
-    ])
-    if expected:
+    if any(eoc.order is not None for eoc in eocs):
+        expected = flatten([
+            (("", f"{eoc.order:.3f}") if eoc.order is not None else ("", "--"))
+            for eoc in eocs
+        ])
+
         lines.append(("Expected", *expected))
 
     widths = [max(len(line[i]) for line in lines) for i in range(ncolumns)]
-    formats = ["{:%s}" % w for w in widths]
+    formats = ["{:%s}" % w for w in widths]  # noqa: UP031
 
     return "\n".join([
         " | ".join(fmt.format(value) for fmt, value in zip(formats, line))
         for line in lines
     ])
 
 
@@ -477,15 +461,15 @@
         "figure": {
             "figsize": (8, 8),
             "dpi": 300,
             "constrained_layout.use": True,
         },
         "savefig": {"format": savefig_format},
         "text": {"usetex": use_tex},
-        "legend": {"fontsize": 32},
+        "legend": {"fontsize": 20},
         "lines": {"linewidth": 2, "markersize": 10},
         "axes": {
             "labelsize": 28,
             "titlesize": 28,
             "grid": True,
             "grid.axis": "both",
             "grid.which": "both",
@@ -679,14 +663,15 @@
 
     @property
     def t_cpu(self) -> float:
         """Total CPU time, obtained from ``t_proc / t_wall``."""
         return self.t_proc / self.t_wall
 
     def __enter__(self) -> BlockTimer:
+        self.t_wall = self.t_proc = 0.0
         self.t_wall_start = time.perf_counter()
         self.t_proc_start = time.process_time()
 
         return self
 
     def __exit__(
         self,
@@ -696,14 +681,18 @@
     ) -> None:
         self.t_wall = time.perf_counter() - self.t_wall_start
         self.t_proc = time.process_time() - self.t_proc_start
 
     def __str__(self) -> str:
         return f"{self.name}: {self.t_wall:.3e}s wall, {self.t_cpu:.3f}x cpu"
 
+    def pretty(self) -> str:
+        # NOTE: this matches how MATLAB shows the time from `toc`.
+        return f"[{self.name}] Elapsed time is {self.t_wall:.5f} seconds."
+
 
 # }}}
 
 
 # {{{ scipy wrappers
 
 
@@ -765,15 +754,18 @@
 
     new_wrapper = update_wrapper(wrapper, func)
     new_wrapper.clear_cached = clear_cached  # type: ignore[attr-defined]
 
     return new_wrapper
 
 
-def single_valued(iterable: Iterable[T], eq: Callable[[T, T], bool] | None = None) -> T:
+def single_valued(
+    iterable: Iterable[T],
+    eq: Callable[[T, T], bool] | None = None,
+) -> T:
     """Retrieve a single value from the *iterable*.
 
     This function will return the first value from the *iterable* and assert that
     all other values are equal to it in the sense of the *eq* predicate. Note
     that the check is not performed when optimizations are turned on (as it is
     an assert).
 
@@ -792,14 +784,43 @@
     except StopIteration:
         raise ValueError("Iterable is empty") from None
 
     assert all(eq(first, other) for other in iterable)
     return first
 
 
+def is_single_valued(
+    iterable: Iterable[T],
+    eq: Callable[[T, T], bool] | None = None,
+) -> bool:
+    """This is a boolean version of :func:`single_valued`.
+
+    The function will return *True* if all the elements in the iterable are equal,
+    in the sense of the *eq* predicate, and *False* otherwise. Note that, unlike
+    :func:`single_valued`, an empty iterable will return *True* to match the
+    behaviour of :func:`all`.
+
+    :arg eq: an equality predicate on the elements of *iterable*, defaulting to
+        :func:`operator.eq`.
+    """
+    if eq is None:
+        import operator
+
+        eq = operator.eq
+
+    iterable = iter(iterable)
+
+    try:
+        first = next(iterable)
+    except StopIteration:
+        return True
+
+    return all(eq(first, other) for other in iterable)
+
+
 # }}}
 
 
 # {{{ dataclass
 
 
 def dc_asdict(dc: DataclassInstance, *, init_only: bool = True) -> dict[str, Any]:
```

### Comparing `pycaputo-0.5.0/src/pycaputo/differentiation/base.py` & `pycaputo-0.6.0/src/pycaputo/differentiation/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,50 +12,32 @@
 from pycaputo.utils import Array, ArrayOrScalarFunction
 
 
 @dataclass(frozen=True)
 class DerivativeMethod(ABC):
     """A generic method used to evaluate a fractional derivative at a set of points."""
 
-    d: FractionalOperator
-
-    if __debug__:
-
-        def __post_init__(self) -> None:
-            if not self.supports(self.d.order):
-                raise ValueError(
-                    f"Method '{self.name}' does not support derivative order "
-                    f"'{self.d.order}'"
-                )
-
     @property
     def name(self) -> str:
-        """An identifier for the differentiation method."""
+        """An (non-unique) identifier for the differentiation method."""
         return type(self).__name__.replace("Method", "")
 
     @property
     @abstractmethod
-    def order(self) -> float:
-        """Expected order of convergence of the method."""
-
-    @abstractmethod
-    def supports(self, alpha: float) -> bool:
-        """
-        :returns: *True* if the method supports computing the fractional
-            order derivative of order *alpha* and *False* otherwise.
-        """
+    def d(self) -> FractionalOperator:
+        """The fractional operator that is being discretized by the method."""
 
 
 @singledispatch
 def diff(m: DerivativeMethod, f: ArrayOrScalarFunction, p: Points) -> Array:
-    """Evaluate the fractional derivative of *f* at *x*.
+    """Evaluate the fractional derivative of *f* at *p* using method *m*.
 
-    Note that not all numerical methods can evaluate the derivative at all
-    points in *x*. For example, the :class:`CaputoL1Method` cannot evaluate the
-    derivative at ``x[0]``.
+    This is a low-level function that should be implemented by methods. For
+    a higher-level function see :func:`pycaputo.diff`. Note that this function
+    evaluates the derivative at all points in *p*, not just at *p[-1]*.
 
     :arg m: method used to evaluate the derivative.
     :arg f: a simple function for which to evaluate the derivative.
     :arg p: an array of points at which to evaluate the derivative.
     """
     raise NotImplementedError(
         f"Cannot evaluate fractional derivative with method '{type(m).__name__}'"
```

### Comparing `pycaputo-0.5.0/src/pycaputo/differentiation/caputo.py` & `pycaputo-0.6.0/src/pycaputo/differentiation/caputo.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,68 +5,67 @@
 
 import math
 from dataclasses import dataclass
 from typing import Iterator
 
 import numpy as np
 
-from pycaputo.derivatives import CaputoDerivative
+from pycaputo.derivatives import CaputoDerivative, Side
 from pycaputo.grid import Points, UniformMidpoints, UniformPoints
 from pycaputo.logging import get_logger
 from pycaputo.utils import Array, ArrayOrScalarFunction
 
 from .base import DerivativeMethod, diff
 
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class CaputoDerivativeMethod(DerivativeMethod):
     """A method used to evaluate a :class:`~pycaputo.derivatives.CaputoDerivative`."""
 
-    d: CaputoDerivative
-    """A Caputo derivative to discretize."""
+    alpha: float
+    """Order of the Caputo derivative that is being discretized."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
-            super().__post_init__()
-            if not isinstance(self.d, CaputoDerivative):
-                raise TypeError(
-                    f"Expected a Caputo derivative: '{type(self.d).__name__}'"
-                )
+            if self.alpha < 0:
+                raise ValueError(f"Negative orders are not supported: {self.alpha}")
+
+    @property
+    def d(self) -> CaputoDerivative:
+        return CaputoDerivative(self.alpha, side=Side.Left)
 
 
-# {{{ Caputo L1 Method
+# {{{ L1
 
 
 @dataclass(frozen=True)
-class CaputoL1Method(CaputoDerivativeMethod):
+class L1(CaputoDerivativeMethod):
     r"""Implements the L1 method for the Caputo fractional derivative
     of order :math:`\alpha \in (0, 1)`.
 
     This method is defined in Section 4.1.1 (II) from [Li2020]_ for general
-    non-uniform grids. Note that it cannot compute the derivative at the
-    starting point, i.e. :math:`D_C^\alpha[f](a)` is undefined.
-
-    This method is of order :math:`\mathcal{O}(h^{2 - \alpha})` and supports
-    arbitrary grids.
+    non-uniform grids.
     """
 
-    @property
-    def order(self) -> float:
-        return 2 - self.d.order
+    if __debug__:
 
-    def supports(self, alpha: float) -> bool:
-        return 0 < alpha < 1
+        def __post_init__(self) -> None:
+            super().__post_init__()
+            if not 0 < self.alpha < 1:
+                raise ValueError(
+                    f"'{type(self).__name__}' only supports 0 < alpha < 1: {self.alpha}"
+                )
 
 
-def _weights_l1(m: CaputoL1Method, p: Points) -> Iterator[Array]:
+def _weights_l1(m: L1, p: Points) -> Iterator[Array]:
     x, dx = p.x, p.dx
-    alpha = m.d.order
+    alpha = m.alpha
     w0 = 1 / math.gamma(2 - alpha)
 
     # NOTE: weights given in [Li2020] Equation 4.20
     if isinstance(p, UniformPoints):
         w0 = w0 / p.dx[0] ** alpha
         k = np.arange(x.size - 1)
 
@@ -78,67 +77,78 @@
             w = (
                 (x[n] - x[:n]) ** (1 - alpha) - (x[n] - x[1 : n + 1]) ** (1 - alpha)
             ) / dx[:n]
 
             yield w0 * w
 
 
-@diff.register(CaputoL1Method)
-def _diff_l1method(m: CaputoL1Method, f: ArrayOrScalarFunction, p: Points) -> Array:
+@diff.register(L1)
+def _diff_l1_method(m: L1, f: ArrayOrScalarFunction, p: Points) -> Array:
     dfx = np.diff(f(p.x) if callable(f) else f)
 
     df = np.empty(p.x.shape, dtype=dfx.dtype)
     df[0] = np.nan
 
     for n, w in enumerate(_weights_l1(m, p)):
         df[n + 1] = np.sum(w * dfx[: n + 1])
 
     return df
 
 
+# }}}
+
+
+# {{{ ModifiedL1
+
+
 @dataclass(frozen=True)
-class CaputoModifiedL1Method(CaputoL1Method):
+class ModifiedL1(CaputoDerivativeMethod):
     r"""Implements the modified L1 method for the Caputo fractional derivative
     of order :math:`\alpha \in (0, 1)`.
 
     This method is defined in Section 4.1.1 (III) from [Li2020]_ for quasi-uniform
-    grids. Note that it cannot compute the derivative at the starting point, i.e.
-    :math:`D_C^\alpha[f](a)` is undefined.
-
-    This method is of order :math:`\mathcal{O}(h^{2 - \alpha})` and requires
-    a special grid constructed by :func:`~pycaputo.grid.make_uniform_midpoints`.
+    grids. These grids can be constructed by :class:`~pycaputo.grid.UniformMidpoints`.
     """
 
+    if __debug__:
+
+        def __post_init__(self) -> None:
+            super().__post_init__()
+            if not 0 < self.alpha < 1:
+                raise ValueError(
+                    f"'{type(self).__name__}' only supports 0 < alpha < 1: {self.alpha}"
+                )
+
 
-def _weights_modified_l1(m: CaputoModifiedL1Method, p: Points) -> Iterator[Array]:
+def _weights_modified_l1(m: ModifiedL1, p: Points) -> Iterator[Array]:
     if not isinstance(p, UniformMidpoints):
         raise NotImplementedError(
             f"'{type(m).__name__}' does not implement 'weights' for"
             f" '{type(p).__name__}' grids"
         )
 
     # NOTE: weights from [Li2020] Equation 4.51
     # FIXME: this does not use the formula from the book; any benefit to it?
-    alpha = m.d.order
+    alpha = m.alpha
     wc = 1 / math.gamma(2 - alpha) / p.dx[-1] ** alpha
     k = np.arange(p.x.size)
 
     # NOTE: first interval has a size of h / 2 and is weighted differently
     w0 = 2 * ((k[:-1] + 0.5) ** (1 - alpha) - k[:-1] ** (1 - alpha))
 
     for n in range(1, p.x.size):
         w = (n - k[:n]) ** (1 - alpha) - (n - k[:n] - 1) ** (1 - alpha)
         w[0] = w0[n - 1]
 
         yield wc * w
 
 
-@diff.register(CaputoModifiedL1Method)
-def _diff_modified_l1method(
-    m: CaputoModifiedL1Method, f: ArrayOrScalarFunction, p: Points
+@diff.register(ModifiedL1)
+def _diff_modified_l1_method(
+    m: ModifiedL1, f: ArrayOrScalarFunction, p: Points
 ) -> Array:
     if not isinstance(p, UniformMidpoints):
         raise NotImplementedError(
             f"'{type(m).__name__}' does not implement 'diff' for '{type(p).__name__}'"
             " grids"
         )
 
@@ -152,49 +162,46 @@
 
     return df
 
 
 # }}}
 
 
-# {{{ Caputo L2 Method
+# {{{ L2
 
 
 @dataclass(frozen=True)
-class CaputoL2Method(CaputoDerivativeMethod):
+class L2(CaputoDerivativeMethod):
     r"""Implements the L2 method for the Caputo fractional derivative
     of order :math:`\alpha \in (1, 2)`.
 
-    This method is defined in Section 4.1.2 from [Li2020]_. Note that
-    it cannot compute the derivative at the starting point, i.e.
-    :math:`D_C^\alpha[f](a)` is undefined.
-
-    This method is of order :math:`\mathcal{O}(h^{3 - \alpha})` and supports
-    only uniform grids.
+    This method is defined in Section 4.1.2 from [Li2020]_ for uniform grids.
     """
 
-    @property
-    def order(self) -> float:
-        return 1
+    if __debug__:
 
-    def supports(self, alpha: float) -> bool:
-        return 1 < alpha < 2
+        def __post_init__(self) -> None:
+            super().__post_init__()
+            if not 1 < self.alpha < 2:
+                raise ValueError(
+                    f"'{type(self).__name__}' only supports 0 < alpha < 1: {self.alpha}"
+                )
 
 
 def _weights_l2(alpha: float, i: int | Array, k: int | Array) -> Array:
     return np.array((i - k) ** (2 - alpha) - (i - k - 1) ** (2 - alpha))
 
 
-@diff.register(CaputoL2Method)
-def _diff_l2method(m: CaputoL2Method, f: ArrayOrScalarFunction, p: Points) -> Array:
+@diff.register(L2)
+def _diff_l2_method(m: L2, f: ArrayOrScalarFunction, p: Points) -> Array:
     # precompute variables
     x = p.x
     fx = f(x) if callable(f) else f
 
-    alpha = m.d.order
+    alpha = m.alpha
     w0 = 1 / math.gamma(3 - alpha)
 
     # NOTE: [Li2020] Section 4.2
     # NOTE: the method is not written as in [Li2020] and has several tweaks:
     # * terms are written as `sum(w * f'')` instead of `sum(w * f)`, which
     #   makes it easier to express w
     # * boundary terms are approximated with a biased stencil.
@@ -219,44 +226,42 @@
 
     return df
 
 
 # }}}
 
 
-# {{{ CaputoL2CMethod
+# {{{ L2C
 
 
 @dataclass(frozen=True)
-class CaputoL2CMethod(CaputoL2Method):
+class L2C(CaputoDerivativeMethod):
     r"""Implements the L2C method for the Caputo fractional derivative
     of order :math:`\alpha \in (1, 2)`.
 
-    This method is defined in Section 4.1.2 from [Li2020]_. Note that
-    it cannot compute the derivative at the starting point, i.e.
-    :math:`D_C^\alpha[f](a)` is undefined.
-
-    This method is of order :math:`\mathcal{O}(h^{3 - \alpha})` and supports
-    only uniform grids.
+    This method is defined in Section 4.1.2 from [Li2020]_ on uniform grids.
     """
 
-    @property
-    def order(self) -> float:
-        return 3 - self.d.order
+    if __debug__:
 
+        def __post_init__(self) -> None:
+            super().__post_init__()
+            if not 1 < self.alpha < 2:
+                raise ValueError(
+                    f"'{type(self).__name__}' only supports 0 < alpha < 1: {self.alpha}"
+                )
 
-@diff.register(CaputoL2CMethod)
-def _diff_uniform_l2cmethod(
-    m: CaputoL2CMethod, f: ArrayOrScalarFunction, p: Points
-) -> Array:
+
+@diff.register(L2C)
+def _diff_l2c_method(m: L2C, f: ArrayOrScalarFunction, p: Points) -> Array:
     # precompute variables
     x = p.x
     fx = f(x) if callable(f) else f
 
-    alpha = m.d.order
+    alpha = m.alpha
     w0 = 1 / math.gamma(3 - alpha)
 
     # NOTE: [Li2020] Section 4.2
     df = np.empty_like(x)
     df[0] = np.nan
 
     if isinstance(p, UniformPoints):
@@ -276,19 +281,20 @@
         )
 
     return df
 
 
 # }}}
 
-# {{{ CaputoSpectralMethod
+
+# {{{ SpectralJacobi
 
 
 @dataclass(frozen=True)
-class CaputoSpectralMethod(CaputoDerivativeMethod):
+class SpectralJacobi(CaputoDerivativeMethod):
     r"""Caputo derivative approximation using spectral methods based
     on Jacobi polynomials.
 
     This method is described in more detail in Section 4.4 of [Li2020]_. It
     approximates the function by projecting it to the Jacobi polynomial basis
     and constructing a quadrature rule, i.e.
 
@@ -303,42 +309,31 @@
     polynomials :math:`P^{(u, v)}`.
 
     This method is of the order of the Jacobi polynomials and requires
     a Gauss-Jacobi-Lobatto grid (for the projection :math:`\hat{f}_k`) as
     constructed by :func:`~pycaputo.grid.make_jacobi_gauss_lobatto_points`.
     """
 
-    @property
-    def name(self) -> str:
-        return "CSpec"
-
-    @property
-    def order(self) -> float:
-        return np.inf
-
-    def supports(self, alpha: float) -> bool:
-        return 0 < alpha < np.inf
-
 
-@diff.register(CaputoSpectralMethod)
-def _diff_jacobi(m: CaputoSpectralMethod, f: ArrayOrScalarFunction, p: Points) -> Array:
+@diff.register(SpectralJacobi)
+def _diff_jacobi(m: SpectralJacobi, f: ArrayOrScalarFunction, p: Points) -> Array:
     from pycaputo.grid import JacobiGaussLobattoPoints
 
     if not isinstance(p, JacobiGaussLobattoPoints):
         raise TypeError(
             f"Only JacobiGaussLobattoPoints points are supported: '{type(p).__name__}'"
         )
 
     from pycaputo.jacobi import jacobi_caputo_derivative, jacobi_project
 
     # NOTE: Equation 3.63 [Li2020]
     fx = f(p.x) if callable(f) else f
     fhat = jacobi_project(fx, p)
 
     df = np.zeros_like(fhat)
-    for n, Dhat in jacobi_caputo_derivative(p, m.d.order):
+    for n, Dhat in jacobi_caputo_derivative(p, m.alpha):
         df += fhat[n] * Dhat
 
     return df
 
 
 # }}}
```

### Comparing `pycaputo-0.5.0/src/pycaputo/fode/caputo.py` & `pycaputo-0.6.0/src/pycaputo/fode/caputo.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 from pycaputo.derivatives import CaputoDerivative, Side
 from pycaputo.fode.product_integration import (
     AdvanceResult,
     ProductIntegrationMethod,
 )
 from pycaputo.history import ProductIntegrationHistory
 from pycaputo.logging import get_logger
-from pycaputo.stepping import advance, gamma1p, gamma2m, make_initial_condition
+from pycaputo.stepping import advance, gamma1p, gamma2m, gamma2p, make_initial_condition
 from pycaputo.utils import Array, StateFunctionT, gamma
 
 logger = get_logger(__name__)
 
 
 def _update_caputo_initial_condition(
-    out: Array, m: CaputoProductIntegrationMethod[StateFunctionT], t: float
+    out: Array, y0: tuple[Array, ...], t: float
 ) -> Array:
-    """Adds the appropriate initial conditions to *dy*."""
-    t = t - m.control.tstart
-    for k, y0k in enumerate(m.y0):
+    """Adds the appropriate initial conditions to *out*."""
+    for k, y0k in enumerate(y0):
         out += t**k / gamma(k + 1) * y0k
 
     return out
 
 
 def _truncation_error(
     c: Controller, alpha: Array, t: float, y: Array, tprev: float, yprev: Array
@@ -57,15 +56,15 @@
 
 
 @dataclass(frozen=True)
 class CaputoProductIntegrationMethod(ProductIntegrationMethod[StateFunctionT]):
     @cached_property
     def d(self) -> tuple[CaputoDerivative, ...]:
         return tuple([
-            CaputoDerivative(order=alpha, side=Side.Left)
+            CaputoDerivative(alpha=alpha, side=Side.Left)
             for alpha in self.derivative_order
         ])
 
 
 @make_initial_condition.register(CaputoProductIntegrationMethod)
 def _make_initial_condition_caputo(
     m: CaputoProductIntegrationMethod[StateFunctionT],
@@ -84,48 +83,58 @@
     """The first-order forward Euler discretization of the Caputo derivative."""
 
     @property
     def order(self) -> float:
         return 1.0
 
 
-def _update_caputo_forward_euler(
-    dy: Array,
+def _weights_quadrature_rectangular(
     m: CaputoProductIntegrationMethod[StateFunctionT],
-    history: ProductIntegrationHistory,
+    t: Array,
     n: int,
 ) -> Array:
-    """Adds the Forward Euler right-hand side to *dy*."""
     # get time history
-    assert 0 < n <= len(history)
-    ts = history.ts[n] - history.ts[: n + 1]
+    ts = (t[n] - t[: n + 1]).reshape(-1, 1)
 
-    # sum up convolution
-    alpha = m.alpha.reshape(-1, 1)
-    g1p = gamma1p(m).reshape(-1, 1)
+    alpha = m.alpha
+    g1p = gamma1p(m)
     omega = (ts[:-1] ** alpha - ts[1:] ** alpha) / g1p
-    dy += np.einsum("ij,ij->j", omega.T, history.storage[:n])
 
-    return dy
+    return np.array(omega)
+
+
+def _update_caputo_forward_euler(
+    out: Array,
+    m: CaputoProductIntegrationMethod[StateFunctionT],
+    history: ProductIntegrationHistory,
+    n: int,
+) -> Array:
+    """Adds the Forward Euler right-hand side to *out*."""
+    assert 0 < n <= len(history)
+    omega = _weights_quadrature_rectangular(m, history.ts, n)
+
+    out += np.einsum("ij,ij->j", omega, history.storage[:n])
+    return out
 
 
 @advance.register(ForwardEuler)
 def _advance_caputo_forward_euler(
     m: ForwardEuler[StateFunctionT],
     history: ProductIntegrationHistory,
     y: Array,
     dt: float,
 ) -> AdvanceResult:
     # set next time step
     n = len(history)
+    tstart = m.control.tstart
     t = history.ts[n] = history.ts[n - 1] + dt
 
     # compute solution
     ynext = np.zeros_like(y)
-    ynext = _update_caputo_initial_condition(ynext, m, t)
+    ynext = _update_caputo_initial_condition(ynext, m.y0, t - tstart)
     ynext = _update_caputo_forward_euler(ynext, m, history, n)
 
     trunc = _truncation_error(m.control, m.alpha, t, ynext, t - dt, y)
     return AdvanceResult(ynext, trunc, m.source(t, ynext))
 
 
 # }}}
@@ -206,72 +215,292 @@
             c,
             r,
             **self._get_kwargs(scalar=y0.size == 1),
         )
 
 
 def _update_caputo_weighted_euler(
-    dy: Array,
+    out: Array,
     m: WeightedEuler[StateFunctionT],
     history: ProductIntegrationHistory,
     n: int,
 ) -> tuple[Array, Array]:
-    """Adds the weighted Euler right-hand side to *dy*."""
-    # NOTE: this is implicit so we never want to compute the last term
+    """Adds the weighted Euler right-hand side to *out*."""
     assert 0 < n <= len(history)
-
-    ts = history.ts[n] - history.ts[: n + 1]
-    theta = m.theta
-
-    # add explicit terms
-    alpha = m.alpha.reshape(-1, 1)
-    g1p = gamma1p(m).reshape(-1, 1)
-    omega = ((ts[:-1] ** alpha - ts[1:] ** alpha) / g1p).T
+    omega = _weights_quadrature_rectangular(m, history.ts, n)
 
     # add forward terms
+    theta = m.theta
     fs = history.storage[:n]
     if theta != 0.0:
-        dy += theta * np.einsum("ij,ij->j", omega, fs)
+        out += theta * np.einsum("ij,ij->j", omega, fs)
 
     # add backwards terms
     if theta != 1.0:
-        dy += (1 - theta) * np.einsum("ij,ij->j", omega[:-1], fs[1:])
+        # NOTE: this is implicit so we do not add the last term
+        out += (1 - theta) * np.einsum("ij,ij->j", omega[:-1], fs[1:])
 
-    return dy, omega[-1].squeeze()
+    return out, (1 - theta) * omega[-1].squeeze()
 
 
 @advance.register(WeightedEuler)
 def _advance_caputo_weighted_euler(
     m: WeightedEuler[StateFunctionT],
     history: ProductIntegrationHistory,
     y: Array,
     dt: float,
 ) -> AdvanceResult:
     # set next time step
     n = len(history)
+    tstart = m.control.tstart
     t = history.ts[n] = history.ts[n - 1] + dt
 
     # add explicit terms
     fnext = np.zeros_like(y)
-    fnext = _update_caputo_initial_condition(fnext, m, t)
-    fnext, omega = _update_caputo_weighted_euler(fnext, m, history, n)
+    fnext = _update_caputo_initial_condition(fnext, m.y0, t - tstart)
+    fnext, fac = _update_caputo_weighted_euler(fnext, m, history, n)
 
-    # solve implicit equation
     if m.theta != 1.0:  # noqa: SIM108
-        ynext = m.solve(t, y, omega * (1 - m.theta), fnext)
+        # NOTE: solve `y = fac * f(t, y) + fnext`
+        ynext = m.solve(t, y, fac, fnext)
     else:
         ynext = fnext
 
     trunc = _truncation_error(m.control, m.alpha, t, ynext, t - dt, y)
     return AdvanceResult(ynext, trunc, m.source(t, ynext))
 
 
 # }}}
 
 
+# {{{ Trapezoidal
+
+
+@dataclass(frozen=True)
+class Trapezoidal(CaputoProductIntegrationMethod[StateFunctionT]):
+    """The trapezoidal method for discretizing the Caputo derivative.
+
+    This is an implicit method described in [Garrappa2015b]_. It uses a linear
+    interpolant on each time step.
+    """
+
+    source_jac: StateFunctionT | None
+    r"""Jacobian of
+    :attr:`~pycaputo.stepping.FractionalDifferentialEquationMethod.source`.
+    By default, implicit methods use :mod:`scipy` for their root finding,
+    which defines the Jacobian as :math:`J_{ij} = \partial f_i / \partial y_j`.
+    """
+
+    @property
+    def order(self) -> float:
+        return 2.0
+
+    # NOTE: `_get_kwargs` is meant to be overwritten for testing purposes or
+    # some specific application (undocumented for now).
+
+    def _get_kwargs(self, *, scalar: bool = True) -> dict[str, object]:
+        """
+        :returns: additional keyword arguments for :func:`scipy.optimize.root_scalar`.
+            or :func:`scipy.optimize.root`.
+        """
+        if scalar:
+            return {}
+        else:
+            # NOTE: the default hybr does not use derivatives, so use lm instead
+            # FIXME: will need to maybe benchmark these a bit?
+            return {"method": "lm" if self.source_jac else None}
+
+    def solve(self, t: float, y0: Array, c: Array, r: Array) -> Array:
+        """Wrapper around :func:`~pycaputo.implicit.solve` to solve the
+        implicit equation.
+
+        This function should be overwritten for specific applications if better
+        solvers are known. For example, many problems can be solved explicitly
+        or approximated to a very good degree to provide a better *y0*.
+        """
+        from pycaputo.implicit import solve
+
+        result = solve(
+            self.source,
+            self.source_jac,
+            t,
+            y0,
+            c,
+            r,
+            **self._get_kwargs(scalar=y0.size == 1),
+        )
+        assert np.linalg.norm(result - c * self.source(t, result) - r) < 1.0e-8
+
+        return result
+
+
+def _weights_quadrature_trapezoidal(
+    m: CaputoProductIntegrationMethod[StateFunctionT],
+    t: Array,
+    n: int,
+    p: int,
+) -> tuple[Array, Array]:
+    # get time history
+    ts = (t[n] - t[: p + 1]).reshape(-1, 1)
+    dt = np.diff(t[: p + 1]).reshape(-1, 1)
+
+    alpha = m.alpha
+    r0 = ts**alpha / gamma1p(m)
+    r1 = ts ** (1.0 + alpha) / gamma2p(m)
+
+    omegal = r1[1:] / dt + r0[:-1] - r1[:-1] / dt
+    omegar = r1[:-1] / dt - r0[1:] - r1[1:] / dt
+
+    return omegal, omegar
+
+
+def _update_caputo_trapezoidal(
+    out: Array,
+    m: CaputoProductIntegrationMethod[StateFunctionT],
+    history: ProductIntegrationHistory,
+    n: int,
+    p: int,
+) -> tuple[Array, Array]:
+    assert 0 < n <= len(history)
+    assert 0 < p <= n
+    omegal, omegar = _weights_quadrature_trapezoidal(m, history.ts, n, p)
+    fs = history.storage[:p]
+
+    # add forward terms
+    out += np.einsum("ij,ij->j", omegal, fs)
+    # add backward terms
+    out += np.einsum("ij,ij->j", omegar[:-1], fs[1:])
+
+    if p < n:
+        out += omegar[-1] * history.storage[p]
+
+    return out, omegar[-1].squeeze()
+
+
+def _error_explicit_step(
+    m: ProductIntegrationMethod[StateFunctionT],
+    t: Array,
+    f: Array,
+) -> Array:
+    assert t.shape[0] == f.shape[0] == 3
+    alpha = m.alpha
+    dt = np.diff(t)
+
+    # numbering {f[0] = f_{n - 2}, f[1] = f_{n - 1}, f[2] = f_n}
+    c2 = dt[1] ** alpha / gamma2p(m)
+    c1 = -c2 * (dt[1] / dt[0] + alpha + 1)
+    c0 = c2 * dt[1] / dt[0]
+    result = c0 * f[0] + c1 * f[1] + c2 * f[2]
+
+    return np.array(result)
+
+
+@advance.register(Trapezoidal)
+def _advance_caputo_trapezoidal(
+    m: Trapezoidal[StateFunctionT],
+    history: ProductIntegrationHistory,
+    y: Array,
+    dt: Array,
+) -> AdvanceResult:
+    # set next time step
+    n = len(history)
+    tstart = m.control.tstart
+    t = history.ts[n] = history.ts[n - 1] + dt
+
+    # compute solution
+    fnext = np.zeros_like(y)
+    fnext = _update_caputo_initial_condition(fnext, m.y0, t - tstart)
+    fnext, fac = _update_caputo_trapezoidal(fnext, m, history, n, n)
+
+    # solve `ynext = fac * f(t, ynext) + fnext`
+    ynext = m.solve(t, y, fac, fnext)
+
+    trunc = _truncation_error(m.control, m.alpha, t, ynext, t - dt, y)
+    return AdvanceResult(ynext, trunc, m.source(t, ynext))
+
+
+@dataclass(frozen=True)
+class ExplicitTrapezoidal(CaputoProductIntegrationMethod[StateFunctionT]):
+    r"""An explicit trapezoidal method for discretizing the Caputo derivative.
+
+    This is an explicit method described in [Garrappa2010]_. Unlike
+    :class:`Trapezoidal`, the last step is estimated by extrapolation, making this
+    an explicit method instead with decreased stability.
+
+    .. warning::
+
+        The extrapolation from [Garrappa2010]_ does not match the one that is
+        used here even in the uniform case. To our knowledge, the paper has an
+        error and the last term in the second line from Equation 8 should be
+
+        .. math::
+
+            (2 \boldsymbol{+ \beta}) \alpha_0 f(t_{n - 1}, y_{n - 1}).
+    """
+
+    @property
+    def order(self) -> float:
+        return 1.0 + self.smallest_derivative_order
+
+
+def _update_caputo_explicit_trapezoidal(
+    out: Array,
+    t: Array,
+    f: Array,
+    alpha: Array,
+    n: int,
+) -> Array:
+    ts1 = t[n] - t[n - 1]
+    dt2 = t[n - 1] - t[n - 2]
+    fm1 = f[n - 1]
+    fm2 = f[n - 2]
+
+    # fmt: off
+    omegal = -(ts1 ** (1 + alpha)) / gamma(2 + alpha) / dt2
+    out += omegal * fm2
+    omegar = (
+        ts1 ** (1 + alpha) / gamma(2 + alpha) / dt2
+        + ts1 ** alpha / gamma(1 + alpha))
+    out += omegar * fm1
+    # fmt: on
+
+    return out
+
+
+@advance.register(ExplicitTrapezoidal)
+def _advance_caputo_explicit_trapezoidal(
+    m: ExplicitTrapezoidal[StateFunctionT],
+    history: ProductIntegrationHistory,
+    y: Array,
+    dt: Array,
+) -> AdvanceResult:
+    # set next time step
+    n = len(history)
+    tstart = m.control.tstart
+    t = history.ts[n] = history.ts[n - 1] + dt
+
+    # compute solution
+    ynext = np.zeros_like(y)
+    ynext = _update_caputo_initial_condition(ynext, m.y0, t - tstart)
+
+    if n <= 1:
+        ynext = _update_caputo_forward_euler(ynext, m, history, n)
+    else:
+        ynext, _ = _update_caputo_trapezoidal(ynext, m, history, n, n - 1)
+        ynext = _update_caputo_explicit_trapezoidal(
+            ynext, history.ts, history.storage, m.alpha, n
+        )
+
+    trunc = _truncation_error(m.control, m.alpha, t, ynext, t - dt, y)
+    return AdvanceResult(ynext, trunc, m.source(t, ynext))
+
+
+# }}}
+
+
 # {{{ Predictor-Corector (PEC and PECE)
 
 
 @dataclass(frozen=True)
 class CaputoPredictorCorrectorMethod(CaputoProductIntegrationMethod[StateFunctionT]):
     r"""The Predictor-Corrector discretization of the Caputo derivative.
 
@@ -413,19 +642,20 @@
 ) -> AdvanceResult:
     from pycaputo.utils import single_valued
 
     n = len(history)
     alpha = single_valued(m.derivative_order)
 
     # set next time step
+    tstart = m.control.tstart
     t = history.ts[n] = history.ts[n - 1] + dt
 
     # add initial conditions
     y0 = np.zeros_like(y)
-    y0 = _update_caputo_initial_condition(y0, m, t)
+    y0 = _update_caputo_initial_condition(y0, m.y0, t - tstart)
 
     # predictor step (forward Euler)
     yp = np.copy(y0)
     yp = _update_caputo_forward_euler(yp, m, history, len(history))
 
     # corrector step (Adams-Bashforth 2)
     yc_explicit = np.copy(y0)
@@ -476,23 +706,24 @@
 
     n = len(history)
     alpha = single_valued(m.derivative_order)
     gamma2 = gamma(2 + alpha)
     gamma1 = gamma(1 + alpha)
 
     # set next time step
+    tstart = m.control.tstart
     t = history.ts[n] = history.ts[n - 1] + dt
 
     ts = history.ts[: n + 1]
     ds = np.diff(ts)
     ts = history.ts[n] - ts
 
     # compute common terms
     dy = np.zeros_like(y)
-    dy = _update_caputo_initial_condition(dy, m, t)
+    dy = _update_caputo_initial_condition(dy, m.y0, t - tstart)
 
     if n == 1:
         yp = _update_caputo_forward_euler(dy, m, history, len(history))
     else:
         dy, _ = _update_caputo_adams_bashforth2(dy, history, alpha, n=n)
 
         # compute predictor
```

### Comparing `pycaputo-0.5.0/src/pycaputo/fode/product_integration.py` & `pycaputo-0.6.0/src/pycaputo/fode/product_integration.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/ad_ex.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/ad_ex.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/base.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             super().__post_init__()
             if any(a > 1.0 or a < 0.0 for a in self.derivative_order):
                 raise ValueError(f"Expected 'alpha' in (0, 1): {self.derivative_order}")
 
     @cached_property
     def d(self) -> tuple[CaputoDerivative, ...]:
         return tuple([
-            CaputoDerivative(order=alpha, side=Side.Left)
+            CaputoDerivative(alpha=alpha, side=Side.Left)
             for alpha in self.derivative_order
         ])
 
     @property
     def order(self) -> float:
         return 1.0
```

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/eif.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/eif.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/lif.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/lif.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 
         n += 1
 
     return a, b
 
 
 def _find_first_spike_time(p: LIF, V0: float = 0.0) -> float:
-    from pycaputo.mittagleffler import mittag_leffler_diethelm
+    from pycaputo.mittagleffler import _mittag_leffler_diethelm
 
     alpha = p.ref.alpha
 
     def func(t: float) -> float:
         a = p.current + p.e_leak
         b = a - V0
 
-        E = mittag_leffler_diethelm(-(t**alpha), alpha=alpha, beta=1.0)
+        E = _mittag_leffler_diethelm(-(t**alpha), alpha=alpha, beta=1.0)
         result = a - b * E - p.v_peak
 
         return float(np.real_if_close(result))
 
     import scipy.optimize as so
 
     bracket = _find_bracket(func)
```

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/pif.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/pif.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/integrate_fire/spikes.py` & `pycaputo-0.6.0/src/pycaputo/integrate_fire/spikes.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/src/pycaputo/quadrature/base.py` & `pycaputo-0.6.0/src/pycaputo/quadrature/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,47 +10,35 @@
 from pycaputo.derivatives import FractionalOperator
 from pycaputo.grid import Points
 from pycaputo.utils import Array, ArrayOrScalarFunction
 
 
 @dataclass(frozen=True)
 class QuadratureMethod(ABC):
-    """A generic method used to evaluate a fractional integral."""
-
-    d: FractionalOperator
-    """Description of the integral that is approximated."""
-
-    if __debug__:
-
-        def __post_init__(self) -> None:
-            if self.d.order >= 0:
-                raise ValueError(
-                    f"Integral requires a negative order: order is '{self.d.order}'"
-                )
+    """A generic method used to evaluate a fractional integral at a set of points."""
 
     @property
-    @abstractmethod
     def name(self) -> str:
         """An identifier for the quadrature method."""
         return type(self).__name__.replace("Method", "")
 
     @property
     @abstractmethod
-    def order(self) -> float:
-        """Expected order of convergence of the method."""
+    def d(self) -> FractionalOperator:
+        """The fractional operator that is being discretized by the method."""
 
 
 @singledispatch
-def quad(m: QuadratureMethod, f: ArrayOrScalarFunction, x: Points) -> Array:
-    """Evaluate the fractional integral of *f* using the points *x*.
+def quad(m: QuadratureMethod, f: ArrayOrScalarFunction, p: Points) -> Array:
+    """Evaluate the fractional integral of *f* at *p* using method *m*.
 
     :arg m: method used to evaluate the integral.
     :arg f: a simple function for which to evaluate the integral. If the
         method requires higher-order derivatives (e.g. for Hermite interpolation),
         this function can also be a
         :class:`~pycaputo.utils.DifferentiableScalarFunction`.
-    :arg x: an array of points at which to evaluate the integral.
+    :arg p: an array of points at which to evaluate the integral.
     """
 
     raise NotImplementedError(
-        f"Cannot evaluate integral with method '{type(m).__name__}'"
+        f"Cannot evaluate fractional integral with method '{type(m).__name__}'"
     )
```

### Comparing `pycaputo-0.5.0/src/pycaputo/quadrature/riemann_liouville.py` & `pycaputo-0.6.0/src/pycaputo/quadrature/riemann_liouville.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass
+from functools import cached_property
 
 import numpy as np
 
-from pycaputo.derivatives import RiemannLiouvilleDerivative
+from pycaputo.derivatives import RiemannLiouvilleDerivative, Side
 from pycaputo.grid import Points
 from pycaputo.utils import Array, ArrayOrScalarFunction, DifferentiableScalarFunction
 
 from .base import QuadratureMethod, quad
 
 
 @dataclass(frozen=True)
 class RiemannLiouvilleMethod(QuadratureMethod):
     """Quadrature method for the Riemann-Liouville integral."""
 
-    d: RiemannLiouvilleDerivative
-    """Description of the integral that is approximated."""
+    alpha: float
+    """Order of the Riemann-Liouville integral that is being discretized."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
-            super().__post_init__()
-            if not isinstance(self.d, RiemannLiouvilleDerivative):
-                raise TypeError(
-                    f"Expected a Riemann-Liouville integral: '{type(self.d).__name__}'"
-                )
+            if self.alpha > 0:
+                raise ValueError(f"Positive orders are not supported: {self.alpha}")
+
+    @property
+    def d(self) -> RiemannLiouvilleDerivative:
+        return RiemannLiouvilleDerivative(self.alpha, side=Side.Left)
 
 
-# {{{ RiemannLiouvilleRectangularMethod
+# {{{ Rectangular
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleRectangularMethod(RiemannLiouvilleMethod):
+class Rectangular(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using the rectangular formula.
 
-    The rectangular formula is derived in Section 3.1.(I) from [Li2020]_. It
-    uses a piecewise constant approximation on each subinterval and cannot
-    be used to evaluate the value at the starting point, i.e.
-    :math:`I_{RL}^\alpha[f](a)` is not defined.
-
-    This method is of order :math:`\mathcal{O}(h)` and supports arbitrary grids.
+    The rectangular formula is derived in Section 3.1.(I) from [Li2020]_ for
+    general non-uniform grids.
     """
 
     theta: float = 0.5
     r"""Weight used in the approximation :math:`\theta f_k + (1 - \theta) f_{k + 1}`."""
 
     if __debug__:
 
@@ -59,31 +57,24 @@
                     f"Weight is expected to be in [0, 1]: theta is '{self.theta}'"
                 )
 
     @property
     def name(self) -> str:
         return "RLRect"
 
-    @property
-    def order(self) -> float:
-        if self.theta == 0.5:
-            return min(2.0, 1.0 - self.d.order)
-
-        return 1.0
-
 
-@quad.register(RiemannLiouvilleRectangularMethod)
+@quad.register(Rectangular)
 def _quad_rl_rect(
-    m: RiemannLiouvilleRectangularMethod,
+    m: Rectangular,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     x = p.x
     fx = f(x) if callable(f) else f
-    alpha = -m.d.order
+    alpha = -m.alpha
     w0 = 1 / math.gamma(1 + alpha)
 
     fc = m.theta * fx[:-1] + (1 - m.theta) * fx[1:]
 
     # compute integral
     qf = np.empty_like(fx)
     qf[0] = np.nan
@@ -94,49 +85,41 @@
 
     return qf
 
 
 # }}}
 
 
-# {{{ RiemannLiouvilleTrapezoidalMethod
+# {{{ Trapezoidal
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleTrapezoidalMethod(RiemannLiouvilleMethod):
+class Trapezoidal(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using the trapezoidal formula.
 
-    The trapezoidal formula is derived in Section 3.1.(II) from [Li2020]_. It
-    uses a linear approximation on each subinterval and cannot be used to
-    evaluate the value at the starting point, i.e.
-    :math:`I_{RL}^\alpha[f](a)` is not defined.
-
-    This method is of order :math:`\mathcal{O}(h^2)` and supports arbitrary grids.
+    The trapezoidal formula is derived in Section 3.1.(II) from [Li2020]_ for
+    general non-uniform grids.
     """
 
     @property
     def name(self) -> str:
         return "RLTrap"
 
-    @property
-    def order(self) -> float:
-        return 2.0
-
 
-@quad.register(RiemannLiouvilleTrapezoidalMethod)
+@quad.register(Trapezoidal)
 def _quad_rl_trap(
-    m: RiemannLiouvilleTrapezoidalMethod,
+    m: Trapezoidal,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     from pycaputo.grid import UniformPoints
 
     x = p.x
     fx = f(x) if callable(f) else f
-    alpha = -m.d.order
+    alpha = -m.alpha
     w0 = 1 / math.gamma(2 + alpha)
 
     # compute integral
     qf = np.empty_like(fx)
     qf[0] = np.nan
 
     if isinstance(p, UniformPoints):
@@ -166,56 +149,48 @@
 
     return qf
 
 
 # }}}
 
 
-# {{{ RiemannLiouvilleSimpsonMethod
+# {{{ Simpson
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleSimpsonMethod(RiemannLiouvilleMethod):
+class Simpson(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using Simpson's method.
 
-    This method is described in more detail in Section 3.3.(III) of [Li2020]_. It
-    uses a quadratic approximation on each subinterval and cannot be used to
-    evaluate the value at the starting point, i.e.
-    :math:`I_{RL}^\alpha[f](a)` is not defined.
-
-    This method is of order :math:`\mathcal{O}(h^3)` and supports uniform grids.
+    This method is described in more detail in Section 3.3.(III) of [Li2020]_
+    for uniform grids.
     """
 
     @property
     def name(self) -> str:
         return "RLSimpson"
 
-    @property
-    def order(self) -> float:
-        return 3.0
-
 
-@quad.register(RiemannLiouvilleSimpsonMethod)
+@quad.register(Simpson)
 def _quad_rl_simpson(
-    m: RiemannLiouvilleSimpsonMethod,
+    m: Simpson,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     from pycaputo.grid import UniformPoints
 
     if not callable(f):
         raise TypeError(f"Input 'f' needs to be a callable: {type(f).__name__}")
 
     if not isinstance(p, UniformPoints):
         raise TypeError(f"Only uniform points are supported: {type(p).__name__}")
 
     fx = f(p.x)
     fm = f(p.xm)
 
-    alpha = -m.d.order
+    alpha = -m.alpha
     w0 = p.dx[0] ** alpha / math.gamma(3 + alpha)
     indices = np.arange(fx.size)
 
     # compute integral
     qf = np.empty_like(fx)
     qf[0] = np.nan
 
@@ -260,58 +235,50 @@
 
     return np.array(w0 * qf)
 
 
 # }}}
 
 
-# {{{ RiemannLiouvilleCubicHermiteMethod
+# {{{ CubicHermite
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleCubicHermiteMethod(RiemannLiouvilleMethod):
+class CubicHermite(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using a cubic Hermite interpolant.
 
-    This method is described in more detail in Section 3.3.(B) of [Li2020]_. It
-    uses a cubic approximation on each subinterval and cannot be used to
-    evaluate the value at the starting point, i.e.
-    :math:`I_{RL}^\alpha[f](a)` is not defined.
+    This method is described in more detail in Section 3.3.(B) of [Li2020]_
+    for uniform grids.
 
     Note that Hermite interpolants require derivative values at the grid points.
-
-    This method is of order :math:`\mathcal{O}(h^4)` and supports uniform grids.
     """
 
     @property
     def name(self) -> str:
-        return "RLCHermite"
-
-    @property
-    def order(self) -> float:
-        return 4.0
+        return "RLCubicHermite"
 
 
-@quad.register(RiemannLiouvilleCubicHermiteMethod)
+@quad.register(CubicHermite)
 def _quad_rl_cubic_hermite(
-    m: RiemannLiouvilleCubicHermiteMethod,
+    m: CubicHermite,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     from pycaputo.grid import UniformPoints
 
     if not isinstance(f, DifferentiableScalarFunction):
         raise TypeError(f"Input 'f' needs to be a callable: {type(f).__name__}")
 
     if not isinstance(p, UniformPoints):
         raise TypeError(f"Only uniform points are supported: {type(p).__name__}")
 
     fx = f(p.x, d=0)
     fp = f(p.x, d=1)
 
-    alpha = -m.d.order
+    alpha = -m.alpha
     h = p.dx[0]
     w0 = h**alpha / math.gamma(4 + alpha)
     indices = np.arange(fx.size)
 
     # compute integral
     qf = np.empty_like(fx)
     qf[0] = np.nan
@@ -348,19 +315,19 @@
 
     return np.array(w0 * qf)
 
 
 # }}}
 
 
-# {{{ RiemannLiouvilleSpectralMethod: Jacobi polynomials
+# {{{ SpectralJacobi
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleSpectralMethod(RiemannLiouvilleMethod):
+class SpectralJacobi(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using spectral methods based
     on Jacobi polynomials.
 
     This method is described in more detail in Section 3.3 of [Li2020]_. It
     approximates the function by projecting it to the Jacobi polynomial basis
     and constructing a quadrature rule, i.e.
 
@@ -377,24 +344,20 @@
     This method is of the order of the Jacobi polynomials and requires
     a Gauss-Jacobi-Lobatto grid (for the projection :math:`\hat{f}_k`) as
     constructed by :func:`~pycaputo.grid.make_jacobi_gauss_lobatto_points`.
     """
 
     @property
     def name(self) -> str:
-        return "RLSpec"
-
-    @property
-    def order(self) -> float:
-        return np.inf
+        return "RLJacobi"
 
 
-@quad.register(RiemannLiouvilleSpectralMethod)
+@quad.register(SpectralJacobi)
 def _quad_rl_spec(
-    m: RiemannLiouvilleSpectralMethod,
+    m: SpectralJacobi,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     from pycaputo.grid import JacobiGaussLobattoPoints
 
     if not isinstance(p, JacobiGaussLobattoPoints):
         raise TypeError(
@@ -404,28 +367,115 @@
     from pycaputo.jacobi import jacobi_project, jacobi_riemann_liouville_integral
 
     # NOTE: Equation 3.63 [Li2020]
     fx = f(p.x) if callable(f) else f
     fhat = jacobi_project(fx, p)
 
     df = np.zeros_like(fhat)
-    for n, Phat in enumerate(jacobi_riemann_liouville_integral(p, -m.d.order)):
+    for n, Phat in enumerate(jacobi_riemann_liouville_integral(p, -m.alpha)):
         df += fhat[n] * Phat
 
     return df
 
 
 # }}}
 
 
-# {{{ RiemannLiouvilleConvolutionMethod: Lubich
+# {{{ SplineLagrange
+
+
+@dataclass(frozen=True)
+class SplineLagrange(RiemannLiouvilleMethod):
+    """Riemann-Lioville integral approximation using the piecewise Lagrange
+    spline method from [Cardone2021]_.
+
+    Note that, unlike other methods, this method requires evaluating the function
+    :math:`f` at interior points on each interval (based on :attr:`xi`). The
+    integral itself, however, is only evaluated at the given points :math:`x`.
+
+    This method has an order that depends on the reference points :attr:`xi` and
+    supports arbitrary grids.
+    """
+
+    npoints: int
+    """Number of points used on each element."""
+
+    if __debug__:
+
+        def __post_init__(self) -> None:
+            from warnings import warn
+
+            super().__post_init__()
+
+            if self.npoints > 16:
+                warn(
+                    "Evaluating Lagrange polynomials of order > 16 might be "
+                    "numerically unstable",
+                    stacklevel=2,
+                )
+
+            if not np.all([0 < xi < 1 for xi in self.xi]):
+                raise ValueError(f"Reference nodes are not in [0, 1]: {self.xi}")
+
+    @property
+    def name(self) -> str:
+        return "RLSpline"
+
+    @cached_property
+    def xi(self) -> Array:
+        """Reference points used to construct the Lagrange polynomials on each
+        element.
+
+        By default, this function constructs the Gauss-Legendre nodes based on
+        :attr:`npoints`. This function can be easily overwritten to make use of
+        different points. However, they must be in :math:`[0, 1]`.
+        """
+        from numpy.polynomial.legendre import leggauss
+
+        xi, _ = leggauss(self.npoints)  # type: ignore[no-untyped-call]
+        return np.array(xi + 1.0) / 2.0
+
+
+@quad.register(SplineLagrange)
+def _quad_rl_spline(
+    m: SplineLagrange,
+    f: ArrayOrScalarFunction,
+    p: Points,
+) -> Array:
+    from pycaputo.lagrange import lagrange_riemann_liouville_integral
+
+    xi = m.xi
+    alpha = -m.alpha
+
+    if not callable(f):
+        raise TypeError(
+            f"'{type(m).__name__}' only supports callable functions: 'f' is a "
+            f"{type(f).__name__}"
+        )
+
+    x = p.x[:-1].reshape(-1, 1) + p.dx.reshape(-1, 1) * xi
+    fx = f(x)
+
+    qf = np.empty(p.size, dtype=fx.dtype)
+    qf[0] = np.nan
+
+    for n, w in enumerate(lagrange_riemann_liouville_integral(p, xi, alpha)):
+        qf[n + 1] = np.sum(w * fx[: n + 1])
+
+    return qf
+
+
+# }}}
+
+
+# {{{ Lubich
 
 
 @dataclass(frozen=True)
-class RiemannLiouvilleConvolutionMethod(RiemannLiouvilleMethod):
+class Lubich(RiemannLiouvilleMethod):
     r"""Riemann-Liouville integral approximation using the convolution quadratures
     of [Lubich1986]_.
 
     This method is described in detail in [Lubich1986]_ and allows approximations
     of the form
 
     .. math::
@@ -445,14 +495,15 @@
     """
 
     quad_order: int
     """The order of the convolution quadrature method. Only orders up to 6 are
     currently supported, see :func:`~pycaputo.generating_functions.lubich_bdf_weights`
     for additional details.
     """
+
     beta: float
     r"""An exponent used in constructing the starting weights of the quadrature.
     Negative values will allow for certain singularities at the origin, while
     a default of :math:`\beta = 1` will benefit a smooth function. Setting
     this to ``float("inf")`` will disable the starting weights.
     """
 
@@ -471,22 +522,18 @@
                     f"Values of beta in 0, -1, ... are not supported: {self.beta}"
                 )
 
     @property
     def name(self) -> str:
         return "RLConv"
 
-    @property
-    def order(self) -> int:
-        return self.quad_order
-
 
-@quad.register(RiemannLiouvilleConvolutionMethod)
+@quad.register(Lubich)
 def _quad_rl_conv(
-    m: RiemannLiouvilleConvolutionMethod,
+    m: Lubich,
     f: ArrayOrScalarFunction,
     p: Points,
 ) -> Array:
     from pycaputo.grid import UniformPoints
 
     if not isinstance(p, UniformPoints):
         raise TypeError(f"Only uniforms points are supported: '{type(p).__name__}'")
@@ -494,15 +541,15 @@
     from pycaputo.generating_functions import (
         lubich_bdf_starting_weights,
         lubich_bdf_starting_weights_count,
         lubich_bdf_weights,
     )
 
     fx = f(p.x) if callable(f) else f
-    alpha = -m.d.order
+    alpha = -m.alpha
     dxa = p.dx[0] ** alpha
 
     qf = np.empty_like(fx)
     qf[0] = np.nan
 
     w = lubich_bdf_weights(-alpha, m.quad_order, p.size)
```

### Comparing `pycaputo-0.5.0/tests/test_diff_caputo.py` & `pycaputo-0.6.0/tests/test_diff_caputo.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 from dataclasses import dataclass
 
 import numpy as np
 import numpy.linalg as la
 import pytest
 
-from pycaputo.differentiation import CaputoDerivativeMethod, diff
+from pycaputo.differentiation import caputo, diff
 from pycaputo.grid import Points
 from pycaputo.logging import get_logger
 from pycaputo.utils import Array, ScalarFunction, set_recommended_matplotlib
 
 dirname = pathlib.Path(__file__).parent
 logger = get_logger("pycaputo.test_diff_caputo")
 set_recommended_matplotlib()
@@ -50,39 +50,54 @@
 
     raise ValueError(f"Unsupported order: {alpha}")
 
 
 @pytest.mark.parametrize(
     ("name", "grid_type"),
     [
-        ("CaputoL1Method", "stretch"),
-        ("CaputoL1Method", "uniform"),
-        ("CaputoModifiedL1Method", "midpoints"),
-        ("CaputoL2CMethod", "uniform"),
-        ("CaputoL2Method", "uniform"),
+        ("L1", "stretch"),
+        ("L1", "uniform"),
+        ("L2", "uniform"),
+        ("L2C", "uniform"),
+        ("ModifiedL1", "midpoints"),
     ],
 )
 @pytest.mark.parametrize("alpha", [0.1, 0.25, 0.5, 0.75, 0.9])
 def test_caputo_lmethods(
     name: str,
     grid_type: str,
     alpha: float,
     *,
     visualize: bool = False,
 ) -> None:
-    from pycaputo.differentiation import make_method_from_name
     from pycaputo.grid import make_points_from_name
 
-    if name in {"CaputoL2Method", "CaputoL2CMethod"}:
+    if name in {"L2", "L2C"}:
         alpha += 1
 
-    from pycaputo.utils import EOCRecorder, savefig
+    from pycaputo.utils import EOCRecorder, savefig, stringify_eoc
+
+    meth: caputo.CaputoDerivativeMethod
+    if name == "L1":
+        meth = caputo.L1(alpha=alpha)
+        order = 2.0 - alpha
+    elif name == "ModifiedL1":
+        meth = caputo.ModifiedL1(alpha=alpha)
+        order = 2 - alpha
+    elif name == "L2":
+        meth = caputo.L2(alpha=alpha)
+        # FIXME: this is wrong
+        order = 1.0
+    elif name == "L2C":
+        meth = caputo.L2C(alpha=alpha)
+        order = 3.0 - alpha
+    else:
+        raise ValueError(f"Unsupported method: '{name}'")
 
-    meth = make_method_from_name(name, alpha)
-    eoc = EOCRecorder(order=meth.order)
+    eoc = EOCRecorder(order=order)
 
     if visualize:
         import matplotlib.pyplot as mp
 
         fig = mp.figure()
         ax = fig.gca()
 
@@ -96,27 +111,26 @@
         eoc.add_data_point(h, e)
         logger.info("n %4d h %.5e e %.12e", n, h, e)
 
         if visualize:
             ax.plot(p.x[1:], df_num[1:])
             # ax.semilogy(p.x, abs(df_num - df_ref))
 
-    logger.info("\n%s", eoc)
+    logger.info("\n%s", stringify_eoc(eoc))
 
     if visualize:
         ax.plot(p.x[1:], df_ref[1:], "k--")
         ax.set_xlabel("$x$")
         ax.set_ylabel(rf"$D^{{{alpha}}}_C f$")
         # ax.set_ylim([1.0e-16, 1])
 
         filename = f"test_caputo_{meth.name}_{alpha}".replace(".", "_")
         savefig(fig, dirname / filename.lower())
 
-    assert eoc.order is not None
-    assert eoc.order - 0.25 < eoc.estimated_order < eoc.order + 0.25
+    assert order - 0.25 < eoc.estimated_order < order + 0.25
 
 
 # }}}
 
 
 # {{{ test_caputo_spectral
 
@@ -136,24 +150,19 @@
 def test_caputo_spectral(
     j_alpha: float,
     j_beta: float,
     alpha: float,
     *,
     visualize: bool = False,
 ) -> None:
-    from pycaputo.derivatives import CaputoDerivative, Side
-    from pycaputo.differentiation import CaputoSpectralMethod
     from pycaputo.grid import make_jacobi_gauss_lobatto_points
-
-    d = CaputoDerivative(alpha, side=Side.Left)
-    meth = CaputoSpectralMethod(d)
-
     from pycaputo.utils import EOCRecorder, savefig
 
-    eoc = EOCRecorder(order=meth.order)
+    meth = caputo.SpectralJacobi(alpha=alpha)
+    eoc = EOCRecorder()
 
     if visualize:
         import matplotlib.pyplot as mp
 
         fig = mp.figure()
         ax = fig.gca()
 
@@ -194,125 +203,110 @@
 # }}}
 
 
 # {{{ test_caputo_vs_differint
 
 
 @dataclass(frozen=True)
-class DifferIntCaputoL1Method(CaputoDerivativeMethod):
-    @property
-    def order(self) -> float:
-        return 2 - self.d.order
+class DifferIntCaputoL1(caputo.CaputoDerivativeMethod):
+    pass
 
 
-@diff.register(DifferIntCaputoL1Method)
-def _diff_differint_l1(
-    m: DifferIntCaputoL1Method, f: ScalarFunction, p: Points
-) -> Array:
+@diff.register(DifferIntCaputoL1)
+def _diff_differint_l1(m: DifferIntCaputoL1, f: ScalarFunction, p: Points) -> Array:
     from differint.differint import CaputoL1point
 
     df = np.empty_like(p.x)
     df[0] = np.nan
 
     for n in range(1, df.size):
         df[n] = CaputoL1point(
-            m.d.order,
+            m.alpha,
             f,
             domain_start=p.a,
             domain_end=p.x[n],
             num_points=n + 1,
         )
 
     return df
 
 
 @dataclass(frozen=True)
-class DifferIntCaputoL2Method(CaputoDerivativeMethod):
-    @property
-    def order(self) -> float:
-        return 3 - self.d.order
+class DifferIntCaputoL2(caputo.CaputoDerivativeMethod):
+    pass
 
 
-@diff.register(DifferIntCaputoL2Method)
-def _diff_differint_l2(
-    m: DifferIntCaputoL2Method, f: ScalarFunction, p: Points
-) -> Array:
+@diff.register(DifferIntCaputoL2)
+def _diff_differint_l2(m: DifferIntCaputoL2, f: ScalarFunction, p: Points) -> Array:
     from differint.differint import CaputoL2point
 
     df = np.empty_like(p.x)
     df[0] = np.nan
 
     for n in range(1, df.size):
         df[n] = CaputoL2point(
-            m.d.order,
+            m.alpha,
             f,
             domain_start=p.a,
             domain_end=p.x[n],
             num_points=n + 1,
         )
 
     return df
 
 
 @dataclass(frozen=True)
-class DifferIntCaputoL2CMethod(CaputoDerivativeMethod):
-    @property
-    def order(self) -> float:
-        return 3 - self.d.order
+class DifferIntCaputoL2C(caputo.CaputoDerivativeMethod):
+    pass
 
 
-@diff.register(DifferIntCaputoL2CMethod)
-def _diff_differint_l2c(
-    m: DifferIntCaputoL2CMethod, f: ScalarFunction, p: Points
-) -> Array:
+@diff.register(DifferIntCaputoL2C)
+def _diff_differint_l2c(m: DifferIntCaputoL2C, f: ScalarFunction, p: Points) -> Array:
     from differint.differint import CaputoL2Cpoint
 
     df = np.empty_like(p.x)
     df[0] = np.nan
 
     for n in range(2, df.size - 1):
         df[n] = CaputoL2Cpoint(
-            m.d.order,
+            m.alpha,
             f,
             domain_start=p.a,
             domain_end=p.x[n],
             num_points=n + 1,
         )
 
     return df
 
 
 @pytest.mark.xfail()
-@pytest.mark.parametrize(
-    ("name", "cls"),
-    [
-        ("CaputoL1Method", DifferIntCaputoL1Method),
-        ("CaputoL2Method", DifferIntCaputoL2Method),
-        ("CaputoL2CMethod", DifferIntCaputoL2CMethod),
-    ],
-)
+@pytest.mark.parametrize("name", ["L1", "L2", "L2C"])
 @pytest.mark.parametrize("alpha", [0.1, 0.5, 0.9])
 def test_caputo_vs_differint(
     name: str,
-    cls: type[CaputoDerivativeMethod],
     alpha: float,
     *,
     visualize: bool = False,
 ) -> None:
     pytest.importorskip("differint")
 
-    from pycaputo.differentiation import CaputoDerivativeMethod, make_method_from_name
-
-    if name in {"CaputoL2Method", "CaputoL2CMethod"}:
+    if name in {"L2", "L2C"}:
         alpha += 1
 
-    meth = make_method_from_name(name, alpha)
-    assert isinstance(meth, CaputoDerivativeMethod)
-
-    differint_meth = cls(d=meth.d)
+    if name == "L1":
+        meth: caputo.CaputoDerivativeMethod = caputo.L1(alpha=alpha)
+        differint_meth: caputo.CaputoDerivativeMethod = DifferIntCaputoL1(alpha=alpha)
+    elif name == "L2":
+        meth = caputo.L2(alpha=alpha)
+        differint_meth = DifferIntCaputoL2(alpha=alpha)
+    elif name == "L2C":
+        meth = caputo.L2C(alpha=alpha)
+        differint_meth = DifferIntCaputoL2C(alpha=alpha)
+    else:
+        raise ValueError(f"Unknown method: '{name}'")
 
     from pycaputo.grid import make_points_from_name
 
     p = make_points_from_name("uniform", 512, a=0.0, b=0.5)
 
     df_ref = df_test(p.x, alpha=alpha)
     df_num = diff(meth, f_test, p)
```

### Comparing `pycaputo-0.5.0/tests/test_diff_riemann_liouville.py` & `pycaputo-0.6.0/tests/test_diff_riemann_liouville.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 import pathlib
 
 import numpy as np
 import numpy.linalg as la
 import pytest
 
-from pycaputo.derivatives import RiemannLiouvilleDerivative, Side
-from pycaputo.differentiation import diff
+from pycaputo.differentiation import diff, riemann_liouville
 from pycaputo.logging import get_logger
 from pycaputo.utils import Array, set_recommended_matplotlib
 
 logger = get_logger("pycaputo.test_diff_riemann_liouville")
 set_recommended_matplotlib()
 
 
@@ -50,39 +49,49 @@
 
     raise ValueError(f"Unsupported order: {alpha}")
 
 
 @pytest.mark.parametrize(
     ("name", "grid_type"),
     [
-        ("RiemannLiouvilleL1Method", "stretch"),
-        ("RiemannLiouvilleL1Method", "uniform"),
-        ("RiemannLiouvilleL2Method", "uniform"),
-        ("RiemannLiouvilleL2CMethod", "uniform"),
+        ("L1", "stretch"),
+        ("L1", "uniform"),
+        ("L2", "uniform"),
+        ("L2C", "uniform"),
     ],
 )
 @pytest.mark.parametrize("alpha", [0.1, 0.25, 0.5, 0.75, 0.9])
 def test_riemann_liouville_lmethods(
     name: str,
     grid_type: str,
     alpha: float,
     *,
     visualize: bool = False,
 ) -> None:
-    from pycaputo.differentiation import make_method_from_name
     from pycaputo.grid import make_points_from_name
 
-    if name in {"RiemannLiouvilleL2Method", "RiemannLiouvilleL2CMethod"}:
+    if name in {"L2", "L2C"}:
         alpha += 1
 
+    meth: riemann_liouville.RiemannLiouvilleDerivativeMethod
+    if name == "L1":
+        meth = riemann_liouville.L1(alpha=alpha)
+        order = 2.0 - alpha
+    elif name == "L2":
+        meth = riemann_liouville.L2(alpha=alpha)
+        order = 1.0
+    elif name == "L2C":
+        meth = riemann_liouville.L2C(alpha=alpha)
+        order = 3.0 - alpha
+    else:
+        raise ValueError(f"Unsupported method: {name}")
+
     from pycaputo.utils import EOCRecorder, savefig
 
-    d = RiemannLiouvilleDerivative(alpha, Side.Left)
-    meth = make_method_from_name(name, d)
-    eoc = EOCRecorder(order=meth.order)
+    eoc = EOCRecorder(order=order)
 
     if visualize:
         import matplotlib.pyplot as mp
 
         fig = mp.figure()
         ax = fig.gca()
 
@@ -110,12 +119,11 @@
 
         dirname = pathlib.Path(__file__).parent
         filename = f"test_rl_{meth.name}_{alpha}".replace(".", "_")
         savefig(fig, dirname / filename.lower())
 
     # FIXME: the L2 methods do not behave as expected, but they're doing better
     # so maybe shouldn't complain too much
-    assert eoc.order is not None
-    assert eoc.order - 0.25 < eoc.estimated_order < eoc.order + 1.5
+    assert order - 0.25 < eoc.estimated_order < order + 1.5
 
 
 # }}}
```

### Comparing `pycaputo-0.5.0/tests/test_finite_difference.py` & `pycaputo-0.6.0/tests/test_finite_difference.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_fode.py` & `pycaputo-0.6.0/tests/test_fode.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_fode_caputo.py` & `pycaputo-0.6.0/tests/test_fode_caputo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Alexandru Fikl <alexfikl@gmail.com>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import pathlib
+from dataclasses import replace
 from functools import partial
 from typing import Any, Callable
 
 import numpy as np
 import numpy.linalg as la
 import pytest
 
@@ -62,21 +63,22 @@
 def garrappa2009_source_jac(t: float, y: Array, *, alpha: float) -> Array:
     return -np.ones_like(y)
 
 
 # }}}
 
 
-# {{{ test_caputo_fode
+# {{{ test_fode_caputo
 
 
 def fode_factory(
     cls: type[FractionalDifferentialEquationMethod[StateFunction]],
     *,
     wrap: bool = True,
+    graded: bool = False,
     **kwargs: Any,
 ) -> Any:
     nterms = kwargs.pop("nterms", 1)
     y0 = np.concatenate([garrappa2009_solution(0.0) for _ in range(nterms)])
     tspan = (0.0, 1.0)
 
     from dataclasses import fields
@@ -103,19 +105,31 @@
 
         assert len(alpha) == nterms
         dt = (tspan[1] - tspan[0]) / n
 
         if has_source_jac:
             kwargs["source_jac"] = partial(source_jac, alpha=alpha)
 
-        from pycaputo.controller import make_fixed_controller
+        from pycaputo.controller import (
+            Controller,
+            make_fixed_controller,
+            make_graded_controller,
+        )
+
+        control: Controller
+        if graded:
+            control = make_graded_controller(
+                dt, tstart=tspan[0], tfinal=tspan[1], alpha=max(alpha)
+            )
+        else:
+            control = make_fixed_controller(dt, tstart=tspan[0], tfinal=tspan[1])
 
         return cls(
             derivative_order=alpha,
-            control=make_fixed_controller(dt, tstart=tspan[0], tfinal=tspan[1]),
+            control=control,
             source=partial(source, alpha=alpha),
             y0=(y0,),
             **kwargs,
         )
 
     if wrap:
         return pytest.param(wrapper, id=cls.__name__)
@@ -125,23 +139,25 @@
 
 @pytest.mark.parametrize(
     "factory",
     [
         fode_factory(caputo.ForwardEuler),
         fode_factory(caputo.WeightedEuler, theta=0.0),
         fode_factory(caputo.WeightedEuler, theta=0.5),
+        fode_factory(caputo.Trapezoidal),
+        fode_factory(caputo.ExplicitTrapezoidal),
         fode_factory(caputo.PECE, corrector_iterations=1),
         # FIXME: this does not converge to the correct order with one iteration
         fode_factory(caputo.PEC, corrector_iterations=2),
         fode_factory(caputo.ModifiedPECE, corrector_iterations=1),
         fode_factory(caputo.L1),
     ],
 )
 @pytest.mark.parametrize("alpha", [0.1, 0.5, 0.9])
-def test_caputo_fode(
+def test_fode_caputo(
     factory: Callable[
         [float, int], FractionalDifferentialEquationMethod[StateFunction]
     ],
     alpha: float,
     *,
     visualize: bool = False,
 ) -> None:
@@ -151,73 +167,76 @@
     eoc = EOCRecorder()
     if not callable(factory):
         # NOTE: this is a pytest.param and we take out the callable
         factory = factory.values[0]
 
     for n in [32, 64, 128, 256, 512]:
         m = factory(alpha, n)
+        dtinit = getattr(m.control, "dt", None)
 
         with BlockTimer(name=m.name) as bt:
             ts = []
             ys = []
-            for event in evolve(m):
+            for event in evolve(m, dtinit=dtinit):
                 if isinstance(event, StepFailed):
                     raise ValueError("Step update failed")
                 elif isinstance(event, StepCompleted):
                     ts.append(event.t)
                     ys.append(event.y)
 
         dt = np.max(np.diff(np.array(ts)))
 
         y_ref = garrappa2009_solution(ts[-1])
         error = la.norm(ys[-1] - y_ref) / la.norm(y_ref)
         logger.info("dt %.5f error %.12e (%s)", dt, error, bt)
 
         eoc.add_data_point(dt, error)
 
-    from dataclasses import replace
-
     eoc = replace(eoc, order=m.order)
     logger.info("\n%s", eoc)
 
     if visualize:
         t = np.array(ts)
         y = np.array(ys).squeeze()
         y_ref = np.array([garrappa2009_solution(ti) for ti in t]).squeeze()
 
         from pycaputo.utils import figure
 
         dirname = pathlib.Path(__file__).parent
-        filename = f"test_caputo_fode_{m.name}_{alpha}".replace(".", "_").lower()
+        filename = f"test_fode_caputo_{m.name}_{alpha}".replace(".", "_").lower()
         with figure(dirname / filename) as fig:
             ax = fig.gca()
 
             ax.plot(t, y, label=f"{m.name}")
             ax.plot(t, y_ref, "k--", label="Reference")
             ax.set_xlabel("$t$")
             ax.set_ylabel("$y$")
             ax.legend()
 
+    if alpha < 0.5 and isinstance(m, caputo.ExplicitTrapezoidal):
+        # FIXME: this seems unstable for some reason
+        return
+
     assert eoc.estimated_order > m.order - 0.25
 
 
 # }}}
 
 
-# {{{ test_caputo_fode_system
+# {{{ test_fode_caputo_system
 
 
 @pytest.mark.parametrize(
     "factory",
     [
         fode_factory(caputo.ForwardEuler, nterms=3),
         fode_factory(caputo.WeightedEuler, theta=0.5, nterms=3),
     ],
 )
-def test_caputo_fode_system(
+def test_fode_caputo_system(
     factory: Callable[
         [tuple[float, ...], int], FractionalDifferentialEquationMethod[StateFunction]
     ],
     *,
     visualize: bool = False,
 ) -> None:
     from pycaputo.events import StepCompleted, StepFailed
@@ -246,24 +265,102 @@
 
         y_ref = garrappa2009_solution(ts[-1])
         error = la.norm(ys[-1] - y_ref) / la.norm(y_ref)
         logger.info("dt %.5f error %.12e (%s)", dt, error, bt)
 
         eoc.add_data_point(dt, error)
 
-    from dataclasses import replace
-
     eoc = replace(eoc, order=m.order)
     logger.info("\n%s", eoc)
 
     assert eoc.estimated_order > m.order - 0.25
 
 
 # }}}
 
+
+# {{{ test_caputo_l1_convergence
+
+
+def singular_solution(t: float, *, alpha: float) -> Array:
+    return np.array([t**alpha])
+
+
+def singular_source(t: float, y: Array, *, alpha: float) -> Array:
+    from math import gamma
+
+    return np.array([gamma(1 + alpha)])
+
+
+@pytest.mark.parametrize("mesh_type", ["uniform", "graded"])
+@pytest.mark.parametrize("alpha", [0.1, 0.5, 0.9])
+def test_singular_caputo_l1(
+    mesh_type: str, alpha: float, *, visualize: bool = False
+) -> None:
+    from pycaputo.events import StepCompleted, StepFailed
+    from pycaputo.utils import BlockTimer, EOCRecorder
+
+    if mesh_type == "uniform":
+        order = 1.0
+    elif mesh_type == "graded":
+        order = 2.0 - alpha
+    else:
+        raise ValueError(f"Unknown mesh type: {mesh_type}")
+
+    eoc = EOCRecorder(order=order)
+    graded = mesh_type == "graded"
+
+    for n in [32, 64, 128, 256, 512]:
+        m = fode_factory(caputo.L1, wrap=False, graded=graded)(alpha, n)
+        m = replace(m, source=partial(singular_source, alpha=alpha))
+
+        with BlockTimer(name=m.name) as bt:
+            ts = []
+            ys = []
+            for event in evolve(m):
+                if isinstance(event, StepFailed):
+                    raise ValueError("Step update failed")
+                elif isinstance(event, StepCompleted):
+                    ts.append(event.t)
+                    ys.append(event.y)
+
+        dt = np.max(np.diff(np.array(ts)))
+
+        y_ref = singular_solution(ts[-1], alpha=alpha)
+        error = la.norm(ys[-1] - y_ref) / la.norm(y_ref)
+        logger.info("dt %.5f error %.12e (%s)", dt, error, bt)
+
+        eoc.add_data_point(dt, error)
+
+    logger.info("\n%s", eoc)
+
+    if visualize:
+        t = np.array(ts)
+        y = np.array(ys).squeeze()
+        y_ref = np.array([singular_solution(ti, alpha=alpha) for ti in t]).squeeze()
+
+        from pycaputo.utils import figure
+
+        dirname = pathlib.Path(__file__).parent
+        filename = f"test_fode_caputo_{m.name}_{alpha}_sing".replace(".", "_").lower()
+        with figure(dirname / filename) as fig:
+            ax = fig.gca()
+
+            ax.plot(t, y, label=f"{m.name}")
+            ax.plot(t, y_ref, "k--", label="Reference")
+            ax.set_xlabel("$t$")
+            ax.set_ylabel("$y$")
+            ax.legend()
+
+    assert order - 0.2 < eoc.estimated_order < order + 0.2
+
+
+# }}}
+
+
 if __name__ == "__main__":
     import sys
 
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         pytest.main([__file__])
```

### Comparing `pycaputo-0.5.0/tests/test_generating_functions.py` & `pycaputo-0.6.0/tests/test_generating_functions.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_integrate_fire.py` & `pycaputo-0.6.0/tests/test_integrate_fire.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_interpolation.py` & `pycaputo-0.6.0/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_jacobi.py` & `pycaputo-0.6.0/tests/test_jacobi.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_misc.py` & `pycaputo-0.6.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/test_mittag_leffler.py` & `pycaputo-0.6.0/tests/test_mittag_leffler.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,102 +13,90 @@
 from pycaputo.utils import set_recommended_matplotlib
 
 dirname = pathlib.Path(__file__).parent
 logger = get_logger("pycaputo.test_mittag_leffler")
 set_recommended_matplotlib()
 
 
-# {{{ test_mittag_leffler_series
+# {{{ test_mittag_leffler_special
 
 
 @pytest.mark.parametrize(
     ("alpha", "beta"),
     [
         (0, 1),
         (0, 3),
         (1, 1),
-        (2, 1),
+        # FIXME: typo?
+        # (2, 1),
         (3, 1),
         (4, 1),
         (0.5, 1),
         (1, 2),
         (2, 2),
     ],
 )
-def test_mittag_leffler_series(alpha: float, beta: float) -> None:
-    rng = np.random.default_rng(seed=42)
-    z = rng.random(128)
-
-    result_ref = ml.mittag_leffler(z, alpha=alpha, beta=beta)
-    result = np.vectorize(
-        lambda zi: 0j + ml.mittag_leffler_series(zi, alpha=alpha, beta=beta)
-    )(z)
-
-    error = np.linalg.norm(result - result_ref) / (1 + np.linalg.norm(result_ref))
-    logger.info("Error E[%g, %g]: %.12e", alpha, beta, error)
-    assert error < 2.0e-15
-
-
-# }}}
-
-
-# {{{ test_mittag_leffler_diethelm
-
-
 @pytest.mark.parametrize(
-    ("alpha", "beta"),
+    "alg",
     [
-        (0, 1),
-        (0, 3),
-        (1, 1),
-        # FIXME: typo?
-        # (2, 1),
-        (3, 1),
-        (4, 1),
-        (0.5, 1),
-        (1, 2),
-        (2, 2),
+        ml.Algorithm.Series,
+        ml.Algorithm.Diethelm,
+        ml.Algorithm.Garrappa,
     ],
 )
-def test_mittag_leffler_diethelm(alpha: float, beta: float) -> None:
-    rng = np.random.default_rng(seed=42)
-    z = rng.random(128)
+def test_mittag_leffler_special(alpha: float, beta: float, alg: ml.Algorithm) -> None:
+    rng = np.random.default_rng(seed=None)
+
+    z = rng.uniform(-4.0, 5.0, 128) + 1j * rng.uniform(-5.0, 4.0, 128)
+    if alpha == 0 or alg == ml.Algorithm.Series:
+        z = z / (np.max(np.abs(z)) + 0.5)
 
-    result_ref = ml.mittag_leffler(z, alpha=alpha, beta=beta)
-    result = np.vectorize(
-        lambda zi: 0j + ml.mittag_leffler_diethelm(zi, alpha=alpha, beta=beta)
-    )(z)
+    if alpha == 0 and alg == ml.Algorithm.Garrappa:
+        pytest.skip("Garrappa algorithm does not handle alpha == 0")
 
+    result_ref = ml.mittag_leffler_special(z, alpha=alpha, beta=beta)
+    assert result_ref is not None
+
+    result = ml.mittag_leffler(z, alpha=alpha, beta=beta, alg=alg, use_explicit=False)
     error = np.linalg.norm(result - result_ref) / (1 + np.linalg.norm(result_ref))
     logger.info("Error E[%g, %g]: %.12e", alpha, beta, error)
 
     # NOTE: due to the numerical quadrature, this can fail sometimes
-    assert error < 2.0e-11
+    rtol = 7.0e-11 if alg == ml.Algorithm.Diethelm else 1.0e-14
+    assert error < rtol
 
 
 # }}}
 
 
 # {{{ test_mittag_leffler_mathematica
 
 
 @pytest.mark.parametrize("iref", [0, 1, 2, 3, 4])
-@pytest.mark.parametrize("alg", [ml.Algorithm.Series, ml.Algorithm.Diethelm])
+@pytest.mark.parametrize(
+    "alg",
+    [
+        ml.Algorithm.Series,
+        ml.Algorithm.Diethelm,
+        ml.Algorithm.Garrappa,
+    ],
+)
 def test_mittag_leffler_mathematica(iref: int, alg: ml.Algorithm) -> None:
     from mittag_leffler_ref import MATHEMATICA_RESULTS
 
     ref = MATHEMATICA_RESULTS[iref]
     is_on_unit_disk = np.all(np.abs(ref.z) <= 1.0)
 
     if alg == ml.Algorithm.Series and not is_on_unit_disk:
         pytest.skip("Series representation is not valid for z >= 1")
 
-    result = ml.mittag_leffler(ref.z, alpha=ref.alpha, beta=ref.beta)
+    result = ml.mittag_leffler(ref.z, alpha=ref.alpha, beta=ref.beta, alg=alg)
     error = np.linalg.norm(result - ref.result) / np.linalg.norm(ref.result)
     logger.info("Error E[%g, %g]: %.12e", ref.alpha, ref.beta, error)
+    # logger.info("Expected %s Result %s", ref.result, result)
     assert error < 1.0e-5
 
 
 # }}}
 
 
 # {{{ test_mittag_leffler_opt
@@ -190,14 +178,51 @@
             ax.plot(t, f)
             ax.plot(result.root, fstar, "ro", ms=10)
 
 
 # }}}
 
 
+# {{{ test_mittag_leffler_sine_mathematica
+
+
+@pytest.mark.parametrize("iref", [0, 1])
+@pytest.mark.parametrize(
+    "alg", [ml.Algorithm.Series, ml.Algorithm.Diethelm, ml.Algorithm.Garrappa]
+)
+def test_mittag_leffler_sine_mathematica(
+    iref: int, alg: ml.Algorithm, *, visualize: bool = False
+) -> None:
+    from mittag_leffler_ref import MATHEMATICA_SINE_RESULTS
+
+    ref = MATHEMATICA_SINE_RESULTS[iref]
+
+    result = ml.caputo_derivative_sine(ref.z, alpha=ref.alpha, alg=alg)
+    error = np.linalg.norm(result - ref.result) / np.linalg.norm(ref.result)
+    logger.info("Error D^%g[sin]: %.12e", ref.alpha, error)
+
+    if visualize:
+        from pycaputo.utils import figure
+
+        i = np.argsort(ref.z)
+
+        suffix = str(ref.alpha).replace(".", "_")
+        with figure(dirname / f"test_mittag_leffler_sine_{suffix}") as fig:
+            ax = fig.gca()
+            ax.semilogy(ref.z[i], np.abs(result[i] - ref.result[i]))
+
+            ax.set_xlabel("$t$")
+            ax.set_ylabel("$D[sin]$")
+
+    assert error < 2.0e-11
+
+
+# }}}
+
+
 if __name__ == "__main__":
     import sys
 
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         pytest.main([__file__])
```

### Comparing `pycaputo-0.5.0/tests/test_points.py` & `pycaputo-0.6.0/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.5.0/tests/benchmarks/test_bench_diff.py` & `pycaputo-0.6.0/tests/benchmarks/test_bench_diff.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 import numpy as np
 import numpy.linalg as la
 import pytest
 from pytest_benchmark.fixture import BenchmarkFixture
 
+from pycaputo.differentiation import caputo, diff
 from pycaputo.utils import Array
 
 
 def func(x: Array, *, alpha: float) -> Array:
     return np.array(x**8 - 3 * x ** (4 + alpha / 2) + 9 / 4 * x**alpha)
 
 
@@ -27,32 +28,42 @@
     )
 
 
 @pytest.mark.benchmark(group="diff")
 @pytest.mark.parametrize(
     ("name", "grid_type"),
     [
-        ("CaputoL1", "stretch"),
-        ("CaputoL1", "uniform"),
-        ("CaputoL2", "uniform"),
-        ("CaputoL2C", "uniform"),
-        ("CaputoModifiedL1", "midpoints"),
+        ("L1", "stretch"),
+        ("L1", "uniform"),
+        ("L2", "uniform"),
+        ("L2C", "uniform"),
+        ("ModifiedL1", "midpoints"),
     ],
 )
 def test_caputo_diff(name: str, grid_type: str, benchmark: BenchmarkFixture) -> None:
-    from pycaputo.differentiation import diff, make_method_from_name
     from pycaputo.grid import make_points_from_name
 
     alpha = 0.9
     n = 1024
 
-    if name in {"CaputoL2", "CaputoL2C"}:
+    if name in {"L2", "L2C"}:
         alpha += 1
 
-    meth = make_method_from_name(f"{name}Method", alpha)
+    meth: caputo.CaputoDerivativeMethod
+    if name == "L1":
+        meth = caputo.L1(alpha=alpha)
+    elif name == "ModifiedL1":
+        meth = caputo.ModifiedL1(alpha=alpha)
+    elif name == "L2":
+        meth = caputo.L2(alpha=alpha)
+    elif name == "L2C":
+        meth = caputo.L2C(alpha=alpha)
+    else:
+        raise ValueError(f"Unsupported method: {name}")
+
     p = make_points_from_name(grid_type, n, a=0.0, b=1.0)
 
     f_test = func(p.x, alpha=alpha)
     df_ref = func_der_ref(p.x, alpha=alpha)
 
     def run_diff() -> None:
         for _ in range(32):
```

### Comparing `pycaputo-0.5.0/README.rst` & `pycaputo-0.6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-.. image:: https://github.com/alexfikl/pycaputo/workflows/CI/badge.svg
+.. |badge-ci| image:: https://github.com/alexfikl/pycaputo/workflows/CI/badge.svg
     :alt: Build Status
     :target: https://github.com/alexfikl/pycaputo/actions?query=branch%3Amain+workflow%3ACI
 
-.. image:: https://badge.fury.io/py/pycaputo.svg
+.. |badge-pypi| image:: https://badge.fury.io/py/pycaputo.svg
     :alt: PyPI
     :target: https://pypi.org/project/pycaputo/
 
-.. image:: https://readthedocs.org/projects/pycaputo/badge/?version=latest
+.. |badge-rtd| image:: https://readthedocs.org/projects/pycaputo/badge/?version=latest
     :alt: Documentation
     :target: https://pycaputo.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://api.reuse.software/badge/github.com/alexfikl/pycaputo
+.. |badge-reuse| image:: https://api.reuse.software/badge/github.com/alexfikl/pycaputo
     :alt: REUSE
     :target: https://api.reuse.software/info/github.com/alexfikl/pycaputo
 
+.. |badge-zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10996100.svg
+    :target: https://doi.org/10.5281/zenodo.10996100
+
+|badge-ci| |badge-pypi| |badge-rtd| |badge-reuse| |badge-zenodo|
+
 pycaputo
 ========
 
 This library can be used to evaluate fractional integrals and solve fractional ODEs.
 It is currently a testbed for various traditional methods, but hopefully
 development will continue and it will be a nice flexible library with support
 for many different types of fractional derivatives (and other related operators).
```

### Comparing `pycaputo-0.5.0/pyproject.toml` & `pycaputo-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,139 +2,144 @@
 build-backend = "hatchling.build"
 requires = [
     "hatchling>=1.10",
 ]
 
 [project]
 name = "pycaputo"
-version = "0.5.0"
+version = "0.6.0"
 description = "Evaluate fractional integrals and solve fractional ODEs"
 readme = "README.rst"
 keywords = [
     "fractional-derivatives",
     "fractional-integrals",
     "quadrature",
     "time-stepping",
 ]
 license = { text = "MIT" }
-maintainers = [{ name = "Alexandru Fikl", email = "alexfikl@gmail.com" }]
-authors = [{ name = "Alexandru Fikl", email = "alexfikl@gmail.com" }]
+maintainers = [
+    { name = "Alexandru Fikl", email = "alexfikl@gmail.com" },
+]
+authors = [
+    { name = "Alexandru Fikl", email = "alexfikl@gmail.com" },
+]
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
 dependencies = [
     "numpy>=1.17",
     "rich>=13",
     "scipy>=1.7",
-    'typing-extensions; python_version < "3.10"',
+    "typing-extensions; python_version<'3.10'",
 ]
-[project.optional-dependencies]
-dev = [
+optional-dependencies.dev = [
     "codespell",
     "differint",
     "doc8",
     "matplotlib",
     "mypy",
     "pyproject-fmt",
     "pytest",
     "pytest-benchmark",
     "reuse",
     "ruff",
     "types-dataclasses",
     "uv",
 ]
-docs = [
+optional-dependencies.docs = [
     "sphinx>=6",
     "sphinx-book-theme",
 ]
-vis = [
-    "SciencePlots",
+optional-dependencies.vis = [
+    "scienceplots",
 ]
-[project.urls]
-Documentation = "https://pycaputo.readthedocs.io"
-Repository = "https://github.com/alexfikl/pycaputo"
+urls.Documentation = "https://pycaputo.readthedocs.io"
+urls.Repository = "https://github.com/alexfikl/pycaputo"
 
 [tool.hatch.build.targets.sdist]
-exclude = [".github", ".ci", "docs/_build"]
+exclude = [
+    ".github",
+    ".ci",
+    "docs/_build",
+]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/pycaputo"]
+packages = [
+    "src/pycaputo",
+]
 
 [tool.ruff]
-preview = true
 target-version = "py38"
 line-length = 88
 
-[tool.ruff.lint]
-select = [
-    "A",        # flake8-builtins
-    "B",        # flake8-bugbear
-    "C4",       # flake8-comprehensions
-    "E",        # flake8
-    "F",        # flake8
-    "FBT",      # flake8-boolean-trap
-    "G",        # flake8-logging-format
-    "I",        # flake8-isort
-    "ISC",      # flake8-implicit-str-concat
-    "N",        # pep8-naming
-    "NPY",      # numpy
-    "PL",       # pylint
-    "PT",       # flake8-pytest-style
-    "Q",        # flake8-quotes
-    "RUF",      # ruff
-    "S",        # flake8-bandit
-    "SIM",      # flake8-simplify
-    "UP",       # pyupgrade
-    "W",        # flake8
-]
-ignore = [
-    "E203",     # whitespace-before-punctuation
-    "E402",     # module-import-not-at-top-of-file
-    "ISC001",   # single-line-implicit-string-concatenation
-    "N806",     # non-lowercase-variable-in-function
-    "N803",     # non-lowercase-argument
-    "PLC0415",  # import-outside-top-level
-    "PLC2801",  # unnecessary-dunder-call
-    "PLR0911",  # too-many-return-statements
-    "PLR0912",  # too-many-branches
-    "PLR0913",  # too-many-arguments
-    "PLR0914",  # too-many-locals
-    "PLR0915",  # too-many-statements
-    "PLR0917",  # too-many-positional
-    "PLR6301",  # no-self-use
-    "PLR6104",  # non-augmented-assignment
-    "PLR2004",  # magic-value-comparison
-    "S101",     # assert
-    "S102",     # exec-builtin
-    "UP037",    # quoted-annotation
-]
-
-[tool.ruff.lint.flake8-quotes]
-docstring-quotes = "double"
-inline-quotes = "double"
-multiline-quotes = "double"
-
-[tool.ruff.lint.isort]
-known-first-party = ["pycaputo"]
-force-wrap-aliases = true
+preview = true
+lint.select = [
+    "A",   # flake8-builtins
+    "B",   # flake8-bugbear
+    "C4",  # flake8-comprehensions
+    "E",   # flake8
+    "F",   # flake8
+    "FBT", # flake8-boolean-trap
+    "G",   # flake8-logging-format
+    "I",   # flake8-isort
+    "ISC", # flake8-implicit-str-concat
+    "N",   # pep8-naming
+    "NPY", # numpy
+    "PL",  # pylint
+    "PT",  # flake8-pytest-style
+    "Q",   # flake8-quotes
+    "RUF", # ruff
+    "S",   # flake8-bandit
+    "SIM", # flake8-simplify
+    "UP",  # pyupgrade
+    "W",   # flake8
+]
+lint.ignore = [
+    "E203",    # whitespace-before-punctuation
+    "E402",    # module-import-not-at-top-of-file
+    "ISC001",  # single-line-implicit-string-concatenation
+    "N803",    # non-lowercase-argument
+    "N806",    # non-lowercase-variable-in-function
+    "PLC0415", # import-outside-top-level
+    "PLC2801", # unnecessary-dunder-call
+    "PLR0911", # too-many-return-statements
+    "PLR0912", # too-many-branches
+    "PLR0913", # too-many-arguments
+    "PLR0914", # too-many-locals
+    "PLR0915", # too-many-statements
+    "PLR0917", # too-many-positional
+    "PLR2004", # magic-value-comparison
+    "PLR6104", # non-augmented-assignment
+    "PLR6301", # no-self-use
+    "S101",    # assert
+    "S102",    # exec-builtin
+    "UP037",   # quoted-annotation
+]
+
+lint.flake8-quotes.docstring-quotes = "double"
+lint.flake8-quotes.inline-quotes = "double"
+lint.flake8-quotes.multiline-quotes = "double"
+lint.isort.force-wrap-aliases = true
+lint.isort.known-first-party = [
+    "pycaputo",
+]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = [
     "-rswx",
     "--durations=25",
     "--capture=no",
```

### Comparing `pycaputo-0.5.0/PKG-INFO` & `pycaputo-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pycaputo
-Version: 0.5.0
+Version: 0.6.0
 Summary: Evaluate fractional integrals and solve fractional ODEs
 Project-URL: Documentation, https://pycaputo.readthedocs.io
 Project-URL: Repository, https://github.com/alexfikl/pycaputo
 Author-email: Alexandru Fikl <alexfikl@gmail.com>
 Maintainer-email: Alexandru Fikl <alexfikl@gmail.com>
 License: MIT
 Keywords: fractional-derivatives,fractional-integrals,quadrature,time-stepping
@@ -43,30 +43,35 @@
 Provides-Extra: docs
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx>=6; extra == 'docs'
 Provides-Extra: vis
 Requires-Dist: scienceplots; extra == 'vis'
 Description-Content-Type: text/x-rst
 
-.. image:: https://github.com/alexfikl/pycaputo/workflows/CI/badge.svg
+.. |badge-ci| image:: https://github.com/alexfikl/pycaputo/workflows/CI/badge.svg
     :alt: Build Status
     :target: https://github.com/alexfikl/pycaputo/actions?query=branch%3Amain+workflow%3ACI
 
-.. image:: https://badge.fury.io/py/pycaputo.svg
+.. |badge-pypi| image:: https://badge.fury.io/py/pycaputo.svg
     :alt: PyPI
     :target: https://pypi.org/project/pycaputo/
 
-.. image:: https://readthedocs.org/projects/pycaputo/badge/?version=latest
+.. |badge-rtd| image:: https://readthedocs.org/projects/pycaputo/badge/?version=latest
     :alt: Documentation
     :target: https://pycaputo.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://api.reuse.software/badge/github.com/alexfikl/pycaputo
+.. |badge-reuse| image:: https://api.reuse.software/badge/github.com/alexfikl/pycaputo
     :alt: REUSE
     :target: https://api.reuse.software/info/github.com/alexfikl/pycaputo
 
+.. |badge-zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10996100.svg
+    :target: https://doi.org/10.5281/zenodo.10996100
+
+|badge-ci| |badge-pypi| |badge-rtd| |badge-reuse| |badge-zenodo|
+
 pycaputo
 ========
 
 This library can be used to evaluate fractional integrals and solve fractional ODEs.
 It is currently a testbed for various traditional methods, but hopefully
 development will continue and it will be a nice flexible library with support
 for many different types of fractional derivatives (and other related operators).
```

