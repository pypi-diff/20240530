# Comparing `tmp/pymc-5.9.1.tar.gz` & `tmp/pymc-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.9.1.tar", last modified: Thu Oct 26 09:24:40 2023, max compression
+gzip compressed data, was "dist/pymc-5.9.2.tar", last modified: Sun Nov 12 10:35:05 2023, max compression
```

## Comparing `pymc-5.9.1.tar` & `pymc-5.9.2.tar`

### file list

```diff
@@ -1,142 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-10-26 09:24:26.000000 pymc-5.9.1/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-10-26 09:24:26.000000 pymc-5.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-26 09:24:26.000000 pymc-5.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    42347 2023-10-26 09:24:26.000000 pymc-5.9.1/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2023-10-26 09:24:26.000000 pymc-5.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-26 09:24:26.000000 pymc-5.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2023-10-26 09:24:40.000000 pymc-5.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2023-10-26 09:24:26.000000 pymc-5.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    81106 2023-10-26 09:24:26.000000 pymc-5.9.1/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (127)    19525 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)    16845 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9769 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (127)   118976 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    42280 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    46291 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    36266 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    95981 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11893 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38439 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (127)    49882 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    22038 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/order.py
--rw-r--r--   0 runner    (1001) docker     (127)    20066 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)    22591 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11909 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    41415 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14514 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/model/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87401 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/model/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model/transform/conditioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    40492 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29883 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    27566 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (127)    52619 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15599 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24432 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17591 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    27526 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (127)    36532 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    35815 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16976 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    28608 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58328 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37930 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-10-26 09:24:26.000000 pymc-5.9.1/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2023-10-26 09:24:39.000000 pymc-5.9.1/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-10-26 09:24:39.000000 pymc-5.9.1/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 09:24:39.000000 pymc-5.9.1/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-26 09:24:39.000000 pymc-5.9.1/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-26 09:24:39.000000 pymc-5.9.1/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-26 09:24:26.000000 pymc-5.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-26 09:24:26.000000 pymc-5.9.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 09:24:40.000000 pymc-5.9.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      833 2023-10-26 09:24:26.000000 pymc-5.9.1/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2023-10-26 09:24:26.000000 pymc-5.9.1/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-10-26 09:24:40.000000 pymc-5.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2653 2023-10-26 09:24:26.000000 pymc-5.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    81282 2023-10-26 09:24:26.000000 pymc-5.9.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-11-12 10:34:54.000000 pymc-5.9.2/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-12 10:34:54.000000 pymc-5.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-11-12 10:34:54.000000 pymc-5.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42347 2023-11-12 10:34:54.000000 pymc-5.9.2/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2023-11-12 10:34:54.000000 pymc-5.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-12 10:34:54.000000 pymc-5.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2023-11-12 10:35:05.000000 pymc-5.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2023-11-12 10:34:54.000000 pymc-5.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    81106 2023-11-12 10:34:54.000000 pymc-5.9.2/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19525 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16845 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9769 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118932 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42280 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46291 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36266 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95981 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11893 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38439 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49882 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22078 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22591 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11909 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13293 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/transform_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30589 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87041 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/model/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model/transform/conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40492 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29883 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27566 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52619 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15599 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24432 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17591 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27526 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36532 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35815 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16976 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28608 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58328 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37930 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-11-12 10:34:54.000000 pymc-5.9.2/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-12 10:35:05.000000 pymc-5.9.2/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-12 10:34:54.000000 pymc-5.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-12 10:34:54.000000 pymc-5.9.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:35:05.000000 pymc-5.9.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      833 2023-11-12 10:34:54.000000 pymc-5.9.2/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2023-11-12 10:34:54.000000 pymc-5.9.2/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-12 10:35:05.000000 pymc-5.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2653 2023-11-12 10:34:54.000000 pymc-5.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81282 2023-11-12 10:34:54.000000 pymc-5.9.2/versioneer.py
```

### Comparing `pymc-5.9.1/ARCHITECTURE.md` & `pymc-5.9.2/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/CODE_OF_CONDUCT.md` & `pymc-5.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/CONTRIBUTING.md` & `pymc-5.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/GOVERNANCE.md` & `pymc-5.9.2/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/LICENSE` & `pymc-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/PKG-INFO` & `pymc-5.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.9.1
+Version: 5.9.2
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.9.1/README.rst` & `pymc-5.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/RELEASE-NOTES.md` & `pymc-5.9.2/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/__init__.py` & `pymc-5.9.2/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/__init__.py` & `pymc-5.9.2/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/arviz.py` & `pymc-5.9.2/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/base.py` & `pymc-5.9.2/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/mcbackend.py` & `pymc-5.9.2/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/ndarray.py` & `pymc-5.9.2/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/backends/report.py` & `pymc-5.9.2/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/blocking.py` & `pymc-5.9.2/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/data.py` & `pymc-5.9.2/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/__init__.py` & `pymc-5.9.2/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/bound.py` & `pymc-5.9.2/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/censored.py` & `pymc-5.9.2/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/continuous.py` & `pymc-5.9.2/pymc/distributions/continuous.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,25 +660,24 @@
 
     rv_op = truncated_normal
     bound_args_indices = (5, 6)  # indexes for lower and upper args
 
     @classmethod
     def dist(
         cls,
-        mu: Optional[DIST_PARAMETER_TYPES] = None,
+        mu: Optional[DIST_PARAMETER_TYPES] = 0,
         sigma: Optional[DIST_PARAMETER_TYPES] = None,
         *,
         tau: Optional[DIST_PARAMETER_TYPES] = None,
         lower: Optional[DIST_PARAMETER_TYPES] = None,
         upper: Optional[DIST_PARAMETER_TYPES] = None,
         **kwargs,
     ) -> RandomVariable:
         tau, sigma = get_tau_sigma(tau=tau, sigma=sigma)
         sigma = pt.as_tensor_variable(sigma)
