# Comparing `tmp/giotto_ph-0.2.3-cp39-cp39-win_amd64.whl.zip` & `tmp/giotto_ph-0.2.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,24 @@
-Zip file size: 406879 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      149 b- defN 24-May-30 00:14 gph/__init__.py
--rw-rw-rw-  2.0 fat      620 b- defN 24-May-30 00:14 gph/_version.py
--rw-rw-rw-  2.0 fat   139264 b- defN 24-May-30 00:18 gph/modules/gph_collapser.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   338944 b- defN 24-May-30 00:18 gph/modules/gph_ripser.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   343040 b- defN 24-May-30 00:18 gph/modules/gph_ripser_coeff.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       89 b- defN 24-May-30 00:14 gph/python/__init__.py
--rw-rw-rw-  2.0 fat    28880 b- defN 24-May-30 00:14 gph/python/ripser_interface.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-30 00:14 gph/python/test/__init__.py
--rw-rw-rw-  2.0 fat     2248 b- defN 24-May-30 00:14 gph/python/test/test_collapser.py
--rw-rw-rw-  2.0 fat    20115 b- defN 24-May-30 00:14 gph/python/test/test_ripser.py
--rw-rw-rw-  2.0 fat     3645 b- defN 24-May-30 00:14 gph/python/test/test_wrp.py
--rw-rw-rw-  2.0 fat    35868 b- defN 24-May-30 00:18 giotto_ph-0.2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2648 b- defN 24-May-30 00:18 giotto_ph-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-30 00:18 giotto_ph-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-May-30 00:18 giotto_ph-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1356 b- defN 24-May-30 00:18 giotto_ph-0.2.3.dist-info/RECORD
-16 files, 916970 bytes uncompressed, 404641 bytes compressed:  55.9%
+Zip file size: 555069 bytes, number of entries: 22
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 gph/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 giotto_ph.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 giotto_ph-0.2.4.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 gph/modules/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 gph/python/
+-rw-r--r--  2.0 unx      141 b- defN 24-May-30 08:00 gph/__init__.py
+-rw-r--r--  2.0 unx      598 b- defN 24-May-30 08:00 gph/_version.py
+-rwxr-xr-x  2.0 unx   545400 b- defN 24-May-30 08:00 gph/modules/gph_ripser.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   561784 b- defN 24-May-30 08:00 gph/modules/gph_ripser_coeff.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   208744 b- defN 24-May-30 08:00 gph/modules/gph_collapser.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 08:00 gph/python/test/
+-rw-r--r--  2.0 unx       84 b- defN 24-May-30 08:00 gph/python/__init__.py
+-rw-r--r--  2.0 unx    28232 b- defN 24-May-30 08:00 gph/python/ripser_interface.py
+-rw-r--r--  2.0 unx     3552 b- defN 24-May-30 08:00 gph/python/test/test_wrp.py
+-rw-r--r--  2.0 unx    19637 b- defN 24-May-30 08:00 gph/python/test/test_ripser.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 08:00 gph/python/test/__init__.py
+-rw-r--r--  2.0 unx     2181 b- defN 24-May-30 08:00 gph/python/test/test_collapser.py
+-rw-r--r--  2.0 unx      148 b- defN 24-May-30 08:00 giotto_ph-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx    35192 b- defN 24-May-30 08:00 giotto_ph-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx        4 b- defN 24-May-30 08:00 giotto_ph-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1409 b- defN 24-May-30 08:00 giotto_ph-0.2.4.dist-info/RECORD
+-rw-r--r--  2.0 unx    10398 b- defN 24-May-30 08:00 giotto_ph-0.2.4.dist-info/METADATA
+22 files, 1417504 bytes uncompressed, 552135 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,49 +1,67 @@
+Filename: gph/
+Comment: 
+
+Filename: giotto_ph.libs/
+Comment: 
+
+Filename: giotto_ph-0.2.4.dist-info/
+Comment: 
+
+Filename: gph/modules/
+Comment: 
+
+Filename: gph/python/
+Comment: 
+
 Filename: gph/__init__.py
 Comment: 
 
 Filename: gph/_version.py
 Comment: 
 
-Filename: gph/modules/gph_collapser.cp39-win_amd64.pyd
+Filename: gph/modules/gph_ripser.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: gph/modules/gph_ripser.cp39-win_amd64.pyd
+Filename: gph/modules/gph_ripser_coeff.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: gph/modules/gph_ripser_coeff.cp39-win_amd64.pyd
+Filename: gph/modules/gph_collapser.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: gph/python/test/
 Comment: 
 
 Filename: gph/python/__init__.py
 Comment: 
 
 Filename: gph/python/ripser_interface.py
 Comment: 
 
-Filename: gph/python/test/__init__.py
+Filename: gph/python/test/test_wrp.py
 Comment: 
 
-Filename: gph/python/test/test_collapser.py
+Filename: gph/python/test/test_ripser.py
 Comment: 
 
-Filename: gph/python/test/test_ripser.py
+Filename: gph/python/test/__init__.py
 Comment: 
 
-Filename: gph/python/test/test_wrp.py
+Filename: gph/python/test/test_collapser.py
 Comment: 
 
-Filename: giotto_ph-0.2.3.dist-info/LICENSE
+Filename: giotto_ph-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: giotto_ph-0.2.3.dist-info/METADATA
+Filename: giotto_ph-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: giotto_ph-0.2.3.dist-info/WHEEL
+Filename: giotto_ph-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: giotto_ph-0.2.3.dist-info/top_level.txt
+Filename: giotto_ph-0.2.4.dist-info/RECORD
 Comment: 
 
-Filename: giotto_ph-0.2.3.dist-info/RECORD
+Filename: giotto_ph-0.2.4.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## gph/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-from .python import ripser_parallel
-from ._version import __version__
-
-__all__ = [
-    "ripser_parallel",
-    "modules",
-    "__version__"
-]
+from .python import ripser_parallel
+from ._version import __version__
+
+__all__ = [
+    "ripser_parallel",
+    "modules",
+    "__version__"
+]
```

## gph/_version.py

```diff
@@ -1,22 +1,22 @@
-"""``giotto-ph`` is a C++/Python library implementing algorithms for the
-computation of persistent homology for different filtrations."""
-# License: GNU AGPLv3
-
-# PEP0440 compatible formatted version, see:
-# https://www.python.org/dev/peps/pep-0440/
-#
-# Generic release markers:
-# X.Y
-# X.Y.Z # For bugfix releases
-#
-# Admissible pre-release markers:
-# X.YaN # Alpha release
-# X.YbN # Beta release
-# X.YrcN # Release Candidate
-# X.Y # Final release
-#
-# Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
-# 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-#
-
-__version__ = "0.2.3"
+"""``giotto-ph`` is a C++/Python library implementing algorithms for the
+computation of persistent homology for different filtrations."""
+# License: GNU AGPLv3
+
+# PEP0440 compatible formatted version, see:
+# https://www.python.org/dev/peps/pep-0440/
+#
+# Generic release markers:
+# X.Y
+# X.Y.Z # For bugfix releases
+#
+# Admissible pre-release markers:
+# X.YaN # Alpha release
+# X.YbN # Beta release
+# X.YrcN # Release Candidate
+# X.Y # Final release
+#
+# Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
+# 'X.Y.dev0' is the canonical version of 'X.Y.dev'
+#
+
+__version__ = "0.2.4"
```

## gph/python/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .ripser_interface import ripser_parallel
-
-__all__ = [
-    "ripser_parallel",
-]
+from .ripser_interface import ripser_parallel
+
+__all__ = [
+    "ripser_parallel",
+]
```

## gph/python/ripser_interface.py

 * *Ordering differences only*