-        tau = pt.as_tensor_variable(tau)
         mu = pt.as_tensor_variable(floatX(mu))
 
         lower = pt.as_tensor_variable(floatX(lower)) if lower is not None else pt.constant(-np.inf)
         upper = pt.as_tensor_variable(floatX(upper)) if upper is not None else pt.constant(np.inf)
         return super().dist([mu, sigma, lower, upper], **kwargs)
 
     def moment(rv, size, mu, sigma, lower, upper):
```

### Comparing `pymc-5.9.1/pymc/distributions/discrete.py` & `pymc-5.9.2/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/dist_math.py` & `pymc-5.9.2/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/distribution.py` & `pymc-5.9.2/pymc/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/mixture.py` & `pymc-5.9.2/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/multivariate.py` & `pymc-5.9.2/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/shape_utils.py` & `pymc-5.9.2/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/simulator.py` & `pymc-5.9.2/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/timeseries.py` & `pymc-5.9.2/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/transforms.py` & `pymc-5.9.2/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/distributions/truncated.py` & `pymc-5.9.2/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/exceptions.py` & `pymc-5.9.2/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/func_utils.py` & `pymc-5.9.2/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/__init__.py` & `pymc-5.9.2/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/cov.py` & `pymc-5.9.2/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/gp.py` & `pymc-5.9.2/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/hsgp_approx.py` & `pymc-5.9.2/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/mean.py` & `pymc-5.9.2/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/gp/util.py` & `pymc-5.9.2/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/initial_point.py` & `pymc-5.9.2/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/__init__.py` & `pymc-5.9.2/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/abstract.py` & `pymc-5.9.2/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/basic.py` & `pymc-5.9.2/pymc/logprob/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     MeasurableVariable,
     _icdf_helper,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
 )
 from pymc.logprob.rewriting import cleanup_ir, construct_ir_fgraph
-from pymc.logprob.transforms import RVTransform, TransformValuesRewrite
+from pymc.logprob.transform_value import TransformValuesRewrite
+from pymc.logprob.transforms import RVTransform
 from pymc.logprob.utils import find_rvs_in_graph, rvs_to_value_vars
 
 TensorLike: TypeAlias = Union[Variable, float, np.ndarray]
 
 
 def _find_unallowed_rvs_in_graph(graph):
     from pymc.data import MinibatchIndexRV
```

### Comparing `pymc-5.9.1/pymc/logprob/binary.py` & `pymc-5.9.2/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/censoring.py` & `pymc-5.9.2/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/checks.py` & `pymc-5.9.2/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/cumsum.py` & `pymc-5.9.2/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/mixture.py` & `pymc-5.9.2/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/order.py` & `pymc-5.9.2/pymc/logprob/order.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/rewriting.py` & `pymc-5.9.2/pymc/logprob/rewriting.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     SequenceDB,
     TopoDB,
 )
 from pytensor.tensor.basic import Alloc
 from pytensor.tensor.elemwise import DimShuffle, Elemwise
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
 from pytensor.tensor.rewriting.basic import register_canonicalize