```diff
@@ -1,648 +1,648 @@
-# MIT License
-# Copyright (c) 2018 Christopher Tralie and Nathaniel Saul
-# Copyright (c) 2021 Julian Burella Pérez and Umberto Lupo
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import math
-from warnings import catch_warnings, simplefilter
-
-import numpy as np
-from scipy.sparse import issparse, csr_matrix, triu
-from scipy.spatial.distance import squareform
-from sklearn.exceptions import EfficiencyWarning
-from sklearn.metrics.pairwise import pairwise_distances
-from sklearn.neighbors import NearestNeighbors, kneighbors_graph
-from sklearn.utils.validation import column_or_1d
-
-from ..modules import gph_ripser, gph_ripser_coeff, gph_collapser
-
-
-MAX_COEFF_SUPPORTED = gph_ripser.get_max_coefficient_field_supported()
-
-
-def _compute_ph_vr_dense(DParam, diagonal, maxHomDim, thresh=-1, coeff=2,
-                         n_threads=1, return_generators=False):
-    if coeff == 2:
-        ret = gph_ripser.rips_dm(DParam, diagonal, coeff, maxHomDim, thresh,
-                                 n_threads, return_generators)
-    else:
-        ret = gph_ripser_coeff.rips_dm(DParam, diagonal, coeff, maxHomDim,
-                                       thresh, n_threads, return_generators)
-    return ret
-
-
-def _compute_ph_vr_sparse(I, J, V, N, maxHomDim, thresh=-1, coeff=2,
-                          n_threads=1, return_generators=False):
-    if coeff == 2:
-        ret = gph_ripser.rips_dm_sparse(I, J, V, I.size, N, coeff,
-                                        maxHomDim, thresh, n_threads,
-                                        return_generators)
-    else:
-        ret = gph_ripser_coeff.rips_dm_sparse(I, J, V, I.size, N, coeff,
-                                              maxHomDim, thresh, n_threads,
-                                              return_generators)
-    return ret
-
-
-def _sanitize_coo(row, col, data, only_extract_upper=False):
-    """Given a sparse matrix in COO format, either return its upper triangular
-    portion directly, or filter out any entry at location (i, j) strictly below
-    the diagonal if the entry at (j, i) is also stored."""
-
-    row_orig, col_orig, data_orig = row, col, data
-
-    # Initialize filtered COO data with information in the upper triangle
-    in_upper_triangle = row_orig <= col_orig
-    row = row_orig[in_upper_triangle]
-    col = col_orig[in_upper_triangle]
-    data = data_orig[in_upper_triangle]
-    if only_extract_upper:
-        return row, col, data
-
-    below_diag_idxs = np.flatnonzero(np.logical_not(in_upper_triangle))
-    # Check if there is anything below the main diagonal
-    if len(below_diag_idxs):
-        # Only keep entries below the diagonal for which entries at transposed
-        # positions are not available
-        upper_triangle_row_col = set(zip(row, col))
-        additions_idxs = [
-            i for i in below_diag_idxs
-            if (col_orig[i], row_orig[i]) not in upper_triangle_row_col
-            ]
-        # Add surviving entries below the diagonal to final COO data
-        if len(additions_idxs):
-            row = np.concatenate([row, col_orig[additions_idxs]])
-            col = np.concatenate([col, row_orig[additions_idxs]])
-            data = np.concatenate([data, data_orig[additions_idxs]])
-
-    return row, col, data
-
-
-def _collapse_coo(row, col, data, thresh):
-    """Run edge collapser on off-diagonal data and then reinsert diagonal
-    data."""
-
-    diag = row == col
-    row_diag, col_diag, data_diag = row[diag], col[diag], data[diag]
-    row, col, data = gph_collapser. \
-        flag_complex_collapse_edges_coo(row, col, data.astype(np.float32),
-                                        thresh)
-    return (np.hstack([row_diag, row]),
-            np.hstack([col_diag, col]),
-            np.hstack([data_diag, data]))
-
-
-def _collapse_dense(dm, thresh):
-    """Run edge collapser on off-diagonal data and then reinsert diagonal
-    data if any non-zero value is present."""
-
-    # Use 32-bit float precision here so when diagonal is extracted,
-    # it is still 32-bit in the entire function operations.
-    dm = dm.astype(np.float32)
-
-    row, col, data = \
-        gph_collapser.flag_complex_collapse_edges_dense(dm, thresh)
-
-    data_diag = dm.diagonal()
-    if (data_diag != 0).any():
-        indices = np.arange(data_diag.shape[0])
-        row = np.hstack([indices, row])
-        col = np.hstack([indices, col])
-        data = np.hstack([data_diag, data])
-
-    return row, col, data
-
-
-def _compute_dtm_weights(dm, n_neighbors, weights_r):
-    with catch_warnings():
-        simplefilter("ignore", category=EfficiencyWarning)
-        knn = kneighbors_graph(dm, n_neighbors=n_neighbors,
-                               metric="precomputed", mode="distance",
-                               include_self=False)
-
-    weights = np.squeeze(np.asarray(knn.power(weights_r).sum(axis=1)))
-    weights /= n_neighbors + 1
-    weights **= (1 / weights_r)
-    weights *= 2
-
-    return weights
-
-
-def _weight_filtration(dist, weights_x, weights_y, p):
-    """Create a weighted distance matrix. For dense data, `weights_x` is a
-    column vector, `weights_y` is a 1D array, `dist` is the original distance
-    matrix, and the computations exploit array broadcasting. For sparse data,
-    all three are 1D arrays. `p` can only be ``numpy.inf``, ``1``, or ``2``."""
-
-    if p == np.inf:
-        return np.maximum(dist, np.maximum(weights_x, weights_y))
-    elif p == 1:
-        return np.where(dist <= np.abs(weights_x - weights_y) / 2,
-                        np.maximum(weights_x, weights_y),
-                        dist + (weights_x + weights_y) / 2)
-    elif p == 2:
-        with np.errstate(divide='ignore', invalid='ignore'):
-            return np.where(
-                dist <= np.abs(weights_x**2 - weights_y**2)**.5 / 2,
-                np.maximum(weights_x, weights_y),
-                np.sqrt((dist**2 + ((weights_x + weights_y) / 2)**2) *
-                        (dist**2 + ((weights_x - weights_y) / 2)**2)) / dist
-                )
-    else:
-        raise NotImplementedError(f"Weighting not supported for p = {p}")
-
-
-def _weight_filtration_sparse(row, col, data, weights, p):
-    weights_x = weights[row]
-    weights_y = weights[col]
-
-    return _weight_filtration(data, weights_x, weights_y, p)
-
-
-def _weight_filtration_dense(dm, weights, p):
-    weights_2d = weights[:, None]
-
-    return _weight_filtration(dm, weights_2d, weights, p)
-
-
-def _check_weights(weights, n_points):
-    weights = column_or_1d(weights)
-    if len(weights) != n_points:
-        raise ValueError(
-            f"Input distance/adjacency matrix implies {n_points} "
-            f"vertices but {len(weights)} weights were passed."
-        )
-    if np.any(weights < 0):
-        raise ValueError("All weights must be non-negative."
-                         "Negative weights passed.")
-
-    return weights
-
-
-def _compute_weights(dm, weights, weight_params, n_points,
-                     sparse_kwargs={}):
-    """TODO: Add documentation"""
-
-    # If one sparse argument is provided, then we compute weights
-    # for sparse
-    is_sparse = len(sparse_kwargs) != 0
-
-    if (is_sparse and (dm < 0).nnz) or (not is_sparse and (dm < 0).any()):
-        raise ValueError("Distance matrix has negative entries. "
-                         "Weighted Rips filtration unavailable.")
-
-    if is_sparse:
-        row = sparse_kwargs['row']
-        col = sparse_kwargs['col']
-        data = sparse_kwargs['data']
-
-    weight_params = {} if weight_params is None else weight_params
-    weights_p = weight_params.get("p", 1)
-
-    if isinstance(weights, str) and (weights == "DTM"):
-        n_neighbors = weight_params.get("n_neighbors", 3)
-        weights_r = weight_params.get("r", 2)
-
-        if is_sparse:
-            # Restrict to off-diagonal entries for weights computation since
-            # diagonal ones are given by `weights`. Explicitly set the diagonal
-            # to 0 -- this is also important for DTM since otherwise
-            # kneighbors_graph with include_self=False skips the first true
-            # neighbor.
-            off_diag = row != col
-            row, col, data = (np.hstack([row[off_diag], np.arange(n_points)]),
-                              np.hstack([col[off_diag], np.arange(n_points)]),
-                              np.hstack([data[off_diag], np.zeros(n_points)]))
-            # CSR matrix must be symmetric for kneighbors_graph to give
-            # correct results
-            dm = csr_matrix((np.hstack([data, data[:-n_points]]),
-                             (np.hstack([row, col[:-n_points]]),
-                              np.hstack([col, row[:-n_points]]))))
-        else:
-            if not np.array_equal(dm, dm.T):
-                dm = np.triu(dm, k=1)
-                dm += dm.T
-
-        weights = _compute_dtm_weights(dm, n_neighbors, weights_r)
-    elif isinstance(weights, str):
-        raise ValueError("'{}' passed for `weights` but the "
-                         "only allowed string is 'DTM'".format(weights))
-    else:
-        weights = _check_weights(weights, n_points)
-
-    if is_sparse:
-        data = _weight_filtration_sparse(row, col, data, weights,
-                                         weights_p)
-        return row, col, data
-    else:
-        dm = _weight_filtration_dense(dm, weights, weights_p)
-        np.fill_diagonal(dm, weights)
-        return dm
-
-
-def _ideal_thresh(dm, thresh):
-    """Compute the enclosing radius of an input distance matrix.
-
-    Under a Vietoris–Rips filtration, all homology groups are trivial above
-    this value because the complex becomes a cone.
-
-    The enclosing radius is only computed if the input matrix is square."""
-
-    # Check that matrix is square
-    if dm.shape[0] != dm.shape[1]:
-        return thresh
-
-    # Compute enclosing radius
-    enclosing_radius = np.min(np.max(dm, axis=1))
-
-    return min([enclosing_radius, thresh])
-
-
-def _pc_to_sparse_dm_with_threshold(X, thresh, nearest_neighbors_params,
-                                    metric, metric_params, n_threads):
-    """Compute a sparse matrix of pairwise distances between points in a point
-    cloud, removing all distances larger than a threshold.
-
-    Return the output as an upper triangular sparse matrix in COO format."""
-
-    neigh = NearestNeighbors(radius=thresh,
-                             metric=metric,
-                             metric_params=metric_params,
-                             n_jobs=n_threads,
-                             **nearest_neighbors_params).fit(X)
-    # Upper triangular COO output
-    dm = triu(neigh.radius_neighbors_graph(mode="distance"),
-              format="coo")
-
-    return dm
-
-
-def _is_prime_and_larger_than_2(x, N):
-    """Test whether 2 < x <= N is prime. Returns False when x is 2."""
-    if not x % 2 or x > N:
-        return False
-
-    # https://stackoverflow.com/questions/2068372/fastest-way-to-list-all-
-    # primes-below-n-in-python/3035188#3035188
-    sieve = [True] * (x + 1)
-    for i in range(3, int(math.sqrt(x)) + 1, 2):
-        if sieve[i]:
-            sieve[i * i::2 * i] = \
-                [False] * ((x - i * i) // (2 * i) + 1)
-
-    return sieve[x]
-
-
-def ripser_parallel(X, maxdim=1, thresh=np.inf, coeff=2, metric="euclidean",
-                    metric_params={}, nearest_neighbors_params={},
-                    weights=None, weight_params=None, collapse_edges=False,
-                    n_threads=1, return_generators=False):
-    """Compute persistence diagrams from an input dense array or sparse matrix.
-
-    If `X` represents a point cloud, a distance matrix will be internally
-    created using the chosen metric and its Vietoris–Rips persistent homology
-    will be computed. Computations in homology dimensions 1 and above can be
-    parallelized, see `n_threads`.
-
-    Parameters
-    ----------
-    X : ndarray or sparse matrix
-        If `metric` is not set to ``"precomputed"``, input data of shape
-        ``(n_samples, n_features)`` representing a point cloud. Otherwise,
-        dense or sparse input data of shape ``(n_samples, n_samples)``
-        representing a distance matrix or adjacency matrix of a weighted
-        undirected graph, with the following conventions:
-            - Diagonal entries indicate vertex weights, i.e. the filtration
-              parameters at which vertices appear.
-            - If `X` is dense, only its upper diagonal portion (including the
-              diagonal) is considered.
-            - If `X` is sparse, it does not need to be upper diagonal or
-              symmetric. If only one of entry (i, j) and (j, i) is stored, its
-              value is taken as the weight of the undirected edge {i, j}. If
-              both are stored, the value in the upper diagonal is taken.
-              Off-diagonal entries which are not explicitly stored are treated
-              as infinite, indicating absent edges.
-            - Entries of `X` should be compatible with a filtration, i.e. the
-              value at index (i, j) should be no smaller than the values at
-              diagonal indices (i, i) and (j, j).
-
-    maxdim : int, optional, default: ``1``
-        Maximum homology dimension computed. Will compute all dimensions lower
-        than or equal to this value.
-
-    thresh : float, optional, default: ``numpy.inf``
-        Maximum value of the Vietoris–Rips filtration parameter. Points whose
-        distance is greater than this value will never be connected by an edge.
-        If ``numpy.inf``, compute the entire filtration. Otherwise, and if
-        `metric` is not ``"precomputed"``, see `nearest_neighbors_params`.
-
-    coeff : int prime, optional, default: ``2``
-        Compute homology with coefficients in the prime field Z/pZ for p=coeff.
-
-    metric : string or callable, optional, default: ``'euclidean'``
-        The metric to use when calculating distance between instances in a
-        feature array. If set to ``'precomputed'``, input data is interpreted
-        as a distance matrix or of adjacency matrices of a weighted undirected
-        graph. If a string, it must be one of the options allowed by
-        :func:`scipy.spatial.distance.pdist` for its metric parameter, or a
-        metric listed in :obj:`sklearn.pairwise.PAIRWISE_DISTANCE_FUNCTIONS`,
-        including ``'euclidean'``, ``'manhattan'`` or ``'cosine'``. If a
-        callable, it should take pairs of vectors (1D arrays) as input and, for
-        each two vectors in a pair, it should return a scalar indicating the
-        distance/dissimilarity between them.
-
-    metric_params : dict, optional, default: ``{}``
-        Additional parameters to be passed to the distance function.
-
-    nearest_neighbors_params : dict, optional, default: ``{}``
-        Additional parameters that can be passed when `thresh` is finite and
-        `metric` is not ``"precomputed"``. Allowed keys and values are as
-        follows:
-
-            - ``"algorithm"``: ``"auto"`` | ``"ball_tree"`` | ``"kd_tree"`` |
-              ``"brute"`` (default when not passed: ``"auto"``)
-            - ``"leaf_size"``: int (default when not passed: ``30``)
-
-        These are passed as keyword arguments to an instance of
-        :class:`sklearn.neighbors.NearestNeighbors` to compute the thresholded
-        distance matrix in a sparse format. See the relevant
-        `scikit-learn User Guide
-        <https://scikit-learn.org/stable/modules/neighbors.html>`_.
-
-    weights : ``"DTM"``, ndarray or None, optional, default: ``None``
-        If not ``None``, the persistence of a weighted Vietoris-Rips filtration
-        is computed as described in [6]_, and this parameter determines the
-        vertex weights in the modified adjacency matrix. ``"DTM"`` denotes the
-        empirical distance-to-measure function defined, following [6]_, by
-
-        .. math:: w(x) = 2\\left(\\frac{1}{n+1} \\sum_{k=1}^n
-           \\mathrm{dist}(x, x_k)^r \\right)^{1/r}.
-
-        Here, :math:`\\mathrm{dist}` is the distance metric used, :math:`x_k`
-        is the :math:`k`-th :math:`\\mathrm{dist}`-nearest neighbour of
-        :math:`x` (:math:`x` is not considered a neighbour of itself),
-        :math:`n` is the number of nearest neighbors to include, and :math:`r`
-        is a parameter (see `weight_params`). If an ndarray is passed, it is
-        interpreted as a user-defined list of vertex weights for the modified
-        adjacency matrix. In either case, the edge weights
-        :math:`\\{w_{ij}\\}_{i, j}` for the modified adjacency matrix are
-        computed from the original distances and the new vertex weights
-        :math:`\\{w_i\\}_i` as follows:
-
-        .. math:: w_{ij} = \\begin{cases} \\max\\{ w_i, w_j \\}
-           &\\text{if } 2\\mathrm{dist}_{ij} \\leq
-           |w_i^p - w_j^p|^{\\frac{1}{p}} \\\\
-           t &\\text{otherwise} \\end{cases}
-
-        where :math:`t` is the only positive root of
-
-        .. math:: 2 \\mathrm{dist}_{ij} = (t^p - w_i^p)^\\frac{1}{p} +
-           (t^p - w_j^p)^\\frac{1}{p}
-
-        and :math:`p` is a parameter specified in `metric_params`.
-
-    weight_params : dict or None, optional, default: ``None``
-        Parameters to be used in the case of weighted filtrations, see
-        `weights`. In this case, the key ``"p"`` determines the power to be
-        used in computing edge weights from vertex weights. It can be one of
-        ``1``, ``2`` or ``np.inf`` and defaults to ``1``. If `weights` is
-        ``"DTM"``, the additional keys ``"r"`` (default: ``2``) and
-        ``"n_neighbors"`` (default: ``3``) are available (see `weights`,
-        where the latter corresponds to :math:`n`).
-
-    collapse_edges : bool, optional, default: ``False``
-        Whether to use the edge collapse algorithm as described in [5]_ prior
-        to computing persistence. Cannot be ``True`` if `return_generators` is
-        also ``True``.
-
-    n_threads : int, optional, default: ``1``
-        Maximum number of threads to be used during the computation in homology
-        dimensions 1 and above. ``-1`` means that the maximum number of threads
-        available on the host machine will be used if possible.
-
-    return_generators : bool, optional, default: ``False``
-        Whether to return information on the simplex pairs and essential
-        simplices corresponding to the finite and infinite bars (respectively)
-        in the persistence barcode. If ``True``, this information is stored in
-        the return dictionary under the key `gens`. Cannot be ``True`` if
-        `collapse_edges` is also ``True``.
-
-    Returns
-    -------
-    A dictionary holding the results of the computation. Keys and values are as
-    follows:
-
-        'dgms': list (length maxdim + 1) of ndarray (n_pairs, 2)
-            A list of persistence diagrams, one for each dimension less than or
-            equal to maxdim. Each diagram is an ndarray of size (n_pairs, 2)
-            with the first column representing the birth time and the second
-            column representing the death time of each pair.
-
-        'gens': tuple (length 4) of ndarray or list of ndarray
-            Information on the simplex pairs and essential simplices generating
-            the points in 'dgms'. Each simplex of dimension 1 or above is
-            replaced with the vertices of the edges that gave it its filtration
-            value. The 4 entries of this tuple are as follows:
-
-            index 0: int ndarray with 3 columns
-                Simplex pairs corresponding to finite bars in dimension 0, with
-                one vertex for birth and two vertices for death.
-            index 1: list (length maxdim) of int ndarray with 4 columns
-                Simplex pairs corresponding to finite bars in dimensions 1 to
-                maxdim, with two vertices (one edge) for birth and two for
-                death.
-            index 2: 1D int ndarray
-                Essential simplices corresponding to infinite bars in dimension
-                0, with one vertex for each birth.
-            index 3: list (length maxdim) of int ndarray with 2 columns
-                Essential simplices corresponding to infinite bars in
-                dimensions 1 to maxdim, with 2 vertices (edge) for each birth.
-
-    Notes
-    -----
-    The C++ backend and Python API for the computation of Vietoris–Rips
-    persistent homology are developments of the ones in the
-    `ripser.py <https://github.com/scikit-tda/ripser.py>`_ project [1]_, with
-    added optimizations from `Ripser <https://github.com/Ripser/ripser>`_ [2]_,
-    lock-free reduction from [3]_, and additional performance improvements. See
-    [4]_ for details.
-
-    Ripser supports two memory representations, dense and sparse. The sparse
-    representation is used in the following cases:
-        - input is sparse of type scipy.sparse;
-        - collapser is enabled;
-        - a threshold is provided.
-    The dense representation will be used in the following cases:
-        - input is a point cloud or a distance matrix.
-
-    The implementation of the edge collapse algorithm [5]_ is a modification of
-    `GUDHI's <https://github.com/GUDHI/gudhi-devel>`_ C++ implementation.
-
-    References
-    ----------
-    .. [1] C. Tralie et al, "Ripser.py: A Lean Persistent Homology Library for
-           Python", *Journal of Open Source Software*, **3**(29), 2021;
-           `DOI: 10.21105/joss.00925
-           <https://doi.org/10.21105/joss.00925>`_.
-   
-    .. [2] U. Bauer, "Ripser: efficient computation of Vietoris–Rips
-           persistence barcodes", *J Appl. and Comput. Topology*, **5**, pp.
-           391–423, 2021; `DOI: 10.1007/s41468-021-00071-5
-           <https://doi.org/10.1007/s41468-021-00071-5>`_.
-
-    .. [3] D. Morozov and A. Nigmetov, "Towards Lockfree Persistent Homology";
-           in *SPAA '20: Proceedings of the 32nd ACM Symposium on Parallelism
-           in Algorithms and Architectures*, pp. 555–557, 2020;
-           `DOI: 10.1145/3350755.3400244
-           <https://doi.org/10.1145/3350755.3400244>`_.
-
-    .. [4] J. Burella Pérez et al, "giotto-ph: A Python Library for
-           High-Performance Computation of Persistent Homology of Vietoris–Rips
-           Filtrations", 2021; `arXiv:2107.05412
-           <https://arxiv.org/abs/2107.05412>`_.
-
-    .. [5] J.-D. Boissonnat and S. Pritam, "Edge Collapse and Persistence of
-           Flag Complexes"; in *36th International Symposium on Computational
-           Geometry (SoCG 2020)*, pp. 19:1–19:15, Schloss
-           Dagstuhl-Leibniz–Zentrum für Informatik, 2020;
-           `DOI: 10.4230/LIPIcs.SoCG.2020.19
-           <https://doi.org/10.4230/LIPIcs.SoCG.2020.19>`_.
-
-    .. [6] H. Anai et al, "DTM-Based Filtrations"; in *Topological Data
-           Analysis* (Abel Symposia, vol 15), Springer, 2020;
-           `DOI: 10.1007/978-3-030-43408-3_2
-           <https://doi.org/10.1007/978-3-030-43408-3_2>`_.
-
-    """
-
-    if collapse_edges and return_generators:
-        raise NotImplementedError(
-            "`collapse_edges` and `return_generators`cannot both be True."
-        )
-
-    if coeff != 2 and \
-            not _is_prime_and_larger_than_2(coeff, MAX_COEFF_SUPPORTED):
-        raise ValueError("coeff value not supported, coeff value must be prime"
-                         " and lower than {}".format(MAX_COEFF_SUPPORTED))
-
-    use_sparse_computer = True
-    is_dm_sparse_and_upper_triangular = False
-    if metric == 'precomputed':
-        dm = X
-    elif thresh != np.inf:
-        dm = _pc_to_sparse_dm_with_threshold(
-            X, thresh, nearest_neighbors_params, metric, metric_params,
-            n_threads
-            )
-        is_dm_sparse_and_upper_triangular = True
-    else:
-        dm = pairwise_distances(X, metric=metric, **metric_params)
-
-    n_points = max(dm.shape)
-
-    if issparse(dm):
-        coo = dm.tocoo()
-        row, col, data = coo.row, coo.col, coo.data
-        if not is_dm_sparse_and_upper_triangular:
-            row, col, data = _sanitize_coo(row, col, data)
-
-        if weights is not None:
-            sparse_kwargs = {
-                'row': row,
-                'col': col,
-                'data': data
-            }
-            row, col, data = _compute_weights(dm, weights, weight_params,
-                                              n_points,
-                                              sparse_kwargs=sparse_kwargs)
-
-        if collapse_edges:
-            row, col, data = _collapse_coo(row, col, data, thresh)
-
-    else:
-        if weights is not None:
-            dm = _compute_weights(dm, weights, weight_params, n_points)
-
-        apply_user_threshold = thresh != np.inf
-        if not apply_user_threshold:
-            # Compute ideal threshold only when a distance matrix is passed
-            # as input without specifying any threshold
-            # We check if any element and if no entries is present in the
-            # diagonal. This allows to have the enclosing radius before
-            # calling collapser if computed
-            thresh = _ideal_thresh(dm, thresh)
-
-        if collapse_edges:
-            row, col, data = _collapse_dense(dm, thresh)
-
-        elif apply_user_threshold:
-            # If the user specifies a threshold, we use a sparse representation
-            # like Ripser does
-            row, col = np.nonzero(dm <= thresh)
-            data = dm[(row, col)]
-            row, col, data = _sanitize_coo(row, col, data,
-                                           only_extract_upper=True)
-        else:
-            use_sparse_computer = False
-
-    if use_sparse_computer:
-        res = _compute_ph_vr_sparse(
-            np.asarray(row, dtype=np.int64, order="C"),
-            np.asarray(col, dtype=np.int64, order="C"),
-            np.asarray(data, dtype=np.float32, order="C"),
-            n_points,
-            maxdim,
-            thresh,
-            coeff,
-            n_threads,
-            return_generators
-            )
-    else:
-        # Only consider upper diagonal
-        diagonal = np.diagonal(dm).astype(np.float32)
-        DParam = squareform(dm, checks=False).astype(np.float32)
-        res = _compute_ph_vr_dense(DParam, diagonal, maxdim, thresh,
-                                   coeff, n_threads, return_generators)
-
-    # Unwrap persistence diagrams
-    # Barcodes must match the inner type of C++ core filtration value.
-    # We call a method from the bindings that returns the barcodes as
-    # numpy arrays with np.float32 type
-    dgms = res.births_and_deaths_by_dim()
-    for dim in range(len(dgms)):
-        N = int(len(dgms[dim]) / 2)
-        dgms[dim] = np.reshape(np.array(dgms[dim]), [N, 2])
-
-    ret = {"dgms": dgms}
-
-    if return_generators:
-        finite_0 = np.array(res.flag_persistence_generators_by_dim.finite_0,
-                            dtype=np.int64).reshape(-1, 3)
-        finite_higher = [
-            np.array(x, dtype=np.int64).reshape(-1, 4)
-            for x in res.flag_persistence_generators_by_dim.finite_higher
-            ]
-        essential_0 = \
-            np.array(res.flag_persistence_generators_by_dim.essential_0,
-                     dtype=np.int64)
-        essential_higher = [
-            np.array(x, dtype=np.int64).reshape(-1, 2)
-            for x in res.flag_persistence_generators_by_dim.essential_higher
-            ]
-        ret['gens'] = (finite_0, finite_higher, essential_0, essential_higher)
-
-    return ret
+# MIT License
+# Copyright (c) 2018 Christopher Tralie and Nathaniel Saul
+# Copyright (c) 2021 Julian Burella Pérez and Umberto Lupo
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import math
+from warnings import catch_warnings, simplefilter
+
+import numpy as np
+from scipy.sparse import issparse, csr_matrix, triu
+from scipy.spatial.distance import squareform
+from sklearn.exceptions import EfficiencyWarning
+from sklearn.metrics.pairwise import pairwise_distances
+from sklearn.neighbors import NearestNeighbors, kneighbors_graph
+from sklearn.utils.validation import column_or_1d
+
+from ..modules import gph_ripser, gph_ripser_coeff, gph_collapser
+
+
+MAX_COEFF_SUPPORTED = gph_ripser.get_max_coefficient_field_supported()
+
+
+def _compute_ph_vr_dense(DParam, diagonal, maxHomDim, thresh=-1, coeff=2,
+                         n_threads=1, return_generators=False):
+    if coeff == 2:
+        ret = gph_ripser.rips_dm(DParam, diagonal, coeff, maxHomDim, thresh,
+                                 n_threads, return_generators)
+    else:
+        ret = gph_ripser_coeff.rips_dm(DParam, diagonal, coeff, maxHomDim,
+                                       thresh, n_threads, return_generators)
+    return ret
+
+
+def _compute_ph_vr_sparse(I, J, V, N, maxHomDim, thresh=-1, coeff=2,
+                          n_threads=1, return_generators=False):
+    if coeff == 2:
+        ret = gph_ripser.rips_dm_sparse(I, J, V, I.size, N, coeff,
+                                        maxHomDim, thresh, n_threads,
+                                        return_generators)
+    else:
+        ret = gph_ripser_coeff.rips_dm_sparse(I, J, V, I.size, N, coeff,
+                                              maxHomDim, thresh, n_threads,
+                                              return_generators)
+    return ret
+
+
+def _sanitize_coo(row, col, data, only_extract_upper=False):
+    """Given a sparse matrix in COO format, either return its upper triangular
+    portion directly, or filter out any entry at location (i, j) strictly below
+    the diagonal if the entry at (j, i) is also stored."""
+
+    row_orig, col_orig, data_orig = row, col, data
+
+    # Initialize filtered COO data with information in the upper triangle
+    in_upper_triangle = row_orig <= col_orig
+    row = row_orig[in_upper_triangle]
+    col = col_orig[in_upper_triangle]
+    data = data_orig[in_upper_triangle]
+    if only_extract_upper:
+        return row, col, data
+
+    below_diag_idxs = np.flatnonzero(np.logical_not(in_upper_triangle))
+    # Check if there is anything below the main diagonal
+    if len(below_diag_idxs):
+        # Only keep entries below the diagonal for which entries at transposed
+        # positions are not available
+        upper_triangle_row_col = set(zip(row, col))
+        additions_idxs = [
+            i for i in below_diag_idxs
+            if (col_orig[i], row_orig[i]) not in upper_triangle_row_col
+            ]
+        # Add surviving entries below the diagonal to final COO data
+        if len(additions_idxs):
+            row = np.concatenate([row, col_orig[additions_idxs]])
+            col = np.concatenate([col, row_orig[additions_idxs]])
+            data = np.concatenate([data, data_orig[additions_idxs]])
+
+    return row, col, data
+
+
+def _collapse_coo(row, col, data, thresh):
+    """Run edge collapser on off-diagonal data and then reinsert diagonal
+    data."""
+
+    diag = row == col
+    row_diag, col_diag, data_diag = row[diag], col[diag], data[diag]
+    row, col, data = gph_collapser. \
+        flag_complex_collapse_edges_coo(row, col, data.astype(np.float32),
+                                        thresh)
+    return (np.hstack([row_diag, row]),
+            np.hstack([col_diag, col]),
+            np.hstack([data_diag, data]))
+
+
+def _collapse_dense(dm, thresh):
+    """Run edge collapser on off-diagonal data and then reinsert diagonal
+    data if any non-zero value is present."""
+
+    # Use 32-bit float precision here so when diagonal is extracted,
+    # it is still 32-bit in the entire function operations.
+    dm = dm.astype(np.float32)
+
+    row, col, data = \
+        gph_collapser.flag_complex_collapse_edges_dense(dm, thresh)
+
+    data_diag = dm.diagonal()
+    if (data_diag != 0).any():
+        indices = np.arange(data_diag.shape[0])
+        row = np.hstack([indices, row])
+        col = np.hstack([indices, col])
+        data = np.hstack([data_diag, data])
+
+    return row, col, data
+
+
+def _compute_dtm_weights(dm, n_neighbors, weights_r):
+    with catch_warnings():
+        simplefilter("ignore", category=EfficiencyWarning)
+        knn = kneighbors_graph(dm, n_neighbors=n_neighbors,
+                               metric="precomputed", mode="distance",
+                               include_self=False)
+
+    weights = np.squeeze(np.asarray(knn.power(weights_r).sum(axis=1)))
+    weights /= n_neighbors + 1
+    weights **= (1 / weights_r)
+    weights *= 2
+
+    return weights
+
+
+def _weight_filtration(dist, weights_x, weights_y, p):
+    """Create a weighted distance matrix. For dense data, `weights_x` is a
+    column vector, `weights_y` is a 1D array, `dist` is the original distance
+    matrix, and the computations exploit array broadcasting. For sparse data,
+    all three are 1D arrays. `p` can only be ``numpy.inf``, ``1``, or ``2``."""
+
+    if p == np.inf:
+        return np.maximum(dist, np.maximum(weights_x, weights_y))
+    elif p == 1:
+        return np.where(dist <= np.abs(weights_x - weights_y) / 2,
+                        np.maximum(weights_x, weights_y),
+                        dist + (weights_x + weights_y) / 2)
+    elif p == 2:
+        with np.errstate(divide='ignore', invalid='ignore'):
+            return np.where(
+                dist <= np.abs(weights_x**2 - weights_y**2)**.5 / 2,
+                np.maximum(weights_x, weights_y),
+                np.sqrt((dist**2 + ((weights_x + weights_y) / 2)**2) *
+                        (dist**2 + ((weights_x - weights_y) / 2)**2)) / dist
+                )
+    else:
+        raise NotImplementedError(f"Weighting not supported for p = {p}")
+
+
+def _weight_filtration_sparse(row, col, data, weights, p):
+    weights_x = weights[row]
+    weights_y = weights[col]
+
+    return _weight_filtration(data, weights_x, weights_y, p)
+
+
+def _weight_filtration_dense(dm, weights, p):
+    weights_2d = weights[:, None]
+
+    return _weight_filtration(dm, weights_2d, weights, p)
+
+
+def _check_weights(weights, n_points):
+    weights = column_or_1d(weights)
+    if len(weights) != n_points:
+        raise ValueError(
+            f"Input distance/adjacency matrix implies {n_points} "
+            f"vertices but {len(weights)} weights were passed."
+        )
+    if np.any(weights < 0):
+        raise ValueError("All weights must be non-negative."
+                         "Negative weights passed.")
+
+    return weights
+
+
+def _compute_weights(dm, weights, weight_params, n_points,
+                     sparse_kwargs={}):
+    """TODO: Add documentation"""
+
+    # If one sparse argument is provided, then we compute weights
+    # for sparse
+    is_sparse = len(sparse_kwargs) != 0
+
+    if (is_sparse and (dm < 0).nnz) or (not is_sparse and (dm < 0).any()):
+        raise ValueError("Distance matrix has negative entries. "
+                         "Weighted Rips filtration unavailable.")
+
+    if is_sparse:
+        row = sparse_kwargs['row']
+        col = sparse_kwargs['col']
+        data = sparse_kwargs['data']
+
+    weight_params = {} if weight_params is None else weight_params
+    weights_p = weight_params.get("p", 1)
+
+    if isinstance(weights, str) and (weights == "DTM"):
+        n_neighbors = weight_params.get("n_neighbors", 3)
+        weights_r = weight_params.get("r", 2)
+
+        if is_sparse:
+            # Restrict to off-diagonal entries for weights computation since
+            # diagonal ones are given by `weights`. Explicitly set the diagonal
+            # to 0 -- this is also important for DTM since otherwise
+            # kneighbors_graph with include_self=False skips the first true
+            # neighbor.
+            off_diag = row != col
+            row, col, data = (np.hstack([row[off_diag], np.arange(n_points)]),
+                              np.hstack([col[off_diag], np.arange(n_points)]),
+                              np.hstack([data[off_diag], np.zeros(n_points)]))
+            # CSR matrix must be symmetric for kneighbors_graph to give
+            # correct results
+            dm = csr_matrix((np.hstack([data, data[:-n_points]]),
+                             (np.hstack([row, col[:-n_points]]),
+                              np.hstack([col, row[:-n_points]]))))
+        else:
+            if not np.array_equal(dm, dm.T):
+                dm = np.triu(dm, k=1)
+                dm += dm.T
+
+        weights = _compute_dtm_weights(dm, n_neighbors, weights_r)
+    elif isinstance(weights, str):
+        raise ValueError("'{}' passed for `weights` but the "
+                         "only allowed string is 'DTM'".format(weights))
+    else:
+        weights = _check_weights(weights, n_points)
+
+    if is_sparse:
+        data = _weight_filtration_sparse(row, col, data, weights,
+                                         weights_p)
+        return row, col, data
+    else:
+        dm = _weight_filtration_dense(dm, weights, weights_p)
+        np.fill_diagonal(dm, weights)
+        return dm
+
+
+def _ideal_thresh(dm, thresh):
+    """Compute the enclosing radius of an input distance matrix.
+
+    Under a Vietoris–Rips filtration, all homology groups are trivial above
+    this value because the complex becomes a cone.
+
+    The enclosing radius is only computed if the input matrix is square."""
+
+    # Check that matrix is square
+    if dm.shape[0] != dm.shape[1]:
+        return thresh
+
+    # Compute enclosing radius
+    enclosing_radius = np.min(np.max(dm, axis=1))
+
+    return min([enclosing_radius, thresh])
+
+
+def _pc_to_sparse_dm_with_threshold(X, thresh, nearest_neighbors_params,
+                                    metric, metric_params, n_threads):
+    """Compute a sparse matrix of pairwise distances between points in a point
+    cloud, removing all distances larger than a threshold.
+
+    Return the output as an upper triangular sparse matrix in COO format."""
+
+    neigh = NearestNeighbors(radius=thresh,
+                             metric=metric,
+                             metric_params=metric_params,
+                             n_jobs=n_threads,
+                             **nearest_neighbors_params).fit(X)
+    # Upper triangular COO output
+    dm = triu(neigh.radius_neighbors_graph(mode="distance"),
+              format="coo")
+
+    return dm
+
+
+def _is_prime_and_larger_than_2(x, N):
+    """Test whether 2 < x <= N is prime. Returns False when x is 2."""
+    if not x % 2 or x > N:
+        return False
+
+    # https://stackoverflow.com/questions/2068372/fastest-way-to-list-all-
+    # primes-below-n-in-python/3035188#3035188
+    sieve = [True] * (x + 1)
+    for i in range(3, int(math.sqrt(x)) + 1, 2):
+        if sieve[i]:
+            sieve[i * i::2 * i] = \
+                [False] * ((x - i * i) // (2 * i) + 1)
+
+    return sieve[x]
+
+
+def ripser_parallel(X, maxdim=1, thresh=np.inf, coeff=2, metric="euclidean",
+                    metric_params={}, nearest_neighbors_params={},
+                    weights=None, weight_params=None, collapse_edges=False,
+                    n_threads=1, return_generators=False):
+    """Compute persistence diagrams from an input dense array or sparse matrix.
+
+    If `X` represents a point cloud, a distance matrix will be internally
+    created using the chosen metric and its Vietoris–Rips persistent homology
+    will be computed. Computations in homology dimensions 1 and above can be
+    parallelized, see `n_threads`.
+
+    Parameters
+    ----------
+    X : ndarray or sparse matrix
+        If `metric` is not set to ``"precomputed"``, input data of shape
+        ``(n_samples, n_features)`` representing a point cloud. Otherwise,
+        dense or sparse input data of shape ``(n_samples, n_samples)``
+        representing a distance matrix or adjacency matrix of a weighted
+        undirected graph, with the following conventions:
+            - Diagonal entries indicate vertex weights, i.e. the filtration
+              parameters at which vertices appear.
+            - If `X` is dense, only its upper diagonal portion (including the
+              diagonal) is considered.
+            - If `X` is sparse, it does not need to be upper diagonal or
+              symmetric. If only one of entry (i, j) and (j, i) is stored, its
+              value is taken as the weight of the undirected edge {i, j}. If
+              both are stored, the value in the upper diagonal is taken.
+              Off-diagonal entries which are not explicitly stored are treated
+              as infinite, indicating absent edges.
+            - Entries of `X` should be compatible with a filtration, i.e. the
+              value at index (i, j) should be no smaller than the values at
+              diagonal indices (i, i) and (j, j).
+
+    maxdim : int, optional, default: ``1``
+        Maximum homology dimension computed. Will compute all dimensions lower
+        than or equal to this value.
+
+    thresh : float, optional, default: ``numpy.inf``
+        Maximum value of the Vietoris–Rips filtration parameter. Points whose
+        distance is greater than this value will never be connected by an edge.
+        If ``numpy.inf``, compute the entire filtration. Otherwise, and if
+        `metric` is not ``"precomputed"``, see `nearest_neighbors_params`.
+
+    coeff : int prime, optional, default: ``2``
+        Compute homology with coefficients in the prime field Z/pZ for p=coeff.
+
+    metric : string or callable, optional, default: ``'euclidean'``
+        The metric to use when calculating distance between instances in a
+        feature array. If set to ``'precomputed'``, input data is interpreted
+        as a distance matrix or of adjacency matrices of a weighted undirected
+        graph. If a string, it must be one of the options allowed by
+        :func:`scipy.spatial.distance.pdist` for its metric parameter, or a
+        metric listed in :obj:`sklearn.pairwise.PAIRWISE_DISTANCE_FUNCTIONS`,
+        including ``'euclidean'``, ``'manhattan'`` or ``'cosine'``. If a
+        callable, it should take pairs of vectors (1D arrays) as input and, for
+        each two vectors in a pair, it should return a scalar indicating the
+        distance/dissimilarity between them.
+
+    metric_params : dict, optional, default: ``{}``
+        Additional parameters to be passed to the distance function.
+
+    nearest_neighbors_params : dict, optional, default: ``{}``
+        Additional parameters that can be passed when `thresh` is finite and
+        `metric` is not ``"precomputed"``. Allowed keys and values are as
+        follows:
+
+            - ``"algorithm"``: ``"auto"`` | ``"ball_tree"`` | ``"kd_tree"`` |
+              ``"brute"`` (default when not passed: ``"auto"``)
+            - ``"leaf_size"``: int (default when not passed: ``30``)
+
+        These are passed as keyword arguments to an instance of
+        :class:`sklearn.neighbors.NearestNeighbors` to compute the thresholded
+        distance matrix in a sparse format. See the relevant
+        `scikit-learn User Guide
+        <https://scikit-learn.org/stable/modules/neighbors.html>`_.
+
+    weights : ``"DTM"``, ndarray or None, optional, default: ``None``
+        If not ``None``, the persistence of a weighted Vietoris-Rips filtration
+        is computed as described in [6]_, and this parameter determines the
+        vertex weights in the modified adjacency matrix. ``"DTM"`` denotes the
+        empirical distance-to-measure function defined, following [6]_, by
+
+        .. math:: w(x) = 2\\left(\\frac{1}{n+1} \\sum_{k=1}^n
+           \\mathrm{dist}(x, x_k)^r \\right)^{1/r}.
+
+        Here, :math:`\\mathrm{dist}` is the distance metric used, :math:`x_k`
+        is the :math:`k`-th :math:`\\mathrm{dist}`-nearest neighbour of
+        :math:`x` (:math:`x` is not considered a neighbour of itself),
+        :math:`n` is the number of nearest neighbors to include, and :math:`r`
+        is a parameter (see `weight_params`). If an ndarray is passed, it is
+        interpreted as a user-defined list of vertex weights for the modified
+        adjacency matrix. In either case, the edge weights
+        :math:`\\{w_{ij}\\}_{i, j}` for the modified adjacency matrix are
+        computed from the original distances and the new vertex weights
+        :math:`\\{w_i\\}_i` as follows:
+
+        .. math:: w_{ij} = \\begin{cases} \\max\\{ w_i, w_j \\}
+           &\\text{if } 2\\mathrm{dist}_{ij} \\leq
+           |w_i^p - w_j^p|^{\\frac{1}{p}} \\\\
+           t &\\text{otherwise} \\end{cases}
+
+        where :math:`t` is the only positive root of
+
+        .. math:: 2 \\mathrm{dist}_{ij} = (t^p - w_i^p)^\\frac{1}{p} +
+           (t^p - w_j^p)^\\frac{1}{p}
+
+        and :math:`p` is a parameter specified in `metric_params`.
+
+    weight_params : dict or None, optional, default: ``None``
+        Parameters to be used in the case of weighted filtrations, see
+        `weights`. In this case, the key ``"p"`` determines the power to be
+        used in computing edge weights from vertex weights. It can be one of
+        ``1``, ``2`` or ``np.inf`` and defaults to ``1``. If `weights` is
+        ``"DTM"``, the additional keys ``"r"`` (default: ``2``) and
+        ``"n_neighbors"`` (default: ``3``) are available (see `weights`,
+        where the latter corresponds to :math:`n`).
+
+    collapse_edges : bool, optional, default: ``False``
+        Whether to use the edge collapse algorithm as described in [5]_ prior
+        to computing persistence. Cannot be ``True`` if `return_generators` is
+        also ``True``.
+
+    n_threads : int, optional, default: ``1``
+        Maximum number of threads to be used during the computation in homology
+        dimensions 1 and above. ``-1`` means that the maximum number of threads
+        available on the host machine will be used if possible.
+
+    return_generators : bool, optional, default: ``False``
+        Whether to return information on the simplex pairs and essential
+        simplices corresponding to the finite and infinite bars (respectively)
+        in the persistence barcode. If ``True``, this information is stored in
+        the return dictionary under the key `gens`. Cannot be ``True`` if
+        `collapse_edges` is also ``True``.
+
+    Returns
+    -------
+    A dictionary holding the results of the computation. Keys and values are as
+    follows:
+
+        'dgms': list (length maxdim + 1) of ndarray (n_pairs, 2)
+            A list of persistence diagrams, one for each dimension less than or
+            equal to maxdim. Each diagram is an ndarray of size (n_pairs, 2)
+            with the first column representing the birth time and the second
+            column representing the death time of each pair.
+
+        'gens': tuple (length 4) of ndarray or list of ndarray
+            Information on the simplex pairs and essential simplices generating
+            the points in 'dgms'. Each simplex of dimension 1 or above is
+            replaced with the vertices of the edges that gave it its filtration
+            value. The 4 entries of this tuple are as follows:
+
+            index 0: int ndarray with 3 columns
+                Simplex pairs corresponding to finite bars in dimension 0, with
+                one vertex for birth and two vertices for death.
+            index 1: list (length maxdim) of int ndarray with 4 columns
+                Simplex pairs corresponding to finite bars in dimensions 1 to
+                maxdim, with two vertices (one edge) for birth and two for
+                death.
+            index 2: 1D int ndarray
+                Essential simplices corresponding to infinite bars in dimension
+                0, with one vertex for each birth.
+            index 3: list (length maxdim) of int ndarray with 2 columns
+                Essential simplices corresponding to infinite bars in
+                dimensions 1 to maxdim, with 2 vertices (edge) for each birth.
+
+    Notes
+    -----
+    The C++ backend and Python API for the computation of Vietoris–Rips
+    persistent homology are developments of the ones in the
+    `ripser.py <https://github.com/scikit-tda/ripser.py>`_ project [1]_, with
+    added optimizations from `Ripser <https://github.com/Ripser/ripser>`_ [2]_,
+    lock-free reduction from [3]_, and additional performance improvements. See
+    [4]_ for details.
+
+    Ripser supports two memory representations, dense and sparse. The sparse
+    representation is used in the following cases:
+        - input is sparse of type scipy.sparse;
+        - collapser is enabled;
+        - a threshold is provided.
+    The dense representation will be used in the following cases:
+        - input is a point cloud or a distance matrix.
+
+    The implementation of the edge collapse algorithm [5]_ is a modification of
+    `GUDHI's <https://github.com/GUDHI/gudhi-devel>`_ C++ implementation.
+
+    References
+    ----------
+    .. [1] C. Tralie et al, "Ripser.py: A Lean Persistent Homology Library for
+           Python", *Journal of Open Source Software*, **3**(29), 2021;
+           `DOI: 10.21105/joss.00925
+           <https://doi.org/10.21105/joss.00925>`_.
+   
+    .. [2] U. Bauer, "Ripser: efficient computation of Vietoris–Rips
+           persistence barcodes", *J Appl. and Comput. Topology*, **5**, pp.
+           391–423, 2021; `DOI: 10.1007/s41468-021-00071-5
+           <https://doi.org/10.1007/s41468-021-00071-5>`_.
+
+    .. [3] D. Morozov and A. Nigmetov, "Towards Lockfree Persistent Homology";
+           in *SPAA '20: Proceedings of the 32nd ACM Symposium on Parallelism
+           in Algorithms and Architectures*, pp. 555–557, 2020;
+           `DOI: 10.1145/3350755.3400244
+           <https://doi.org/10.1145/3350755.3400244>`_.
+
+    .. [4] J. Burella Pérez et al, "giotto-ph: A Python Library for
+           High-Performance Computation of Persistent Homology of Vietoris–Rips
+           Filtrations", 2021; `arXiv:2107.05412
+           <https://arxiv.org/abs/2107.05412>`_.
+
+    .. [5] J.-D. Boissonnat and S. Pritam, "Edge Collapse and Persistence of
+           Flag Complexes"; in *36th International Symposium on Computational
+           Geometry (SoCG 2020)*, pp. 19:1–19:15, Schloss
+           Dagstuhl-Leibniz–Zentrum für Informatik, 2020;
+           `DOI: 10.4230/LIPIcs.SoCG.2020.19
+           <https://doi.org/10.4230/LIPIcs.SoCG.2020.19>`_.
+
+    .. [6] H. Anai et al, "DTM-Based Filtrations"; in *Topological Data
+           Analysis* (Abel Symposia, vol 15), Springer, 2020;
+           `DOI: 10.1007/978-3-030-43408-3_2
+           <https://doi.org/10.1007/978-3-030-43408-3_2>`_.
+
+    """
+
+    if collapse_edges and return_generators:
+        raise NotImplementedError(
+            "`collapse_edges` and `return_generators`cannot both be True."
+        )
+
+    if coeff != 2 and \
+            not _is_prime_and_larger_than_2(coeff, MAX_COEFF_SUPPORTED):
+        raise ValueError("coeff value not supported, coeff value must be prime"
+                         " and lower than {}".format(MAX_COEFF_SUPPORTED))
+
+    use_sparse_computer = True
+    is_dm_sparse_and_upper_triangular = False
+    if metric == 'precomputed':
+        dm = X
+    elif thresh != np.inf:
+        dm = _pc_to_sparse_dm_with_threshold(
+            X, thresh, nearest_neighbors_params, metric, metric_params,
+            n_threads
+            )
+        is_dm_sparse_and_upper_triangular = True
+    else:
+        dm = pairwise_distances(X, metric=metric, **metric_params)
+
+    n_points = max(dm.shape)
+
+    if issparse(dm):
+        coo = dm.tocoo()
+        row, col, data = coo.row, coo.col, coo.data
+        if not is_dm_sparse_and_upper_triangular:
+            row, col, data = _sanitize_coo(row, col, data)
+
+        if weights is not None:
+            sparse_kwargs = {
+                'row': row,
+                'col': col,
+                'data': data
+            }
+            row, col, data = _compute_weights(dm, weights, weight_params,
+                                              n_points,
+                                              sparse_kwargs=sparse_kwargs)
+
+        if collapse_edges:
+            row, col, data = _collapse_coo(row, col, data, thresh)
+
+    else:
+        if weights is not None:
+            dm = _compute_weights(dm, weights, weight_params, n_points)
+
+        apply_user_threshold = thresh != np.inf
+        if not apply_user_threshold:
+            # Compute ideal threshold only when a distance matrix is passed
+            # as input without specifying any threshold
+            # We check if any element and if no entries is present in the
+            # diagonal. This allows to have the enclosing radius before
+            # calling collapser if computed
+            thresh = _ideal_thresh(dm, thresh)
+
+        if collapse_edges:
+            row, col, data = _collapse_dense(dm, thresh)
+
+        elif apply_user_threshold:
+            # If the user specifies a threshold, we use a sparse representation
+            # like Ripser does
+            row, col = np.nonzero(dm <= thresh)
+            data = dm[(row, col)]
+            row, col, data = _sanitize_coo(row, col, data,
+                                           only_extract_upper=True)
+        else:
+            use_sparse_computer = False
+
+    if use_sparse_computer:
+        res = _compute_ph_vr_sparse(
+            np.asarray(row, dtype=np.int64, order="C"),
+            np.asarray(col, dtype=np.int64, order="C"),
+            np.asarray(data, dtype=np.float32, order="C"),
+            n_points,
+            maxdim,
+            thresh,
+            coeff,
+            n_threads,
+            return_generators
+            )
+    else:
+        # Only consider upper diagonal
+        diagonal = np.diagonal(dm).astype(np.float32)
+        DParam = squareform(dm, checks=False).astype(np.float32)
+        res = _compute_ph_vr_dense(DParam, diagonal, maxdim, thresh,
+                                   coeff, n_threads, return_generators)
+
+    # Unwrap persistence diagrams
+    # Barcodes must match the inner type of C++ core filtration value.
+    # We call a method from the bindings that returns the barcodes as
+    # numpy arrays with np.float32 type
+    dgms = res.births_and_deaths_by_dim()
+    for dim in range(len(dgms)):
+        N = int(len(dgms[dim]) / 2)
+        dgms[dim] = np.reshape(np.array(dgms[dim]), [N, 2])
+
+    ret = {"dgms": dgms}
+
+    if return_generators:
+        finite_0 = np.array(res.flag_persistence_generators_by_dim.finite_0,
+                            dtype=np.int64).reshape(-1, 3)
+        finite_higher = [
+            np.array(x, dtype=np.int64).reshape(-1, 4)
+            for x in res.flag_persistence_generators_by_dim.finite_higher
+            ]
+        essential_0 = \
+            np.array(res.flag_persistence_generators_by_dim.essential_0,
+                     dtype=np.int64)
+        essential_higher = [
+            np.array(x, dtype=np.int64).reshape(-1, 2)
+            for x in res.flag_persistence_generators_by_dim.essential_higher
+            ]
+        ret['gens'] = (finite_0, finite_higher, essential_0, essential_higher)
+
+    return ret
```

## gph/python/test/test_collapser.py

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python
-
-""" Test comes from
-https://github.com/GUDHI/gudhi-devel/blob/master/src/Collapse/example/edge_collapse_basic_example.cpp
-"""
-
-import numpy as np
-from gph.modules.gph_collapser import \
-    flag_complex_collapse_edges_dense, \
-    flag_complex_collapse_edges_coo
-from scipy.sparse import coo_matrix, csr_matrix
-
-X = np.array([[0, 1, 1.],
-              [1, 2, 1.],
-              [2, 3, 1.],
-              [0, 3, np.inf],
-              [3, 0, 1.],
-              [0, 2, 2.],
-              [1, 3, 2.]])
-tX = np.transpose(X)
-tX = np.array([tX[0].astype(np.int32), tX[1].astype(np.int32), tX[2]])
-X_expected_row = [0, 1, 2]
-X_expected_col = [1, 2, 3]
-X_expected_data = [1.0, 1.0, 1.0]
-
-
-def check_collapse(collapsed, removed):
-    coo = collapsed.tocoo()
-    cooT = np.array([coo.row, coo.col, coo.data]).transpose()
-    for elem in removed:
-        if (cooT == elem).all(axis=1).any():
-            return False
-    return True
-
-
-def test_simple_coo_example():
-    coo_ = flag_complex_collapse_edges_coo(
-        tX[0], tX[1], tX[2])
-    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
-    assert check_collapse(coo, [[1, 3, 2]])
-
-
-def test_simple_dense_example():
-    data = csr_matrix((tX[2], (tX[0].astype(np.int32),
-                               tX[1].astype(np.int32)))).toarray()
-    coo_ = flag_complex_collapse_edges_dense(data)
-    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
-    assert check_collapse(coo, [[1, 3, 2]])
-
-
-def test_coo_expected_output():
-    coo_ = flag_complex_collapse_edges_coo(
-        tX[0], tX[1], tX[2])
-    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
-    assert np.equal(coo.row, X_expected_row).all()
-    assert np.equal(coo.col, X_expected_col).all()
-    assert np.equal(coo.data, X_expected_data).all()
-
-
-def test_dense_expected_output():
-    data = csr_matrix((tX[2], (tX[0].astype(np.int32),
-                               tX[1].astype(np.int32)))).toarray()
-    coo_ = flag_complex_collapse_edges_dense(data)
-    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
-    assert np.equal(coo.row, X_expected_row).all()
-    assert np.equal(coo.col, X_expected_col).all()
-    assert np.equal(coo.data, X_expected_data).all()
+#!/usr/bin/env python
+
+""" Test comes from
+https://github.com/GUDHI/gudhi-devel/blob/master/src/Collapse/example/edge_collapse_basic_example.cpp
+"""
+
+import numpy as np
+from gph.modules.gph_collapser import \
+    flag_complex_collapse_edges_dense, \
+    flag_complex_collapse_edges_coo
+from scipy.sparse import coo_matrix, csr_matrix
+
+X = np.array([[0, 1, 1.],
+              [1, 2, 1.],
+              [2, 3, 1.],
+              [0, 3, np.inf],
+              [3, 0, 1.],
+              [0, 2, 2.],
+              [1, 3, 2.]])
+tX = np.transpose(X)
+tX = np.array([tX[0].astype(np.int32), tX[1].astype(np.int32), tX[2]])
+X_expected_row = [0, 1, 2]
+X_expected_col = [1, 2, 3]
+X_expected_data = [1.0, 1.0, 1.0]
+
+
+def check_collapse(collapsed, removed):
+    coo = collapsed.tocoo()
+    cooT = np.array([coo.row, coo.col, coo.data]).transpose()
+    for elem in removed:
+        if (cooT == elem).all(axis=1).any():
+            return False
+    return True
+
+
+def test_simple_coo_example():
+    coo_ = flag_complex_collapse_edges_coo(
+        tX[0], tX[1], tX[2])
+    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
+    assert check_collapse(coo, [[1, 3, 2]])
+
+
+def test_simple_dense_example():
+    data = csr_matrix((tX[2], (tX[0].astype(np.int32),
+                               tX[1].astype(np.int32)))).toarray()
+    coo_ = flag_complex_collapse_edges_dense(data)
+    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
+    assert check_collapse(coo, [[1, 3, 2]])
+
+
+def test_coo_expected_output():
+    coo_ = flag_complex_collapse_edges_coo(
+        tX[0], tX[1], tX[2])
+    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
+    assert np.equal(coo.row, X_expected_row).all()
+    assert np.equal(coo.col, X_expected_col).all()
+    assert np.equal(coo.data, X_expected_data).all()
+
+
+def test_dense_expected_output():
+    data = csr_matrix((tX[2], (tX[0].astype(np.int32),
+                               tX[1].astype(np.int32)))).toarray()
+    coo_ = flag_complex_collapse_edges_dense(data)
+    coo = coo_matrix((coo_[2], (coo_[0], coo_[1])))
+    assert np.equal(coo.row, X_expected_row).all()
+    assert np.equal(coo.col, X_expected_col).all()
+    assert np.equal(coo.data, X_expected_data).all()
```

## gph/python/test/test_ripser.py

 * *Ordering differences only*

```diff
@@ -1,478 +1,478 @@
-import numpy as np
-import pytest
-from hypothesis import given, settings
-from hypothesis.extra.numpy import arrays
-from hypothesis.strategies import floats, integers, composite
-from numpy.testing import assert_almost_equal, assert_array_equal
-from scipy.sparse import coo_matrix
-from scipy.spatial.distance import pdist, squareform
-
-from gph import ripser_parallel as ripser
-
-
-def make_dm_symmetric(dm):
-    # Extract strict upper diagonal and make symmetric
-    dm = np.triu(dm.astype(np.float32), k=1)
-    return dm + dm.T
-
-
-@composite
-def get_dense_distance_matrices(draw):
-    """Generate 2d dense square arrays of floats, with zero along the
-    diagonal."""
-    shapes = draw(integers(min_value=2, max_value=30))
-    dm = draw(arrays(dtype=float,
-                     elements=floats(allow_nan=False,
-                                     allow_infinity=True,
-                                     min_value=0,
-                                     exclude_min=True,
-                                     width=32),
-                     shape=(shapes, shapes), unique=False))
-    return make_dm_symmetric(dm)
-
-
-@composite
-def get_sparse_distance_matrices(draw):
-    """Generate 2d upper triangular sparse matrices of floats, with zero along
-    the diagonal."""
-    shapes = draw(integers(min_value=2, max_value=40))
-    dm = draw(arrays(dtype=float,
-                     elements=floats(allow_nan=False,
-                                     allow_infinity=True,
-                                     min_value=0,
-                                     exclude_min=True,
-                                     width=32),
-                     shape=(shapes, shapes), unique=False))
-    dm = np.triu(dm.astype(np.float32), k=1)
-    dm = coo_matrix(dm)
-    row, col, data = dm.row, dm.col, dm.data
-    not_inf_idx = data != np.inf
-    row = row[not_inf_idx]
-    col = col[not_inf_idx]
-    data = data[not_inf_idx]
-    shape_kwargs = {} if data.size else {"shape": (0, 0)}
-    dm = coo_matrix((data, (row, col)), **shape_kwargs)
-    return dm
-
-
-@settings(deadline=500)
-@given(dm=get_sparse_distance_matrices())
-def test_coo_below_diagonal_and_mixed_same_as_above(dm):
-    """Test that if we feed sparse matrices representing the same undirected
-    weighted graph we obtain the same results regardless of whether all entries
-    are above the diagonal, all are below the diagonal, or neither.
-    Furthermore, test that conflicts between stored data in the upper and lower
-    triangle are resolved in favour of the upper triangle."""
-    ripser_kwargs = {"maxdim": 2, "metric": "precomputed"}
-
-    pd_above = ripser(dm, **ripser_kwargs)['dgms']
-
-    pd_below = ripser(dm.T, **ripser_kwargs)['dgms']
-
-    _row, _col, _data = dm.row, dm.col, dm.data
-    coo_shape_kwargs = {} if _data.size else {"shape": (0, 0)}
-    to_transpose_mask = np.full(len(_row), False)
-    to_transpose_mask[np.random.choice(np.arange(len(_row)),
-                                       size=len(_row) // 2,
-                                       replace=False)] = True
-    row = np.concatenate([_col[to_transpose_mask], _row[~to_transpose_mask]])
-    col = np.concatenate([_row[to_transpose_mask], _col[~to_transpose_mask]])
-    dm_mixed = coo_matrix((_data, (row, col)), **coo_shape_kwargs)
-    pd_mixed = ripser(dm_mixed, **ripser_kwargs)['dgms']
-
-    row = np.concatenate([row, _row[to_transpose_mask]])
-    col = np.concatenate([col, _col[to_transpose_mask]])
-    data = np.random.random(len(row))
-    data[:len(_row)] = _data
-    dm_conflicts = coo_matrix((data, (row, col)), **coo_shape_kwargs)
-    pd_conflicts = ripser(dm_conflicts, **ripser_kwargs)['dgms']
-
-    for i in range(ripser_kwargs["maxdim"] + 1):
-        pd_above[i] = np.sort(pd_above[i], axis=0)
-        pd_below[i] = np.sort(pd_below[i], axis=0)
-        pd_mixed[i] = np.sort(pd_mixed[i], axis=0)
-        pd_conflicts[i] = np.sort(pd_conflicts[i], axis=0)
-        assert_almost_equal(pd_above[i], pd_below[i])
-
-
-@pytest.mark.parametrize('thresh', [False, True])
-@pytest.mark.parametrize('coeff', [2, 7])
-@settings(deadline=500)
-@given(dm=get_dense_distance_matrices())
-def test_collapse_consistent_with_no_collapse_dense(thresh, coeff, dm):
-    thresh = np.max(dm) / 2 if thresh else np.inf
-    maxdim = 3
-    pd_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
-                         metric='precomputed', collapse_edges=True)['dgms']
-    pd_no_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
-                            metric='precomputed', collapse_edges=False)['dgms']
-    for i in range(maxdim + 1):
-        pd_collapse[i] = np.sort(pd_collapse[i], axis=0)
-        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
-        assert_almost_equal(pd_collapse[i], pd_no_collapse[i])
-
-
-@pytest.mark.parametrize('thresh', [False, True])
-@pytest.mark.parametrize('coeff', [2, 7])
-@settings(deadline=500)
-@given(dm=get_sparse_distance_matrices())
-def test_collapse_consistent_with_no_collapse_coo(thresh, coeff, dm):
-    if thresh and dm.nnz:
-        thresh = np.max(dm) / 2
-    else:
-        thresh = np.inf
-    maxdim = 3
-    pd_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
-                         metric='precomputed', collapse_edges=True)['dgms']
-    pd_no_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
-                            metric='precomputed', collapse_edges=False)['dgms']
-    for i in range(maxdim + 1):
-        pd_collapse[i] = np.sort(pd_collapse[i], axis=0)
-        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
-        assert_almost_equal(pd_collapse[i], pd_no_collapse[i])
-
-
-def test_collapser_with_negative_weights():
-    """Test that collapser works as expected when some of the vertex and edge
-    weights are negative."""
-    n_points = 20
-    dm = make_dm_symmetric(np.random.random((n_points, n_points)))
-    np.fill_diagonal(dm, -np.random.random(n_points))
-    dm -= 0.2
-    dm_sparse = coo_matrix(dm)
-
-    maxdim = 2
-    pd_collapse_dense = ripser(dm, metric='precomputed', maxdim=maxdim,
-                               collapse_edges=True)['dgms']
-    pd_collapse_sparse = ripser(dm_sparse, metric='precomputed',
-                                maxdim=maxdim, collapse_edges=True)['dgms']
-    pd_no_collapse = ripser(dm, metric='precomputed', maxdim=maxdim,
-                            collapse_edges=False)['dgms']
-
-    for i in range(maxdim + 1):
-        pd_collapse_dense[i] = np.sort(pd_collapse_dense[i], axis=0)
-        pd_collapse_sparse[i] = np.sort(pd_collapse_sparse[i], axis=0)
-        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
-        assert_almost_equal(pd_collapse_dense[i], pd_no_collapse[i])
-        assert_almost_equal(pd_collapse_sparse[i], pd_no_collapse[i])
-
-
-def test_coo_results_independent_of_order():
-    """Regression test for PR #465"""
-    data = np.array([6., 8., 2., 4., 5., 9., 10., 3., 1., 1.])
-    row = np.array([0, 0, 0, 0, 1, 1, 1, 2, 2, 3])
-    col = np.array([4, 1, 3, 2, 4, 3, 2, 3, 4, 4])
-    dm = coo_matrix((data, (row, col)))
-    diagrams = ripser(dm, metric="precomputed")['dgms']
-    diagrams_csr = ripser(dm.tocsr(), metric="precomputed")['dgms']
-    expected = [np.array([[0., 1.],
-                          [0., 1.],
-                          [0., 2.],
-                          [0., 5.],
-                          [0., np.inf]]),
-                np.array([], dtype=float).reshape(0, 2)]
-    for i in range(2):
-        assert np.array_equal(diagrams[i], expected[i])
-        assert np.array_equal(diagrams_csr[i], expected[i])
-
-
-@settings(deadline=500)
-@given(dm=get_dense_distance_matrices())
-def test_multithread_consistent(dm):
-    """Test that varying the number of threads produces consistent results"""
-    maxdim = 3
-    nb_threads_to_test = [1, 2, 3, 4, 5]
-    res = []
-    for nb_threads in nb_threads_to_test:
-        res.append(ripser(dm, maxdim=maxdim, metric='precomputed',
-                          n_threads=nb_threads)['dgms'])
-    for dim in range(maxdim + 1):
-        res[0][dim] = np.sort(res[0][dim], axis=0)
-        for i in range(1, len(res)):
-            res[i][dim] = np.sort(res[i][dim], axis=0)
-            assert_almost_equal(res[0][dim], res[i][dim])
-
-
-def test_gens_edge_in_dm_and_sorted():
-    """This test verifies that the representative simplicies, the index of the
-    vertices matches the corresponding edge in the distance matrix and that
-    the gens are aligned with the correponding barcodes"""
-    X = squareform(pdist(np.random.random((100, 3))))
-
-    ret = ripser(X, metric='precomputed', maxdim=3, thresh=np.inf,
-                 collapse_edges=False, return_generators=True)
-
-    barcodes = ret['dgms']
-    gens = ret['gens']
-
-    for dim, bar_in_dim in enumerate(barcodes):
-        idx_essential = 0
-        idx_finite = 0
-        for barcode in bar_in_dim:
-            if dim == 0 and barcode[1] != np.inf:
-                # Verifies gens in dim 0, discards essential ones
-                gens_of_barcode = gens[0][idx_finite]
-                assert np.isclose(barcode[1],
-                                  X[gens_of_barcode[1]][gens_of_barcode[2]])
-                idx_finite = idx_finite + 1
-            if dim > 0:
-                # Verifies gens in dim > 0, expects first all non essential
-                # barcodes and then the finite ones
-                if barcode[1] != np.inf:
-                    gens_of_barcode = gens[1][dim-1][idx_finite]
-                    assert np.isclose(barcode[0],
-                                      X[gens_of_barcode[0]][gens_of_barcode[1]]
-                                      )
-                    assert np.isclose(barcode[1],
-                                      X[gens_of_barcode[2]][gens_of_barcode[3]]
-                                      )
-                    idx_finite = idx_finite + 1
-                else:
-                    gens_of_barcode = gens[3][dim-1][idx_essential]
-                    assert np.isclose(barcode[0],
-                                      X[gens_of_barcode[0]][gens_of_barcode[1]]
-                                      )
-                    idx_essential = idx_essential + 1
-
-
-def test_gens_with_collapser():
-    """This test ensures that you cannot use collapser and
-    retrieve generators. This is a temporary behavior."""
-    X = squareform(pdist(np.random.random((10, 3))))
-
-    with pytest.raises(NotImplementedError):
-        ripser(X, metric='precomputed', collapse_edges=True,
-               return_generators=True)
-
-
-@settings(deadline=500)
-@given(dm=get_dense_distance_matrices())
-@pytest.mark.parametrize('format', ['dense', 'sparse'])
-def test_gens_non_0_diagonal_dim0(dm, format):
-    np.fill_diagonal(dm, np.random.uniform(low=0, high=np.amin(dm),
-                                           size=(dm.shape[0])))
-    x_len = dm.shape[0]
-    if format == 'dense':
-        X = dm
-    else:
-        X = coo_matrix(dm).tocsr()
-
-    ret = ripser(X, metric='precomputed', return_generators=True)
-
-    dgms_0 = ret['dgms'][0]
-    gens_fin_0 = ret['gens'][0]
-    gens_ess_0 = ret['gens'][2]
-
-    # Verifies that the number of essential and finite generators
-    # combined is equal to the number of points in the point cloud
-    assert (x_len - len(gens_ess_0)) == len(gens_fin_0)
-
-    # Verifies that the birth indices for essential and finite
-    # representatives are unique
-    assert len(np.unique(np.sort(gens_fin_0[:, 0]))) == len(gens_fin_0[:, 0])
-    assert len(np.unique(np.sort(gens_ess_0))) == len(gens_ess_0)
-    # Verifies that there are no duplicates between finite and essential
-    # And also the other way around
-    assert len([x for x in gens_fin_0[:, 0] if x in gens_ess_0]) == 0
-    assert len([x for x in gens_ess_0 if x in gens_fin_0[:, 0]]) == 0
-
-    for barcode, rp in zip(dgms_0, gens_fin_0):
-        # Verify birth of dim-0 finite representative
-        # The birth is located on the diagonal
-        assert np.isclose(barcode[0], X[rp[0], rp[0]])
-
-        # Verify death of dim-0 finite representative
-        assert np.isclose(barcode[1], X[rp[1], rp[2]])
-
-    for barcode, rp in zip(dgms_0[len(dgms_0):], gens_ess_0):
-        # Verify birth of dim-0 essential representative
-        # The birth is located on the diagonal
-        assert np.isclose(barcode[0], X[rp, rp])
-
-
-def test_gens_order_vertices_higher_dimension():
-    """This test verifies that function `get_youngest_edge_simplex` returns the
-    correct vertices. It should return the edge with the largest diameter in
-    the simplex and, if several are present with the same diameter, the oldest
-    one in the reverse colexicographic order used to build the simplexwise
-    refinement of the Vietoris-Rips filtration."""
-    diamond = np.array(
-        [[0,      1,    100,      1,      1,      1],
-         [0,      0,      1,    100,      1,      1],
-         [0,      0,      0,      1,      1,      1],
-         [0,      0,      0,      0,      1,      1],
-         [0,      0,      0,      0,      0,    100],
-         [0,      0,      0,      0,      0,      0]],
-        dtype=np.float64)
-
-    diamond += diamond.T
-
-    gens = ripser(diamond, maxdim=2, return_generators=True)['gens']
-    gens_fin_dim2 = gens[1][1]
-
-    assert len(gens_fin_dim2) == 1
-    assert np.array_equal(gens_fin_dim2[0], np.array([1, 0, 5, 4]))
-
-
-def test_ph_maxdim_0():
-    """Regression test for issue #39, an issue was found when only computing
-    up to dimension 0. The test also compares the results of dimension 0
-    when maxdim=1 and maxdim=0"""
-    X = np.array([[1., 2], [3, 4], [5, 0]])
-    res_maxdim_0 = ripser(X, maxdim=0)['dgms'][0]
-    res_maxdim_1 = ripser(X, maxdim=1)['dgms'][0]
-
-    # Verifies that the two computations lead to the same barcodes
-    assert_array_equal(res_maxdim_0, res_maxdim_1)
-
-
-@settings(deadline=500)
-@given(dm=get_dense_distance_matrices())
-def test_equivariance(dm):
-    """Test that if we shift all entries (diagonal or not) in the input matrix
-    by a constant then the barcodes are also shifted by that constant. Doubles
-    also as a regression test for issue #31."""
-    maxdim = 1
-    kwargs = {"metric": "precomputed", "maxdim": maxdim}
-
-    # - Median may or may not make some edges zero, and will make some edges
-    #   negative and all vertex weights negative
-    # - Min is guaranteed to make at least one edge exactly zero, and all
-    #   vertex weights negative
-    # - Max is guaranteed to make all edge and vertex weights non-positive (or
-    #   infinite)
-    dm_flat = squareform(dm, checks=False)  # Get strict upper diagonal
-    dm_finite_nonzero_flat_sorted = np.sort(
-        dm_flat[np.logical_and(dm_flat > 0, dm_flat < np.inf)]
-        )  # Filter out zero values and infinite values, and sort
-    # This test will fail if val - offset = -offset numerically for some entry
-    # val in dm, because this will make some 0-dimensional classes disappear
-    # (they are born dead)
-    offsets = [0, 0, 0]  # Fallback if no edge weights are finite and positive
-    if len(dm_finite_nonzero_flat_sorted):
-        offset_cand = [np.float32(np.median(dm_finite_nonzero_flat_sorted)),
-                       np.min(dm_finite_nonzero_flat_sorted),
-                       np.max(dm_finite_nonzero_flat_sorted)]
-        for i, offset in enumerate(offset_cand):
-            if not np.any(dm - offset == -offset):
-                offsets[i] = offset_cand
-
-    dgms_orig = ripser(dm, **kwargs)["dgms"]
-
-    for offset in offsets:
-        dgms_offset = ripser(dm - offset, **kwargs)["dgms"]
-        for dim in range(maxdim + 1):
-            assert_array_equal(dgms_offset[dim], dgms_orig[dim] - offset)
-
-
-def test_equivariance_regression():
-    """Make sure that, if `hypothesis` did not pick up a distance matrix like
-    the one in issue #31, then we test it by hand anyway, to avoid regressions.
-    """
-    maxdim = 1
-    kwargs = {"metric": "precomputed", "maxdim": maxdim}
-    dm = np.array([[0, 1, 3, 5, 4],
-                   [1, 0, 6, 7, 2],
-                   [3, 6, 0, 8, 9],
-                   [5, 7, 8, 0, 10],
-                   [4, 2, 9, 10, 0]], dtype=np.float32)
-
-    dm_flat = squareform(dm)
-    offsets = [np.median(dm_flat),
-               np.min(dm_flat),
-               np.max(dm_flat)]
-
-    dgms_orig = ripser(dm, **kwargs)["dgms"]
-
-    for offset in offsets:
-        dgms_offset = ripser(dm - offset, **kwargs)["dgms"]
-        for dim in range(maxdim + 1):
-            assert_array_equal(dgms_offset[dim], dgms_orig[dim] - offset)
-
-
-def test_optimized_distance_matrix():
-    """Ensure that using the optimized distance matrix computation when using
-    threshold produces the same results than using one with a threshold who
-    correspond to the enclosing radius.
-    """
-    X = np.random.default_rng(0).random((100, 3))
-    maxdim = 2
-    enclosing_radius = 0.8884447324918705
-
-    dgms = ripser(X, maxdim=maxdim)["dgms"]
-    dgms_thresh = ripser(X, maxdim=maxdim, thresh=enclosing_radius)["dgms"]
-
-    for dim, dgm in enumerate(dgms):
-        assert_array_equal(dgm, dgms_thresh[dim])
-
-
-def test_dense_finite_thresh_zero_edges():
-    """Check that if a dense distance matrix and a finite threshold are passed,
-    and some edges are zero, these edges are not treated as absent. Serves as
-    a regression test for issue #55."""
-    dm = np.array([[0., 0.],
-                   [0., 0.]])
-    dgm_0 = ripser(dm)["dgms"][0]
-    dgm_0_finite_thresh = ripser(dm, thresh=1.)["dgms"][0]
-    dgm_0_exp = np.array([[0., np.inf]])
-    assert_array_equal(dgm_0, dgm_0_exp)
-    assert_array_equal(dgm_0_finite_thresh, dgm_0_exp)
-
-
-def test_unsupported_coefficient():
-    from gph.modules import gph_ripser
-
-    X = squareform(pdist(np.random.random((10, 3))))
-
-    # Verifies that an exception is thrown if the coefficient value passed
-    # is not a prime number
-    with pytest.raises(ValueError):
-        ripser(X, metric='precomputed', coeff=4)
-
-    # Verifies that an exception is thrown if the coefficient value passed
-    # is bigger that the maximal value supported
-    with pytest.raises(ValueError):
-        ripser(X, metric='precomputed',
-               coeff=gph_ripser.get_max_coefficient_field_supported()+1)
-
-
-@settings(deadline=500)
-@given(dm_dense=get_dense_distance_matrices())
-def test_non_0_diagonal_internal_representation(dm_dense):
-    """Checks that, when passing a full distance matrix with non-zero values in
-    the diagonal, the result is the same regardless of whether the input is in
-    dense or sparse format."""
-    diagonal = np.random.random(dm_dense.shape[0])
-
-    # Ensure that all entries are bigger than the diagonal
-    dm_dense = dm_dense + 1
-    np.fill_diagonal(dm_dense, diagonal)
-
-    dgms1 = ripser(dm_dense, maxdim=2, metric='precomputed')['dgms']
-    dgms2 = ripser(coo_matrix(dm_dense), maxdim=2,
-                   metric='precomputed')['dgms']
-
-    for bars1, bars2 in zip(dgms1, dgms2):
-        assert_array_equal(bars1, bars2)
-
-
-def test_infinite_deaths_always_essential():
-    """Regression test for issue #37"""
-    diamond_dm = np.array(
-        [[0,      1,      np.inf, 1,      1,      1],
-         [0,      0,      1,      np.inf, 1,      1],
-         [0,      0,      0,      1,      1,      1],
-         [0,      0,      0,      0,      1,      1],
-         [0,      0,      0,      0,      0,      np.inf],
-         [0,      0,      0,      0,      0,      0]],
-        dtype=np.float64
-    )
-    diamond_dm += diamond_dm.T
-
-    gens = ripser(diamond_dm, metric="precomputed", maxdim=2,
-                  return_generators=True)["gens"]
-
-    gens_fin_dim1 = gens[1][1]
-
-    # With this example no finite generators in dimension 1 shall be found
-    assert len(gens_fin_dim1) == 0
+import numpy as np
+import pytest
+from hypothesis import given, settings
+from hypothesis.extra.numpy import arrays
+from hypothesis.strategies import floats, integers, composite
+from numpy.testing import assert_almost_equal, assert_array_equal
+from scipy.sparse import coo_matrix
+from scipy.spatial.distance import pdist, squareform
+
+from gph import ripser_parallel as ripser
+
+
+def make_dm_symmetric(dm):
+    # Extract strict upper diagonal and make symmetric
+    dm = np.triu(dm.astype(np.float32), k=1)
+    return dm + dm.T
+
+
+@composite
+def get_dense_distance_matrices(draw):
+    """Generate 2d dense square arrays of floats, with zero along the
+    diagonal."""
+    shapes = draw(integers(min_value=2, max_value=30))
+    dm = draw(arrays(dtype=float,
+                     elements=floats(allow_nan=False,
+                                     allow_infinity=True,
+                                     min_value=0,
+                                     exclude_min=True,
+                                     width=32),
+                     shape=(shapes, shapes), unique=False))
+    return make_dm_symmetric(dm)
+
+
+@composite
+def get_sparse_distance_matrices(draw):
+    """Generate 2d upper triangular sparse matrices of floats, with zero along
+    the diagonal."""
+    shapes = draw(integers(min_value=2, max_value=40))
+    dm = draw(arrays(dtype=float,
+                     elements=floats(allow_nan=False,
+                                     allow_infinity=True,
+                                     min_value=0,
+                                     exclude_min=True,
+                                     width=32),
+                     shape=(shapes, shapes), unique=False))
+    dm = np.triu(dm.astype(np.float32), k=1)
+    dm = coo_matrix(dm)
+    row, col, data = dm.row, dm.col, dm.data
+    not_inf_idx = data != np.inf
+    row = row[not_inf_idx]
+    col = col[not_inf_idx]
+    data = data[not_inf_idx]
+    shape_kwargs = {} if data.size else {"shape": (0, 0)}
+    dm = coo_matrix((data, (row, col)), **shape_kwargs)
+    return dm
+
+
+@settings(deadline=500)
+@given(dm=get_sparse_distance_matrices())
+def test_coo_below_diagonal_and_mixed_same_as_above(dm):
+    """Test that if we feed sparse matrices representing the same undirected
+    weighted graph we obtain the same results regardless of whether all entries
+    are above the diagonal, all are below the diagonal, or neither.
+    Furthermore, test that conflicts between stored data in the upper and lower
+    triangle are resolved in favour of the upper triangle."""
+    ripser_kwargs = {"maxdim": 2, "metric": "precomputed"}
+
+    pd_above = ripser(dm, **ripser_kwargs)['dgms']
+
+    pd_below = ripser(dm.T, **ripser_kwargs)['dgms']
+
+    _row, _col, _data = dm.row, dm.col, dm.data
+    coo_shape_kwargs = {} if _data.size else {"shape": (0, 0)}
+    to_transpose_mask = np.full(len(_row), False)
+    to_transpose_mask[np.random.choice(np.arange(len(_row)),
+                                       size=len(_row) // 2,
+                                       replace=False)] = True
+    row = np.concatenate([_col[to_transpose_mask], _row[~to_transpose_mask]])
+    col = np.concatenate([_row[to_transpose_mask], _col[~to_transpose_mask]])
+    dm_mixed = coo_matrix((_data, (row, col)), **coo_shape_kwargs)
+    pd_mixed = ripser(dm_mixed, **ripser_kwargs)['dgms']
+
+    row = np.concatenate([row, _row[to_transpose_mask]])
+    col = np.concatenate([col, _col[to_transpose_mask]])
+    data = np.random.random(len(row))
+    data[:len(_row)] = _data
+    dm_conflicts = coo_matrix((data, (row, col)), **coo_shape_kwargs)
+    pd_conflicts = ripser(dm_conflicts, **ripser_kwargs)['dgms']
+
+    for i in range(ripser_kwargs["maxdim"] + 1):
+        pd_above[i] = np.sort(pd_above[i], axis=0)
+        pd_below[i] = np.sort(pd_below[i], axis=0)
+        pd_mixed[i] = np.sort(pd_mixed[i], axis=0)
+        pd_conflicts[i] = np.sort(pd_conflicts[i], axis=0)
+        assert_almost_equal(pd_above[i], pd_below[i])
+
+
+@pytest.mark.parametrize('thresh', [False, True])
+@pytest.mark.parametrize('coeff', [2, 7])
+@settings(deadline=500)
+@given(dm=get_dense_distance_matrices())
+def test_collapse_consistent_with_no_collapse_dense(thresh, coeff, dm):
+    thresh = np.max(dm) / 2 if thresh else np.inf
+    maxdim = 3
+    pd_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
+                         metric='precomputed', collapse_edges=True)['dgms']
+    pd_no_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
+                            metric='precomputed', collapse_edges=False)['dgms']
+    for i in range(maxdim + 1):
+        pd_collapse[i] = np.sort(pd_collapse[i], axis=0)
+        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
+        assert_almost_equal(pd_collapse[i], pd_no_collapse[i])
+
+
+@pytest.mark.parametrize('thresh', [False, True])
+@pytest.mark.parametrize('coeff', [2, 7])
+@settings(deadline=500)
+@given(dm=get_sparse_distance_matrices())
+def test_collapse_consistent_with_no_collapse_coo(thresh, coeff, dm):
+    if thresh and dm.nnz:
+        thresh = np.max(dm) / 2
+    else:
+        thresh = np.inf
+    maxdim = 3
+    pd_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
+                         metric='precomputed', collapse_edges=True)['dgms']
+    pd_no_collapse = ripser(dm, thresh=thresh, maxdim=maxdim, coeff=coeff,
+                            metric='precomputed', collapse_edges=False)['dgms']
+    for i in range(maxdim + 1):
+        pd_collapse[i] = np.sort(pd_collapse[i], axis=0)
+        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
+        assert_almost_equal(pd_collapse[i], pd_no_collapse[i])
+
+
+def test_collapser_with_negative_weights():
+    """Test that collapser works as expected when some of the vertex and edge
+    weights are negative."""
+    n_points = 20
+    dm = make_dm_symmetric(np.random.random((n_points, n_points)))
+    np.fill_diagonal(dm, -np.random.random(n_points))
+    dm -= 0.2
+    dm_sparse = coo_matrix(dm)
+
+    maxdim = 2
+    pd_collapse_dense = ripser(dm, metric='precomputed', maxdim=maxdim,
+                               collapse_edges=True)['dgms']
+    pd_collapse_sparse = ripser(dm_sparse, metric='precomputed',
+                                maxdim=maxdim, collapse_edges=True)['dgms']
+    pd_no_collapse = ripser(dm, metric='precomputed', maxdim=maxdim,
+                            collapse_edges=False)['dgms']
+
+    for i in range(maxdim + 1):
+        pd_collapse_dense[i] = np.sort(pd_collapse_dense[i], axis=0)
+        pd_collapse_sparse[i] = np.sort(pd_collapse_sparse[i], axis=0)
+        pd_no_collapse[i] = np.sort(pd_no_collapse[i], axis=0)
+        assert_almost_equal(pd_collapse_dense[i], pd_no_collapse[i])
+        assert_almost_equal(pd_collapse_sparse[i], pd_no_collapse[i])
+
+
+def test_coo_results_independent_of_order():
+    """Regression test for PR #465"""
+    data = np.array([6., 8., 2., 4., 5., 9., 10., 3., 1., 1.])
+    row = np.array([0, 0, 0, 0, 1, 1, 1, 2, 2, 3])
+    col = np.array([4, 1, 3, 2, 4, 3, 2, 3, 4, 4])
+    dm = coo_matrix((data, (row, col)))
+    diagrams = ripser(dm, metric="precomputed")['dgms']
+    diagrams_csr = ripser(dm.tocsr(), metric="precomputed")['dgms']
+    expected = [np.array([[0., 1.],
+                          [0., 1.],
+                          [0., 2.],
+                          [0., 5.],
+                          [0., np.inf]]),
+                np.array([], dtype=float).reshape(0, 2)]
+    for i in range(2):
+        assert np.array_equal(diagrams[i], expected[i])
+        assert np.array_equal(diagrams_csr[i], expected[i])
+
+
+@settings(deadline=500)
+@given(dm=get_dense_distance_matrices())
+def test_multithread_consistent(dm):
+    """Test that varying the number of threads produces consistent results"""
+    maxdim = 3
+    nb_threads_to_test = [1, 2, 3, 4, 5]
+    res = []
+    for nb_threads in nb_threads_to_test:
+        res.append(ripser(dm, maxdim=maxdim, metric='precomputed',
+                          n_threads=nb_threads)['dgms'])
+    for dim in range(maxdim + 1):
+        res[0][dim] = np.sort(res[0][dim], axis=0)
+        for i in range(1, len(res)):
+            res[i][dim] = np.sort(res[i][dim], axis=0)
+            assert_almost_equal(res[0][dim], res[i][dim])
+
+
+def test_gens_edge_in_dm_and_sorted():
+    """This test verifies that the representative simplicies, the index of the
+    vertices matches the corresponding edge in the distance matrix and that
+    the gens are aligned with the correponding barcodes"""
+    X = squareform(pdist(np.random.random((100, 3))))
+
+    ret = ripser(X, metric='precomputed', maxdim=3, thresh=np.inf,
+                 collapse_edges=False, return_generators=True)
+
+    barcodes = ret['dgms']
+    gens = ret['gens']
+
+    for dim, bar_in_dim in enumerate(barcodes):
+        idx_essential = 0
+        idx_finite = 0
+        for barcode in bar_in_dim:
+            if dim == 0 and barcode[1] != np.inf:
+                # Verifies gens in dim 0, discards essential ones
+                gens_of_barcode = gens[0][idx_finite]
+                assert np.isclose(barcode[1],
+                                  X[gens_of_barcode[1]][gens_of_barcode[2]])
+                idx_finite = idx_finite + 1
+            if dim > 0:
+                # Verifies gens in dim > 0, expects first all non essential
+                # barcodes and then the finite ones
+                if barcode[1] != np.inf:
+                    gens_of_barcode = gens[1][dim-1][idx_finite]
+                    assert np.isclose(barcode[0],
+                                      X[gens_of_barcode[0]][gens_of_barcode[1]]
+                                      )
+                    assert np.isclose(barcode[1],
+                                      X[gens_of_barcode[2]][gens_of_barcode[3]]
+                                      )
+                    idx_finite = idx_finite + 1
+                else:
+                    gens_of_barcode = gens[3][dim-1][idx_essential]
+                    assert np.isclose(barcode[0],
+                                      X[gens_of_barcode[0]][gens_of_barcode[1]]
+                                      )
+                    idx_essential = idx_essential + 1
+
+
+def test_gens_with_collapser():
+    """This test ensures that you cannot use collapser and
+    retrieve generators. This is a temporary behavior."""
+    X = squareform(pdist(np.random.random((10, 3))))
+
+    with pytest.raises(NotImplementedError):
+        ripser(X, metric='precomputed', collapse_edges=True,
+               return_generators=True)
+
+
+@settings(deadline=500)
+@given(dm=get_dense_distance_matrices())
+@pytest.mark.parametrize('format', ['dense', 'sparse'])
+def test_gens_non_0_diagonal_dim0(dm, format):
+    np.fill_diagonal(dm, np.random.uniform(low=0, high=np.amin(dm),
+                                           size=(dm.shape[0])))
+    x_len = dm.shape[0]
+    if format == 'dense':
+        X = dm
+    else:
+        X = coo_matrix(dm).tocsr()
+
+    ret = ripser(X, metric='precomputed', return_generators=True)
+
+    dgms_0 = ret['dgms'][0]
+    gens_fin_0 = ret['gens'][0]
+    gens_ess_0 = ret['gens'][2]
+
+    # Verifies that the number of essential and finite generators
+    # combined is equal to the number of points in the point cloud
+    assert (x_len - len(gens_ess_0)) == len(gens_fin_0)
+
+    # Verifies that the birth indices for essential and finite
+    # representatives are unique
+    assert len(np.unique(np.sort(gens_fin_0[:, 0]))) == len(gens_fin_0[:, 0])
+    assert len(np.unique(np.sort(gens_ess_0))) == len(gens_ess_0)
+    # Verifies that there are no duplicates between finite and essential
+    # And also the other way around
+    assert len([x for x in gens_fin_0[:, 0] if x in gens_ess_0]) == 0
+    assert len([x for x in gens_ess_0 if x in gens_fin_0[:, 0]]) == 0
+
+    for barcode, rp in zip(dgms_0, gens_fin_0):
+        # Verify birth of dim-0 finite representative
+        # The birth is located on the diagonal
+        assert np.isclose(barcode[0], X[rp[0], rp[0]])
+
+        # Verify death of dim-0 finite representative
+        assert np.isclose(barcode[1], X[rp[1], rp[2]])
+
+    for barcode, rp in zip(dgms_0[len(dgms_0):], gens_ess_0):
+        # Verify birth of dim-0 essential representative
+        # The birth is located on the diagonal
+        assert np.isclose(barcode[0], X[rp, rp])
+
+
+def test_gens_order_vertices_higher_dimension():
+    """This test verifies that function `get_youngest_edge_simplex` returns the
+    correct vertices. It should return the edge with the largest diameter in
+    the simplex and, if several are present with the same diameter, the oldest
+    one in the reverse colexicographic order used to build the simplexwise
+    refinement of the Vietoris-Rips filtration."""
+    diamond = np.array(
+        [[0,      1,    100,      1,      1,      1],
+         [0,      0,      1,    100,      1,      1],
+         [0,      0,      0,      1,      1,      1],
+         [0,      0,      0,      0,      1,      1],
+         [0,      0,      0,      0,      0,    100],
+         [0,      0,      0,      0,      0,      0]],
+        dtype=np.float64)
+
+    diamond += diamond.T
+
+    gens = ripser(diamond, maxdim=2, return_generators=True)['gens']
+    gens_fin_dim2 = gens[1][1]
+
+    assert len(gens_fin_dim2) == 1
+    assert np.array_equal(gens_fin_dim2[0], np.array([1, 0, 5, 4]))
+
+
+def test_ph_maxdim_0():
+    """Regression test for issue #39, an issue was found when only computing
+    up to dimension 0. The test also compares the results of dimension 0
+    when maxdim=1 and maxdim=0"""
+    X = np.array([[1., 2], [3, 4], [5, 0]])
+    res_maxdim_0 = ripser(X, maxdim=0)['dgms'][0]
+    res_maxdim_1 = ripser(X, maxdim=1)['dgms'][0]
+
+    # Verifies that the two computations lead to the same barcodes
+    assert_array_equal(res_maxdim_0, res_maxdim_1)
+
+
+@settings(deadline=500)
+@given(dm=get_dense_distance_matrices())
+def test_equivariance(dm):
+    """Test that if we shift all entries (diagonal or not) in the input matrix
+    by a constant then the barcodes are also shifted by that constant. Doubles
+    also as a regression test for issue #31."""
+    maxdim = 1
+    kwargs = {"metric": "precomputed", "maxdim": maxdim}
+
+    # - Median may or may not make some edges zero, and will make some edges
+    #   negative and all vertex weights negative
+    # - Min is guaranteed to make at least one edge exactly zero, and all
+    #   vertex weights negative
+    # - Max is guaranteed to make all edge and vertex weights non-positive (or
+    #   infinite)
+    dm_flat = squareform(dm, checks=False)  # Get strict upper diagonal
+    dm_finite_nonzero_flat_sorted = np.sort(
+        dm_flat[np.logical_and(dm_flat > 0, dm_flat < np.inf)]
+        )  # Filter out zero values and infinite values, and sort
+    # This test will fail if val - offset = -offset numerically for some entry
+    # val in dm, because this will make some 0-dimensional classes disappear
+    # (they are born dead)
+    offsets = [0, 0, 0]  # Fallback if no edge weights are finite and positive
+    if len(dm_finite_nonzero_flat_sorted):
+        offset_cand = [np.float32(np.median(dm_finite_nonzero_flat_sorted)),
+                       np.min(dm_finite_nonzero_flat_sorted),
+                       np.max(dm_finite_nonzero_flat_sorted)]
+        for i, offset in enumerate(offset_cand):
+            if not np.any(dm - offset == -offset):
+                offsets[i] = offset_cand
+
+    dgms_orig = ripser(dm, **kwargs)["dgms"]
+
+    for offset in offsets:
+        dgms_offset = ripser(dm - offset, **kwargs)["dgms"]
+        for dim in range(maxdim + 1):
+            assert_array_equal(dgms_offset[dim], dgms_orig[dim] - offset)
+
+
+def test_equivariance_regression():
+    """Make sure that, if `hypothesis` did not pick up a distance matrix like
+    the one in issue #31, then we test it by hand anyway, to avoid regressions.
+    """
+    maxdim = 1
+    kwargs = {"metric": "precomputed", "maxdim": maxdim}
+    dm = np.array([[0, 1, 3, 5, 4],
+                   [1, 0, 6, 7, 2],
+                   [3, 6, 0, 8, 9],
+                   [5, 7, 8, 0, 10],
+                   [4, 2, 9, 10, 0]], dtype=np.float32)
+
+    dm_flat = squareform(dm)
+    offsets = [np.median(dm_flat),
+               np.min(dm_flat),
+               np.max(dm_flat)]
+
+    dgms_orig = ripser(dm, **kwargs)["dgms"]
+
+    for offset in offsets:
+        dgms_offset = ripser(dm - offset, **kwargs)["dgms"]
+        for dim in range(maxdim + 1):
+            assert_array_equal(dgms_offset[dim], dgms_orig[dim] - offset)
+
+
+def test_optimized_distance_matrix():
+    """Ensure that using the optimized distance matrix computation when using
+    threshold produces the same results than using one with a threshold who
+    correspond to the enclosing radius.
+    """
+    X = np.random.default_rng(0).random((100, 3))
+    maxdim = 2
+    enclosing_radius = 0.8884447324918705
+
+    dgms = ripser(X, maxdim=maxdim)["dgms"]
+    dgms_thresh = ripser(X, maxdim=maxdim, thresh=enclosing_radius)["dgms"]
+
+    for dim, dgm in enumerate(dgms):
+        assert_array_equal(dgm, dgms_thresh[dim])
+
+
+def test_dense_finite_thresh_zero_edges():
+    """Check that if a dense distance matrix and a finite threshold are passed,
+    and some edges are zero, these edges are not treated as absent. Serves as
+    a regression test for issue #55."""
+    dm = np.array([[0., 0.],
+                   [0., 0.]])
+    dgm_0 = ripser(dm)["dgms"][0]
+    dgm_0_finite_thresh = ripser(dm, thresh=1.)["dgms"][0]
+    dgm_0_exp = np.array([[0., np.inf]])
+    assert_array_equal(dgm_0, dgm_0_exp)
+    assert_array_equal(dgm_0_finite_thresh, dgm_0_exp)
+
+
+def test_unsupported_coefficient():
+    from gph.modules import gph_ripser
+
+    X = squareform(pdist(np.random.random((10, 3))))
+
+    # Verifies that an exception is thrown if the coefficient value passed
+    # is not a prime number
+    with pytest.raises(ValueError):
+        ripser(X, metric='precomputed', coeff=4)
+
+    # Verifies that an exception is thrown if the coefficient value passed
+    # is bigger that the maximal value supported
+    with pytest.raises(ValueError):
+        ripser(X, metric='precomputed',
+               coeff=gph_ripser.get_max_coefficient_field_supported()+1)
+
+
+@settings(deadline=500)
+@given(dm_dense=get_dense_distance_matrices())
+def test_non_0_diagonal_internal_representation(dm_dense):
+    """Checks that, when passing a full distance matrix with non-zero values in
+    the diagonal, the result is the same regardless of whether the input is in
+    dense or sparse format."""
+    diagonal = np.random.random(dm_dense.shape[0])
+
+    # Ensure that all entries are bigger than the diagonal
+    dm_dense = dm_dense + 1
+    np.fill_diagonal(dm_dense, diagonal)
+
+    dgms1 = ripser(dm_dense, maxdim=2, metric='precomputed')['dgms']
+    dgms2 = ripser(coo_matrix(dm_dense), maxdim=2,
+                   metric='precomputed')['dgms']
+
+    for bars1, bars2 in zip(dgms1, dgms2):
+        assert_array_equal(bars1, bars2)
+
+
+def test_infinite_deaths_always_essential():
+    """Regression test for issue #37"""
+    diamond_dm = np.array(
+        [[0,      1,      np.inf, 1,      1,      1],
+         [0,      0,      1,      np.inf, 1,      1],
+         [0,      0,      0,      1,      1,      1],
+         [0,      0,      0,      0,      1,      1],
+         [0,      0,      0,      0,      0,      np.inf],
+         [0,      0,      0,      0,      0,      0]],
+        dtype=np.float64
+    )
+    diamond_dm += diamond_dm.T
+
+    gens = ripser(diamond_dm, metric="precomputed", maxdim=2,
+                  return_generators=True)["gens"]
+
+    gens_fin_dim1 = gens[1][1]
+
+    # With this example no finite generators in dimension 1 shall be found
+    assert len(gens_fin_dim1) == 0
```

## gph/python/test/test_wrp.py

 * *Ordering differences only*

```diff
@@ -1,93 +1,93 @@
-import numpy as np
-import pytest
-from numpy.testing import assert_almost_equal
-from scipy.spatial.distance import squareform
-from scipy.spatial.distance import pdist
-from scipy.sparse import csr_matrix
-
-from gph import ripser_parallel as ripser
-
-
-X_pc = np.array([[2., 2.47942554],
-                 [2.47942554, 2.84147098],
-                 [2.98935825, 2.79848711],
-                 [2.79848711, 2.41211849],
-                 [2.41211849, 1.92484888]])
-
-X_dist = squareform(pdist(X_pc))
-
-X_pc_sparse = csr_matrix(X_pc)
-X_dist_sparse = csr_matrix(X_dist)
-
-X_dist_disconnected = np.array([[0, np.inf], [np.inf, 0]])
-
-X_vrp_exp = [
-    np.array([[0., 0.43094373],
-              [0., 0.5117411],
-              [0., 0.60077095],
-              [0., 0.62186205],
-              [0., np.inf]]),
-    np.array([[0.69093919, 0.80131882]])
-    ]
-
-
-def test_wrp_notimplemented_string_weights():
-    with pytest.raises(ValueError, match="'foo' passed for `weights` but the "
-                                         "only allowed string is 'DTM'"):
-        ripser(X_pc, weights="foo")
-
-
-def test_wrp_notimplemented_p():
-    with pytest.raises(NotImplementedError):
-        ripser(X_pc, weights="DTM", weight_params={"p": 1.2})
-
-
-@pytest.mark.parametrize("X, metric", [(X_pc, "euclidean"),
-                                       (X_pc_sparse, "euclidean"),
-                                       (X_dist, "precomputed"),
-                                       (X_dist_sparse, "precomputed")])
-@pytest.mark.parametrize("weight_params", [{"p": 1}, {"p": 2}, {"p": np.inf}])
-@pytest.mark.parametrize("collapse_edges", [True, False])
-@pytest.mark.parametrize("thresh", [np.inf, 0.81])
-def test_wrp_same_as_vrp_when_zero_weights(X, metric, weight_params,
-                                           collapse_edges, thresh):
-    def weights(x): return np.zeros(x.shape[0])
-    weights = weights(X)
-    X_wrp = ripser(X, weights=weights,
-                   weight_params=weight_params,
-                   metric=metric,
-                   collapse_edges=collapse_edges,
-                   thresh=thresh)['dgms']
-
-    for i in range(2):
-        assert_almost_equal(X_wrp[i], X_vrp_exp[i])
-
-
-X_dtm_exp = {1: [np.array([[0.95338798, 1.474913],
-                           [1.23621261, 1.51234496],
-                           [1.21673107, 1.68583047],
-                           [1.30722439, 1.73876917],
-                           [0.92658985, np.inf]]),
-                 np.empty((0, 2))],
-             2: [np.array([[0.95338798, 1.08187652],
-                           [1.23621261, 1.2369417],
-                           [1.21673107, 1.26971364],
-                           [1.30722439, 1.33688354],
-                           [0.92658985, np.inf]]),
-                 np.empty((0, 2))],
-             np.inf: [np.array([[0.9265898, np.inf]]),
-                      np.empty((0, 2))]}
-
-
-@pytest.mark.parametrize("X, metric", [(X_pc, "euclidean"),
-                                       (X_pc_sparse, "euclidean"),
-                                       (X_dist, "precomputed"),
-                                       (X_dist_sparse, "precomputed")])
-@pytest.mark.parametrize("weight_params", [{"p": 1}, {"p": 2}, {"p": np.inf}])
-@pytest.mark.parametrize("collapse_edges", [True, False])
-def test_dtm(X, metric, weight_params, collapse_edges):
-    X_dtm = ripser(X, weights="DTM", weight_params=weight_params,
-                   metric=metric, collapse_edges=collapse_edges)['dgms']
-
-    for i in range(2):
-        assert_almost_equal(X_dtm[i], X_dtm_exp[weight_params["p"]][i])
+import numpy as np
+import pytest
+from numpy.testing import assert_almost_equal
+from scipy.spatial.distance import squareform
+from scipy.spatial.distance import pdist
+from scipy.sparse import csr_matrix
+
+from gph import ripser_parallel as ripser
+
+
+X_pc = np.array([[2., 2.47942554],
+                 [2.47942554, 2.84147098],
+                 [2.98935825, 2.79848711],
+                 [2.79848711, 2.41211849],
+                 [2.41211849, 1.92484888]])
+
+X_dist = squareform(pdist(X_pc))
+
+X_pc_sparse = csr_matrix(X_pc)
+X_dist_sparse = csr_matrix(X_dist)
+
+X_dist_disconnected = np.array([[0, np.inf], [np.inf, 0]])
+
+X_vrp_exp = [
+    np.array([[0., 0.43094373],
+              [0., 0.5117411],
+              [0., 0.60077095],
+              [0., 0.62186205],
+              [0., np.inf]]),
+    np.array([[0.69093919, 0.80131882]])
+    ]
+
+
+def test_wrp_notimplemented_string_weights():
+    with pytest.raises(ValueError, match="'foo' passed for `weights` but the "
+                                         "only allowed string is 'DTM'"):
+        ripser(X_pc, weights="foo")
+
+
+def test_wrp_notimplemented_p():
+    with pytest.raises(NotImplementedError):
+        ripser(X_pc, weights="DTM", weight_params={"p": 1.2})
+
+
+@pytest.mark.parametrize("X, metric", [(X_pc, "euclidean"),
+                                       (X_pc_sparse, "euclidean"),
+                                       (X_dist, "precomputed"),
+                                       (X_dist_sparse, "precomputed")])
+@pytest.mark.parametrize("weight_params", [{"p": 1}, {"p": 2}, {"p": np.inf}])
+@pytest.mark.parametrize("collapse_edges", [True, False])
+@pytest.mark.parametrize("thresh", [np.inf, 0.81])
+def test_wrp_same_as_vrp_when_zero_weights(X, metric, weight_params,
+                                           collapse_edges, thresh):
+    def weights(x): return np.zeros(x.shape[0])
+    weights = weights(X)
+    X_wrp = ripser(X, weights=weights,
+                   weight_params=weight_params,
+                   metric=metric,
+                   collapse_edges=collapse_edges,
+                   thresh=thresh)['dgms']
+
+    for i in range(2):
+        assert_almost_equal(X_wrp[i], X_vrp_exp[i])
+
+
+X_dtm_exp = {1: [np.array([[0.95338798, 1.474913],
+                           [1.23621261, 1.51234496],
+                           [1.21673107, 1.68583047],
+                           [1.30722439, 1.73876917],
+                           [0.92658985, np.inf]]),
+                 np.empty((0, 2))],
+             2: [np.array([[0.95338798, 1.08187652],
+                           [1.23621261, 1.2369417],
+                           [1.21673107, 1.26971364],
+                           [1.30722439, 1.33688354],
+                           [0.92658985, np.inf]]),
+                 np.empty((0, 2))],
+             np.inf: [np.array([[0.9265898, np.inf]]),
+                      np.empty((0, 2))]}
+
+
+@pytest.mark.parametrize("X, metric", [(X_pc, "euclidean"),
+                                       (X_pc_sparse, "euclidean"),
+                                       (X_dist, "precomputed"),
+                                       (X_dist_sparse, "precomputed")])
+@pytest.mark.parametrize("weight_params", [{"p": 1}, {"p": 2}, {"p": np.inf}])
+@pytest.mark.parametrize("collapse_edges", [True, False])
+def test_dtm(X, metric, weight_params, collapse_edges):
+    X_dtm = ripser(X, weights="DTM", weight_params=weight_params,
+                   metric=metric, collapse_edges=collapse_edges)['dgms']
+
+    for i in range(2):
+        assert_almost_equal(X_dtm[i], X_dtm_exp[weight_params["p"]][i])
```

## Comparing `giotto_ph-0.2.3.dist-info/LICENSE` & `giotto_ph-0.2.4.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,676 +1,676 @@
-Copyright 2021 L2F SA.
-
-If you need a different distribution license, please contact the L2F team
-at business@l2f.ch.
-
-Licensed under the GNU Affero General Public License (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License below or at https://www.gnu.org/licenses/agpl-3.0.html
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+Copyright 2021 L2F SA.
+
+If you need a different distribution license, please contact the L2F team
+at business@l2f.ch.
+
+Licensed under the GNU Affero General Public License (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License below or at https://www.gnu.org/licenses/agpl-3.0.html
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

## Comparing `giotto_ph-0.2.3.dist-info/RECORD` & `giotto_ph-0.2.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-gph/__init__.py,sha256=HmQTSsXVNzn_4uZdkKn8zJc9X7tVzuBbtwM4FIBoUTY,149
-gph/_version.py,sha256=5-p8t5VwEtw3yXrvypTVieUFHIgaTPXxjA4by6a5op0,620
-gph/modules/gph_collapser.cp39-win_amd64.pyd,sha256=6oVBORk2-HRvuTeyKszBvJLSIroDpTFPXybYEGOaLNU,139264
-gph/modules/gph_ripser.cp39-win_amd64.pyd,sha256=ocfY58haFFm6Yp8lVHrTkVGVNT772tDatRfrn6OhI6w,338944
-gph/modules/gph_ripser_coeff.cp39-win_amd64.pyd,sha256=JlXLBUBBK-t6dywDxe56tX0enzFja7q3AQwoWXfipE8,343040
-gph/python/__init__.py,sha256=WtwHCYEMYScWKy4oHKM8euZr76_DLGCazX6ayf9n9tg,89
-gph/python/ripser_interface.py,sha256=oR-RTQm_TTiFYSmLnb16ca7RYcJBGl0GEVzqHF7LFTg,28880
-gph/python/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gph/python/test/test_collapser.py,sha256=AxOgbvN7RivvIc0YH9JcOIyY-WkxGHVUvYxu4Ie8cDI,2248
-gph/python/test/test_ripser.py,sha256=fndezRyFgqzymUrrRbRr-2e3F-w8t0N964mA28hWTEM,20115
-gph/python/test/test_wrp.py,sha256=sTB5Q3el8Sd99fd4-ySmt3NZ5uXtEWRStB1ZYYt4ToM,3645
-giotto_ph-0.2.3.dist-info/LICENSE,sha256=K2mHDYGGPDF90WsUydGOBt1SVUHUJRX3U460v8e5HnM,35868
-giotto_ph-0.2.3.dist-info/METADATA,sha256=kuTYAhoU-u443GXDdfuV8x5YpfdvFCIy4xiSMaBmK5s,2648
-giotto_ph-0.2.3.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-giotto_ph-0.2.3.dist-info/top_level.txt,sha256=VY7JNFK1ziu4gNFeDEd7UqJthhMsYdylwSXFxf4CX6U,4
-giotto_ph-0.2.3.dist-info/RECORD,,
+gph/__init__.py,sha256=Kp2TDJvgynZcWFsi9FNPfjd_ciAEDz_bIRnXIsjywhY,141
+gph/_version.py,sha256=kC9KnedO6JIwHdV7D461h1uui1bME6CRtwBz04fGnu4,598
+gph/modules/gph_ripser.cpython-39-x86_64-linux-gnu.so,sha256=Uf635FAVL3TbtT1C7TkV7WxNo61pOFvN8r4b2FynRI8,545400
+gph/modules/gph_ripser_coeff.cpython-39-x86_64-linux-gnu.so,sha256=C6IC9LvOj2iDMymxA2VlNCM4_yWPwxcGNSDnQCjt1zw,561784
+gph/modules/gph_collapser.cpython-39-x86_64-linux-gnu.so,sha256=ieKgMn_wXTA68d9lafMOKnszYAfwVAPZ51CzHwYhdEU,208744
+gph/python/__init__.py,sha256=1QXkIWM8CgI_Ld3ZAKSzHhAPo8nYnTChD8q-paAjR8A,84
+gph/python/ripser_interface.py,sha256=91UXlgPMWULqC_WLTChpZaouANyI9Bo6z5JUYvQaI9U,28232
+gph/python/test/test_wrp.py,sha256=vPIdJL4DdLOyzsdC1bnUpiJwgvTzno4pcT-F7M8vHm0,3552
+gph/python/test/test_ripser.py,sha256=2nmqw3RwosX9rJ9uOp_buhU0vt6b4BCImG4YTzYKb1M,19637
+gph/python/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+gph/python/test/test_collapser.py,sha256=4Vlt2F73_i3_qq8g1WFC6JvVyTepFC6mRD8wjVNq2S4,2181
+giotto_ph-0.2.4.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+giotto_ph-0.2.4.dist-info/LICENSE,sha256=wiv9A2iMcIYnFR9B2R0f9McuWnQYBHxQ5zLh3j7mN4g,35192
+giotto_ph-0.2.4.dist-info/top_level.txt,sha256=VY7JNFK1ziu4gNFeDEd7UqJthhMsYdylwSXFxf4CX6U,4
+giotto_ph-0.2.4.dist-info/RECORD,,
+giotto_ph-0.2.4.dist-info/METADATA,sha256=x6GQt1tGGyFj9_CRMNecC7V36oR8uToX44R1zX01ziE,10398
```