+from pytensor.tensor.rewriting.math import local_exp_over_1_plus_exp
 from pytensor.tensor.rewriting.shape import ShapeFeature
 from pytensor.tensor.rewriting.uncanonicalize import local_max_and_argmax
 from pytensor.tensor.subtensor import (
     AdvancedIncSubtensor,
     AdvancedIncSubtensor1,
     AdvancedSubtensor,
     AdvancedSubtensor1,
@@ -355,15 +356,20 @@
 
     # Return the `RandomVariable` being indexed
     return [base_rv_var]
 
 
 logprob_rewrites_db = SequenceDB()
 logprob_rewrites_db.name = "logprob_rewrites_db"
+# Introduce sigmoid. We do it before canonicalization so that useless mul are removed next
+logprob_rewrites_db.register(
+    "local_exp_over_1_plus_exp", out2in(local_exp_over_1_plus_exp), "basic"
+)
 logprob_rewrites_db.register("pre-canonicalize", optdb.query("+canonicalize"), "basic")
+# Split max_and_argmax
 logprob_rewrites_db.register("local_max_and_argmax", out2in(local_max_and_argmax), "basic")
 
 # These rewrites convert un-measurable variables into their measurable forms,
 # but they need to be reapplied, because some of the measurable forms require
 # their inputs to be measurable.
 measurable_ir_rewrites_db = MeasurableEquilibriumDB()
 measurable_ir_rewrites_db.name = "measurable_ir_rewrites_db"
```

### Comparing `pymc-5.9.1/pymc/logprob/scan.py` & `pymc-5.9.2/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/tensor.py` & `pymc-5.9.2/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/logprob/transforms.py` & `pymc-5.9.2/pymc/logprob/transforms.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,31 +29,26 @@
 #   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
-
 import abc
 
-from copy import copy
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import pytensor.tensor as pt
 
 from pytensor import scan
-from pytensor.gradient import DisconnectedType, jacobian
-from pytensor.graph.basic import Apply, Node, Variable
-from pytensor.graph.features import AlreadyThere, Feature
+from pytensor.gradient import jacobian
+from pytensor.graph.basic import Node, Variable
 from pytensor.graph.fg import FunctionGraph
-from pytensor.graph.op import Op
-from pytensor.graph.replace import clone_replace
-from pytensor.graph.rewriting.basic import GraphRewriter, in2out, node_rewriter
+from pytensor.graph.rewriting.basic import node_rewriter
 from pytensor.scalar import (
     Abs,
     Add,
     ArcCosh,
     ArcSinh,
     ArcTanh,
     Cosh,
@@ -73,15 +68,14 @@
     Sigmoid,
     Sinh,
     Softplus,
     Sqr,
     Sqrt,
     Tanh,
 )
-from pytensor.scan.op import Scan
 from pytensor.tensor.exceptions import NotScalarConstantError
 from pytensor.tensor.math import (
     abs,
     add,
     arccosh,
     arcsinh,
     arctanh,
@@ -118,60 +112,18 @@
     _icdf,
     _icdf_helper,
     _logcdf,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
 )
-from pymc.logprob.rewriting import (
-    PreserveRVMappings,
-    cleanup_ir_rewrites_db,
-    measurable_ir_rewrites_db,
-)
+from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
 from pymc.logprob.utils import CheckParameterValue, check_potential_measurability
 
 
-class TransformedVariable(Op):
-    """A no-op that identifies a transform and its un-transformed input."""
-
-    view_map = {0: [0]}
-
-    def make_node(self, tran_value: TensorVariable, value: TensorVariable):
-        return Apply(self, [tran_value, value], [tran_value.type()])
-
-    def perform(self, node, inputs, outputs):
-        raise NotImplementedError("These `Op`s should be removed from graphs used for computation.")
-
-    def connection_pattern(self, node):
-        return [[True], [False]]
-
-    def infer_shape(self, fgraph, node, input_shapes):
-        return [input_shapes[0]]
-
-    def grad(self, args, g_outs):
-        return g_outs[0], DisconnectedType()()
-
-
-transformed_variable = TransformedVariable()
-
-
-@node_rewriter([TransformedVariable])
-def remove_TransformedVariables(fgraph, node):
-    if isinstance(node.op, TransformedVariable):
-        return [node.inputs[0]]
-
-
-cleanup_ir_rewrites_db.register(
-    "remove_TransformedVariables",
-    remove_TransformedVariables,
-    "cleanup",
-    "transform",
-)
-
-
 class RVTransform(abc.ABC):
     ndim_supp = None
 
     @abc.abstractmethod
     def forward(self, value: TensorVariable, *inputs: Variable) -> TensorVariable:
         """Apply the transformation."""
 
@@ -195,206 +147,14 @@
             phi_inv = self.backward(value, *inputs)
             return pt.log(pt.abs(pt.nlinalg.det(pt.atleast_2d(jacobian(phi_inv, [value])[0]))))
 
     def __str__(self):
         return f"{self.__class__.__name__}"
 
 
-@node_rewriter(tracks=None)
-def transform_values(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
-    """Apply transforms to value variables.
-
-    It is assumed that the input value variables correspond to forward
-    transformations, usually chosen in such a way that the values are
-    unconstrained on the real line.
-
-    For example, if ``Y = halfnormal(...)``, we assume the respective value
-    variable is specified on the log scale and back-transform it to obtain
-    ``Y`` on the natural scale.
-    """
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    values_to_transforms: Optional[TransformValuesMapping] = getattr(
-        fgraph, "values_to_transforms", None
-    )
-
-    if rv_map_feature is None or values_to_transforms is None:
-        return None  # pragma: no cover
-
-    rv_vars = []
-    value_vars = []
-
-    for out in node.outputs:
-        value = rv_map_feature.rv_values.get(out, None)
-        if value is None:
-            continue
-        rv_vars.append(out)
-        value_vars.append(value)
-
-    if not value_vars:
-        return None
-
-    transforms = [values_to_transforms.get(value_var, None) for value_var in value_vars]
-
-    if all(transform is None for transform in transforms):
-        return None
-
-    new_op = _create_transformed_rv_op(node.op, transforms)
-    # Create a new `Apply` node and outputs
-    trans_node = node.clone()
-    trans_node.op = new_op
-
-    # We now assume that the old value variable represents the *transformed space*.
-    # This means that we need to replace all instance of the old value variable
-    # with "inversely/un-" transformed versions of itself.
-    for rv_var, value_var, transform in zip(rv_vars, value_vars, transforms):
-        rv_var_out_idx = node.outputs.index(rv_var)
-
-        if transform is None:
-            continue
-
-        new_value_var = transformed_variable(
-            transform.backward(value_var, *trans_node.inputs), value_var
-        )
-
-        if value_var.name and getattr(transform, "name", None):
-            new_value_var.name = f"{value_var.name}_{transform.name}"
-
-        rv_map_feature.update_rv_maps(rv_var, new_value_var, trans_node.outputs[rv_var_out_idx])
-
-    return trans_node.outputs
-
-
-@node_rewriter(tracks=[Scan])
-def transform_scan_values(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
-    """Apply transforms to Scan value variables.
-
-    This specialized rewrite is needed because Scan replaces the original value variables
-    by a more complex graph. We want to apply the transform to the original value variable
-    in this subgraph, leaving the rest intact
-    """
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    values_to_transforms: Optional[TransformValuesMapping] = getattr(
-        fgraph, "values_to_transforms", None
-    )
-
-    if rv_map_feature is None or values_to_transforms is None:
-        return None  # pragma: no cover
-
-    rv_vars = []
-    value_vars = []
-
-    for out in node.outputs:
-        value = rv_map_feature.rv_values.get(out, None)
-        if value is None:
-            continue
-        rv_vars.append(out)
-        value_vars.append(value)
-
-    if not value_vars:
-        return None
-
-    transforms = [
-        values_to_transforms.get(rv_map_feature.original_values[value_var], None)
-        for value_var in value_vars
-    ]
-
-    if all(transform is None for transform in transforms):
-        return None
-
-    new_op = _create_transformed_rv_op(node.op, transforms)
-    trans_node = node.clone()
-    trans_node.op = new_op
-
-    # We now assume that the old value variable represents the *transformed space*.
-    # This means that we need to replace all instance of the old value variable
-    # with "inversely/un-" transformed versions of itself.
-    for rv_var, value_var, transform in zip(rv_vars, value_vars, transforms):
-        rv_var_out_idx = node.outputs.index(rv_var)
-
-        if transform is None:
-            continue
-
-        # We access the original value variable and apply the transform to that
-        original_value_var = rv_map_feature.original_values[value_var]
-        trans_original_value_var = transform.backward(original_value_var, *trans_node.inputs)
-
-        # We then replace the reference to the original value variable in the scan value
-        # variable by the back-transform projection computed above
-
-        # The first input corresponds to the original value variable. We are careful to
-        # only clone_replace that part of the graph, as we don't want to break the
-        # mappings between other rvs that are likely to be present in the rest of the
-        # scan value variable graph
-        # TODO: Is it true that the original value only appears in the first input
-        #  and that no other RV can appear there?
-        (trans_original_value_var,) = clone_replace(
-            (value_var.owner.inputs[0],),
-            replace={original_value_var: trans_original_value_var},
-        )
-        trans_value_var = value_var.owner.clone_with_new_inputs(
-            inputs=[trans_original_value_var] + value_var.owner.inputs[1:]
-        ).default_output()
-
-        new_value_var = transformed_variable(trans_value_var, original_value_var)
-
-        if value_var.name and getattr(transform, "name", None):
-            new_value_var.name = f"{value_var.name}_{transform.name}"
-
-        rv_map_feature.update_rv_maps(rv_var, new_value_var, trans_node.outputs[rv_var_out_idx])
-
-    return trans_node.outputs
-
-
-class TransformValuesMapping(Feature):
-    r"""A `Feature` that maintains a map between value variables and their transforms."""
-
-    def __init__(self, values_to_transforms):
-        self.values_to_transforms = values_to_transforms.copy()
-
-    def on_attach(self, fgraph):
-        if hasattr(fgraph, "values_to_transforms"):
-            raise AlreadyThere()
-
-        fgraph.values_to_transforms = self.values_to_transforms
-
-
-class TransformValuesRewrite(GraphRewriter):
-    r"""Transforms value variables according to a map."""
-
-    transform_rewrite = in2out(transform_values, ignore_newtrees=True)
-    scan_transform_rewrite = in2out(transform_scan_values, ignore_newtrees=True)
-
-    def __init__(
-        self,
-        values_to_transforms: Dict[TensorVariable, Union[RVTransform, None]],
-    ):
-        """
-        Parameters
-        ----------
-        values_to_transforms
-            Mapping between value variables and their transformations.  Each
-            value variable can be assigned one of `RVTransform`, or ``None``.
-            If a transform is not specified for a specific value variable it will
-            not be transformed.
-
-        """
-
-        self.values_to_transforms = values_to_transforms
-
-    def add_requirements(self, fgraph):
-        values_transforms_feature = TransformValuesMapping(self.values_to_transforms)
-        fgraph.attach_feature(values_transforms_feature)
-
-    def apply(self, fgraph: FunctionGraph):
-        self.transform_rewrite.rewrite(fgraph)
-        self.scan_transform_rewrite.rewrite(fgraph)
-
-
 class MeasurableTransform(MeasurableElemwise):
     """A placeholder used to specify a log-likelihood for a transformed measurable variable"""
 
     valid_scalar_types = (
         Exp,
         Log,
         Add,
@@ -1052,49 +812,105 @@
         args_fn
             Function that expects inputs of RandomVariable and returns the lower
             and upper bounds for the interval transformation. If one of these is
             None, the RV is considered to be unbounded on the respective edge.
         """
         self.args_fn = args_fn
 
-    def forward(self, value, *inputs):
-        a, b = self.args_fn(*inputs)
+    def get_a_and_b(self, inputs):
+        """Return interval bound values.
 
-        if a is not None and b is not None:
-            return pt.log(value - a) - pt.log(b - value)
-        elif a is not None:
-            return pt.log(value - a)
-        elif b is not None:
-            return pt.log(b - value)
+        Also returns two boolean variables indicating whether the transform is known to be statically bounded.
+        This is used to generate smaller graphs in the transform methods.
+        """
+        a, b = self.args_fn(*inputs)
+        lower_bounded, upper_bounded = True, True
+        if a is None:
+            a = -pt.inf
+            lower_bounded = False
+        if b is None:
+            b = pt.inf
+            upper_bounded = False
+        return a, b, lower_bounded, upper_bounded
+
+    def forward(self, value, *inputs):
+        a, b, lower_bounded, upper_bounded = self.get_a_and_b(inputs)
+
+        log_lower_distance = pt.log(value - a)
+        log_upper_distance = pt.log(b - value)
+
+        if lower_bounded and upper_bounded:
+            return pt.where(
+                pt.and_(pt.neq(a, -pt.inf), pt.neq(b, pt.inf)),
+                log_lower_distance - log_upper_distance,
+                pt.where(
+                    pt.neq(a, -pt.inf),
+                    log_lower_distance,
+                    pt.where(
+                        pt.neq(b, pt.inf),
+                        log_upper_distance,
+                        value,
+                    ),
+                ),
+            )
+        elif lower_bounded:
+            return log_lower_distance
+        elif upper_bounded:
+            return log_upper_distance
         else:
-            raise ValueError("Both edges of IntervalTransform cannot be None")
+            return value
 
     def backward(self, value, *inputs):
-        a, b = self.args_fn(*inputs)
+        a, b, lower_bounded, upper_bounded = self.get_a_and_b(inputs)
 
-        if a is not None and b is not None:
-            sigmoid_x = pt.sigmoid(value)
-            return sigmoid_x * b + (1 - sigmoid_x) * a
-        elif a is not None:
-            return pt.exp(value) + a
-        elif b is not None:
-            return b - pt.exp(value)
+        exp_value = pt.exp(value)
+        sigmoid_x = pt.sigmoid(value)
+        lower_distance = exp_value + a
+        upper_distance = b - exp_value
+
+        if lower_bounded and upper_bounded:
+            return pt.where(
+                pt.and_(pt.neq(a, -pt.inf), pt.neq(b, pt.inf)),
+                sigmoid_x * b + (1 - sigmoid_x) * a,
+                pt.where(
+                    pt.neq(a, -pt.inf),
+                    lower_distance,
+                    pt.where(
+                        pt.neq(b, pt.inf),
+                        upper_distance,
+                        value,
+                    ),
+                ),
+            )
+        elif lower_bounded:
+            return lower_distance
+        elif upper_bounded:
+            return upper_distance
         else:
-            raise ValueError("Both edges of IntervalTransform cannot be None")
+            return value
 
     def log_jac_det(self, value, *inputs):
-        a, b = self.args_fn(*inputs)
+        a, b, lower_bounded, upper_bounded = self.get_a_and_b(inputs)
 
-        if a is not None and b is not None:
+        if lower_bounded and upper_bounded:
             s = pt.softplus(-value)
-            return pt.log(b - a) - 2 * s - value
-        elif a is None and b is None:
-            raise ValueError("Both edges of IntervalTransform cannot be None")
-        else:
+
+            return pt.where(
+                pt.and_(pt.neq(a, -pt.inf), pt.neq(b, pt.inf)),
+                pt.log(b - a) - 2 * s - value,
+                pt.where(
+                    pt.or_(pt.neq(a, -pt.inf), pt.neq(b, pt.inf)),
+                    value,
+                    pt.zeros_like(value),
+                ),
+            )
+        elif lower_bounded or upper_bounded:
             return value
+        else:
+            return pt.zeros_like(value)
 
 
 class LogOddsTransform(RVTransform):
     name = "logodds"
 
     def backward(self, value, *inputs):
         return pt.expit(value)
@@ -1178,113 +994,7 @@
         for det_ in det_list:
             if det_.ndim > ndim0:
                 ndim_diff = det_.ndim - ndim0
                 det += det_.sum(axis=tuple(range(-ndim_diff, 0)))
             else:
                 det += det_
         return det
-
-
-def _create_transformed_rv_op(
-    rv_op: Op,
-    transforms: Union[RVTransform, Sequence[Union[None, RVTransform]]],
-    *,
-    cls_dict_extra: Optional[Dict] = None,
-) -> Op:
-    """Create a new transformed variable instance given a base `RandomVariable` `Op`.
-
-    This will essentially copy the `type` of the given `Op` instance, create a
-    copy of said `Op` instance and change it's `type` to the new one.
-
-    In the end, we have an `Op` instance that will map to a `RVTransform` while
-    also behaving exactly as it did before.
-
-    Parameters
-    ----------
-    rv_op
-        The `RandomVariable` for which we want to construct a `TransformedRV`.
-    transform
-        The `RVTransform` for `rv_op`.
-    cls_dict_extra
-        Additional class members to add to the constructed `TransformedRV`.
-
-    """
-
-    if not isinstance(transforms, Sequence):
-        transforms = (transforms,)
-
-    trans_names = [
-        getattr(transform, "name", "transformed") if transform is not None else "None"
-        for transform in transforms
-    ]
-    rv_op_type = type(rv_op)
-    rv_type_name = rv_op_type.__name__
-    cls_dict = rv_op_type.__dict__.copy()
-    rv_name = cls_dict.get("name", "")
-    if rv_name:
-        cls_dict["name"] = f"{rv_name}_{'_'.join(trans_names)}"
-    cls_dict["transforms"] = transforms
-
-    if cls_dict_extra is not None:
-        cls_dict.update(cls_dict_extra)
-
-    new_op_type = type(f"Transformed{rv_type_name}", (rv_op_type,), cls_dict)
-
-    MeasurableVariable.register(new_op_type)
-
-    @_logprob.register(new_op_type)
-    def transformed_logprob(op, values, *inputs, use_jacobian=True, **kwargs):
-        """Compute the log-likelihood graph for a `TransformedRV`.
-
-        We assume that the value variable was back-transformed to be on the natural
-        support of the respective random variable.
-        """
-        logprobs = _logprob(rv_op, values, *inputs, **kwargs)
-
-        if not isinstance(logprobs, Sequence):
-            logprobs = [logprobs]
-
-        # Handle jacobian
-        assert len(values) == len(logprobs) == len(op.transforms)
-        logprobs_jac = []
-        for value, transform, logp in zip(values, op.transforms, logprobs):
-            if transform is None:
-                logprobs_jac.append(logp)
-                continue
-
-            assert isinstance(value.owner.op, TransformedVariable)
-            original_forward_value = value.owner.inputs[1]
-            log_jac_det = transform.log_jac_det(original_forward_value, *inputs).copy()
-            # The jacobian determinant has less dims than the logp
-            # when a multivariate transform (like Simplex or Ordered) is applied to univariate distributions.
-            # In this case we have to reduce the last logp dimensions, as they are no longer independent
-            if log_jac_det.ndim < logp.ndim:
-                diff_ndims = logp.ndim - log_jac_det.ndim
-                logp = logp.sum(axis=np.arange(-diff_ndims, 0))
-            # This case is sometimes, but not always, trivial to accomodate depending on the "space rank" of the
-            # multivariate distribution. See https://proceedings.mlr.press/v130/radul21a.html
-            elif log_jac_det.ndim > logp.ndim:
-                raise NotImplementedError(
-                    f"Univariate transform {transform} cannot be applied to multivariate {rv_op}"
-                )
-            else:
-                # Check there is no broadcasting between logp and jacobian
-                if logp.type.broadcastable != log_jac_det.type.broadcastable:
-                    raise ValueError(
-                        f"The logp of {rv_op} and log_jac_det of {transform} are not allowed to broadcast together. "
-                        "There is a bug in the implementation of either one."
-                    )
-
-            if use_jacobian:
-                if value.name:
-                    log_jac_det.name = f"{value.name}_jacobian"
-                logprobs_jac.append(logp + log_jac_det)
-            else:
-                # We still want to use the reduced logp, even though the jacobian isn't included
-                logprobs_jac.append(logp)
-
-        return logprobs_jac
-
-    new_op = copy(rv_op)
-    new_op.__class__ = new_op_type
-
-    return new_op
```

### Comparing `pymc-5.9.1/pymc/logprob/utils.py` & `pymc-5.9.2/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/math.py` & `pymc-5.9.2/pymc/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,29 @@
 from pytensor.graph.basic import Apply
 from pytensor.graph.op import Op
 
 # pylint: disable=unused-import
 from pytensor.tensor import (
     abs,
     and_,
+    arccos,
+    arccosh,
+    arcsin,
+    arcsinh,
+    arctan,
+    arctanh,
     broadcast_to,
     ceil,
     clip,
     concatenate,
     constant,
     cos,
     cosh,
+    cumprod,
+    cumsum,
     dot,
     eq,
     erf,
     erfc,
     erfcinv,
     erfinv,
     exp,
@@ -55,16 +63,18 @@
     le,
     log,
     log1pexp,
     logaddexp,
     logsumexp,
     lt,
     matmul,
+    max,
     maximum,
     mean,
+    min,
     minimum,
     neq,
     ones,
     ones_like,
     or_,
     prod,
     sgn,
@@ -90,21 +100,29 @@
 from pymc.pytensorf import floatX, ix_, largest_common_dtype
 
 # pylint: enable=unused-import
 
 __all__ = [
     "abs",
     "and_",
+    "arccos",
+    "arccosh",
+    "arcsin",
+    "arcsinh",
+    "arctan",
+    "arctanh",
     "broadcast_to",
     "ceil",
     "clip",
     "concatenate",
     "constant",
     "cos",
     "cosh",
+    "cumprod",
+    "cumsum",
     "dot",
     "eq",
     "erf",
     "erfc",
     "erfcinv",
     "erfinv",
     "exp",
@@ -117,22 +135,25 @@
     "le",
     "log",
     "log1pexp",
     "logaddexp",
     "logsumexp",
     "lt",
     "matmul",
+    "max",
     "maximum",
     "mean",
+    "min",
     "minimum",
     "neq",
     "ones",
     "ones_like",
     "or_",
     "prod",
+    "round",
     "sgn",
     "sigmoid",
     "sin",
     "sinh",
     "sqr",
     "sqrt",
     "stack",
@@ -254,23 +275,28 @@
     ----------
     diags: 1D arrays
            The diagonals of matrices that are to be Kroneckered
     """
     return reduce(flat_outer, diags)
 
 
-def tround(*args, **kwargs):
+def round(*args, **kwargs):
     """
     Temporary function to silence round warning in PyTensor. Please remove
     when the warning disappears.
     """
     kwargs["mode"] = "half_to_even"
     return pt.round(*args, **kwargs)
 
 
+def tround(*args, **kwargs):
+    warnings.warn("tround is deprecated. Use round instead.")
+    return round(*args, **kwargs)
+
+
 def logdiffexp(a, b):
     """log(exp(a) - exp(b))"""
     return a + pt.log1mexp(b - a)
 
 
 def logdiffexp_numpy(a, b):
     """log(exp(a) - exp(b))"""
```

### Comparing `pymc-5.9.1/pymc/model/__init__.py` & `pymc-5.9.2/pymc/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/model/core.py` & `pymc-5.9.2/pymc/model/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1343,23 +1343,14 @@
         data = convert_observed_data(data).astype(rv_var.dtype)
 
         if data.ndim != rv_var.ndim:
             raise ShapeError(
                 "Dimensionality of data and RV don't match.", actual=data.ndim, expected=rv_var.ndim
             )
 
-        if pytensor.config.compute_test_value != "off":
-            test_value = getattr(rv_var.tag, "test_value", None)
-
-            if test_value is not None:
-                # We try to reuse the old test value
-                rv_var.tag.test_value = np.broadcast_to(test_value, rv_var.shape)
-            else:
-                rv_var.tag.test_value = data
-
         mask = getattr(data, "mask", None)
         if mask is not None:
             impute_message = (
                 f"Data in {rv_var} contains missing values and"
                 " will be automatically imputed from the"
                 " sampling distribution."
             )
```

### Comparing `pymc-5.9.1/pymc/model/fgraph.py` & `pymc-5.9.2/pymc/model/fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/model/transform/__init__.py` & `pymc-5.9.2/pymc/model/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/model/transform/basic.py` & `pymc-5.9.2/pymc/model/transform/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/model/transform/conditioning.py` & `pymc-5.9.2/pymc/model/transform/conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/model_graph.py` & `pymc-5.9.2/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/ode/__init__.py` & `pymc-5.9.2/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/ode/ode.py` & `pymc-5.9.2/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/ode/utils.py` & `pymc-5.9.2/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/plots/__init__.py` & `pymc-5.9.2/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/printing.py` & `pymc-5.9.2/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/pytensorf.py` & `pymc-5.9.2/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/__init__.py` & `pymc-5.9.2/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/forward.py` & `pymc-5.9.2/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/jax.py` & `pymc-5.9.2/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/mcmc.py` & `pymc-5.9.2/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/parallel.py` & `pymc-5.9.2/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling/population.py` & `pymc-5.9.2/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/sampling_jax.py` & `pymc-5.9.2/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/smc/__init__.py` & `pymc-5.9.2/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/smc/kernels.py` & `pymc-5.9.2/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/smc/sampling.py` & `pymc-5.9.2/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/stats/__init__.py` & `pymc-5.9.2/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/stats/convergence.py` & `pymc-5.9.2/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/stats/log_likelihood.py` & `pymc-5.9.2/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/__init__.py` & `pymc-5.9.2/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/arraystep.py` & `pymc-5.9.2/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/compound.py` & `pymc-5.9.2/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/__init__.py` & `pymc-5.9.2/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.9.2/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/hmc.py` & `pymc-5.9.2/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/integration.py` & `pymc-5.9.2/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/nuts.py` & `pymc-5.9.2/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.9.2/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/metropolis.py` & `pymc-5.9.2/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/slicer.py` & `pymc-5.9.2/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/step_methods/step_sizes.py` & `pymc-5.9.2/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/testing.py` & `pymc-5.9.2/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/tuning/__init__.py` & `pymc-5.9.2/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/tuning/scaling.py` & `pymc-5.9.2/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/tuning/starting.py` & `pymc-5.9.2/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/util.py` & `pymc-5.9.2/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/__init__.py` & `pymc-5.9.2/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/approximations.py` & `pymc-5.9.2/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/callbacks.py` & `pymc-5.9.2/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/inference.py` & `pymc-5.9.2/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/minibatch_rv.py` & `pymc-5.9.2/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/operators.py` & `pymc-5.9.2/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/opvi.py` & `pymc-5.9.2/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/stein.py` & `pymc-5.9.2/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/test_functions.py` & `pymc-5.9.2/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/variational/updates.py` & `pymc-5.9.2/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc/vartypes.py` & `pymc-5.9.2/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/pymc.egg-info/PKG-INFO` & `pymc-5.9.2/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.9.1
+Version: 5.9.2
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.9.1/pymc.egg-info/SOURCES.txt` & `pymc-5.9.2/pymc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 pymc/logprob/checks.py
 pymc/logprob/cumsum.py
 pymc/logprob/mixture.py
 pymc/logprob/order.py
 pymc/logprob/rewriting.py
 pymc/logprob/scan.py
 pymc/logprob/tensor.py
+pymc/logprob/transform_value.py
 pymc/logprob/transforms.py
 pymc/logprob/utils.py
 pymc/model/__init__.py
 pymc/model/core.py
 pymc/model/fgraph.py
 pymc/model/transform/__init__.py
 pymc/model/transform/basic.py
```

### Comparing `pymc-5.9.1/scripts/docker_container.sh` & `pymc-5.9.2/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/setup.py` & `pymc-5.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.9.1/versioneer.py` & `pymc-5.9.2/versioneer.py`

 * *Files identical despite different names*

