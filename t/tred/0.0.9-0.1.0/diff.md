# Comparing `tmp/tred-0.0.9.tar.gz` & `tmp/tred-0.1.0.tar.gz`

## Comparing `tred-0.0.9.tar` & `tred-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 tred-0.0.9/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 tred-0.0.9/tests/test_m_transforms.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 tred-0.0.9/tests/test_tensor_ops.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 tred-0.0.9/tests/test_tensor_pca.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tred-0.0.9/tred/__init__.py
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 tred-0.0.9/tred/_m_transforms.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 tred-0.0.9/tred/_tensor_ops.py
--rw-r--r--   0        0        0    21257 2020-02-02 00:00:00.000000 tred-0.0.9/tred/_tensor_pca.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 tred-0.0.9/tred/_utils.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.0.9/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.0.9/LICENSE
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 tred-0.0.9/README.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tred-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.0/requirements.txt
+-rw-r--r--   0        0        0    19615 2020-02-02 00:00:00.000000 tred-0.1.0/examples/basic.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_m_transforms.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_tensor_pca.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tred-0.1.0/tred/__init__.py
+-rw-r--r--   0        0        0     8117 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_m_transforms.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_tensor_ops.py
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_tensor_pca.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 tred-0.1.0/tred/_utils.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.0/README.txt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.0/PKG-INFO
```

### Comparing `tred-0.0.9/tests/test_tensor_ops.py` & `tred-0.1.0/tests/test_tensor_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     C1 = 5
     C2 = 6
 
     rng = np.random.default_rng(seed=GLOBAL_SEED)
     n, p, t = tensor_shape
 
     # generate some compatibly sized tensors
-    A = rng.random(size=((n, p, t))) * C1 - include_negatives * 0.5 * C1
+    A = rng.random(size=(n, p, t)) * C1 - include_negatives * 0.5 * C1
 
     B = (
-        rng.random(size=((p, n + rectangular_offset, t))) * C2
+        rng.random(size=(p, n + rectangular_offset, t)) * C2
         - include_negatives * 0.5 * C2
     )
 
     # compute expected results using naive implementations
     fp_expected = np.zeros(shape=(n, n + rectangular_offset, t))
     for i in range(t):
         fp_expected[:, :, i] = A[:, :, i] @ B[:, :, i]
```

### Comparing `tred-0.0.9/tests/test_tensor_pca.py` & `tred-0.1.0/tests/test_tensor_pca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 from functools import reduce
 
 import numpy as np
 import pytest
 from numpy.testing import assert_allclose
+from scipy.stats import special_ortho_group
 
 from tred import (
     generate_default_m_transform_pair,
     TPCA,
     tsvdm,
     m_product,
+    generate_transform_pair_from_matrix,
     generate_dctii_m_transform_pair,
     generate_dstii_m_transform_pair,
 )
 
 
+GLOBAL_SEED = 1
+RNG = np.random.default_rng(seed=GLOBAL_SEED)
+
+
+def _dummy_random_orthogonal_m_transform_generator(t):
+    """Let's test a m-transform defined by a random orthogonal matrix too!"""
+    M_mat = special_ortho_group.rvs(t, random_state=RNG)
+    M, Minv = generate_transform_pair_from_matrix(M_mat)
+    return M, Minv
+
+
 def _dummy_default_transform_generator(t):
     """Return M=None, Minv=None to test default m-transform configuration"""
     return None, None
 
 
-GLOBAL_SEED = 1
-
 # various n, p, t sizes
 # ensure n > p, p > n inputs are tested
 TENSOR_SHAPES = [(4, 3, 2), (5, 7, 6), (2, 2, 6)]
 
 # m transforms to suit the tensor sizes above
 TRANSFORM_FAMILY_GENERATORS = [
+    _dummy_random_orthogonal_m_transform_generator,
     _dummy_default_transform_generator,
     generate_dctii_m_transform_pair,
     generate_dstii_m_transform_pair,
 ]
 
 # test tiny, small, medium, and large numbers
-ELEMENT_SCALES = [10**i for i in range(-4, 5, 2)]
+ELEMENT_SCALES = [10**i for i in range(-4, 5, 4)]
 
 
 def _check_fitted_tpca_close(tpca1, tpca2, rtol, atol):
     """Check all of the fitted attributes of the two tpca classes
     NOTE: unused at the moment, but will likely be useful in future tests
     """
     assert_allclose(tpca1.n_, tpca2.n_, rtol=rtol, atol=atol)
@@ -58,27 +70,34 @@
     assert_allclose(tpca1.rho_, tpca2.rho_, rtol=rtol, atol=atol)
 
 
 @pytest.mark.parametrize("tensor_shape", TENSOR_SHAPES)
 @pytest.mark.parametrize("element_scale", ELEMENT_SCALES)
 @pytest.mark.parametrize("include_negatives", [0, 1])
 @pytest.mark.parametrize("transform_generator", TRANSFORM_FAMILY_GENERATORS)
-def test_tsvdm(tensor_shape, element_scale, include_negatives, transform_generator):
+@pytest.mark.parametrize("return_full_frontal_slices", [True, False])
+def test_tsvdm(
+    tensor_shape,
+    element_scale,
+    include_negatives,
+    transform_generator,
+    return_full_frontal_slices,
+):
     rng = np.random.default_rng(seed=GLOBAL_SEED)
     n, p, t = tensor_shape
 
     # tensors of various sizes with uniformly distributed elements
     # within [0, element_scale) or [-0.5*element_scale, 0.5*element_scale)
     X = (
         rng.random(size=tensor_shape) * element_scale
         - include_negatives * 0.5 * element_scale
     )
 
     M, Minv = transform_generator(t)
-    U, S, V = tsvdm(X, M=M, Minv=Minv)
+    U, S, V = tsvdm(X, M=M, Minv=Minv, full_frontal_slices=return_full_frontal_slices)
     Vt = V.transpose(1, 0, 2)
 
     # make sure that the m-product below has a 'non-None' set of inputs for M and Minv
     if M is None:
         M, Minv = generate_default_m_transform_pair(t)
 
     def m_product_wrapper(A, B):
@@ -88,30 +107,36 @@
     X_reconstruct = reduce(m_product_wrapper, (U, S, Vt))
     assert_allclose(X, X_reconstruct)
 
 
 @pytest.mark.parametrize("tensor_shape", TENSOR_SHAPES)
 @pytest.mark.parametrize("element_scale", ELEMENT_SCALES)
 @pytest.mark.parametrize("include_negatives", [0, 1])
-@pytest.mark.parametrize("n_components", [None, 1, 6, 0.3, 0.8])
+@pytest.mark.parametrize("n_components", [None, 1, 6, 0.8])
+@pytest.mark.parametrize("centre", [True, False])
 @pytest.mark.parametrize("transform_generator", TRANSFORM_FAMILY_GENERATORS)
 def test_tpca(
-    tensor_shape, element_scale, include_negatives, n_components, transform_generator
+    tensor_shape,
+    element_scale,
+    include_negatives,
+    n_components,
+    transform_generator,
+    centre,
 ):
     """Make sure different inputs work, and perform basic sense checks"""
     RTOL = 1e-7
     ATOL = 1e-10
 
     rng = np.random.default_rng(seed=GLOBAL_SEED)
 
     n, p, t = tensor_shape
     k = min(n, p)
 
     M, Minv = transform_generator(t)
-    tpca = TPCA(n_components=n_components, M=M, Minv=Minv)
+    tpca = TPCA(n_components=n_components, M=M, Minv=Minv, centre=centre)
 
     # tensors of various sizes with uniformly distributed elements
     # within [0, element_scale) or [-0.5*element_scale, 0.5*element_scale)
     X = (
         rng.random(size=tensor_shape) * element_scale
         - include_negatives * 0.5 * element_scale
     )
```

### Comparing `tred-0.0.9/tred/__init__.py` & `tred-0.1.0/tred/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ._tensor_ops import facewise_product, m_product
 from ._tensor_pca import generate_default_m_transform_pair, tsvdm, TPCA
 from ._utils import display_tensor_facewise
 
 # private - for testing
 ##########################################################################################
 from ._tensor_ops import _mode_1_unfold, _mode_2_unfold, _mode_3_unfold
+from ._utils import _singular_vals_tensor_to_mat, _singular_vals_mat_to_tensor
 
 __all__ = [
     "generate_transform_pair_from_matrix",
     "generate_dctii_m_transform_pair",
     "generate_dstii_m_transform_pair",
     "facewise_product",
     "m_product",
```

### Comparing `tred-0.0.9/tred/_m_transforms.py` & `tred-0.1.0/tred/_m_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #   1. order 3 tensors: by applying the transform along the tubal fibres
 #   2. matrices: by applying the transform along the rows
 # i.e., along the -1 axis of order-2 and order-3 arrays
 #
 # we do not need extensive parameter validation however, as the M and Minv Callables
 # returned by the generator functions are meant to be passed into classes and functions
 # in the tred package - which do some of their own parameter validation
-SUPPORTED_TRANSFORM_ORDERS = (2, 3)
+SUPPORTED_TRANSFORM_ORDERS = (1, 2, 3)
 
 
 def _assert_t_and_order(X_input, t_expected):
     assert (
         len(X_input.shape) in SUPPORTED_TRANSFORM_ORDERS
     ), "Expecting matrix or order-3 tensor input"
     assert (
@@ -31,32 +31,35 @@
     """Generate a pair of functions to apply a matrix, and its inverse, to the tubal
     fibres of an order-3 tensor. See Kilmer et al. (20211).
 
     Parameters
     ----------
         M_mat : ArrayLike
             Square matrix
-        
+
         Minv_mat : ArrayLike or None, default=None
-            Square matrix, the inverse of M_mat. If not specified, this function will 
+            Square matrix, the inverse of M_mat. If not specified, this function will
             numerically evaluate the inverse of `M_mat`
 
         inplace : bool, default=False
-                Control whether or not the generated functions modify the input tensor
-                in-place, or return a copy with the m-transform applied
+            Control whether or not the generated functions modify the input tensor
+            in-place, or return a copy with the m-transform applied
+
+            THIS ARGUMENT DOES NOT CURRENTLY ALTER ANY BEHAVIOUR FOR THIS FUNCTION, BUT
+            IS A PLACEHOLDER FOR FUTURE DEVELOPMENT.
 
     Returns
     -------
         M : Callable[[ArrayLike], ndarray]
-                A function which expects an order-3 tensor as input, and applies `M_mat` 
-                to each of the tubal fibres. This preserves the dimensions of the tensor.
+            A function which expects an order-3 tensor as input, and applies `M_mat`
+            to each of the tubal fibres. This preserves the dimensions of the tensor.
 
         Minv : Callable[[ArrayLike], ndarray]
             A tensor transform (the inverse of `M`)
-    
+
     References
     ----------
     `Kilmer, M.E., Horesh, L., Avron, H. and Newman, E., 2021. Tensor-tensor
     algebra for optimal representation and compression of multiway data. Proceedings
     of the National Academy of Sciences, 118(28), p.e2015851118.`
     """
     assert len(M_mat.shape) == 2, "Expecting matrix (order-2 array) input"
@@ -71,33 +74,41 @@
         # https://stackoverflow.com/questions/17931613/how-to-decide-a-whether-a-matrix-is-singular-in-python-numpy
         if linalg.cond(M_mat) < 1 / sys.float_info.epsilon:
             Minv_mat = linalg.inv(M_mat)
         else:
             raise ValueError(
                 "Input matrix must be invertible, but appears singular, or close to singular"
             )
+    else:
+        assert (
+            Minv_mat.shape == M_mat.shape
+        ), "Ensure the shapes of matrix M and its inverse are the same"
 
     # a quick way of applying M along the tubal fibres of X, using np broadcasting:
     # transpose X into a n x t x p vertical stack of t x p matrices. matrix
     # multiplication is broadcast vertically, whereby M multiplies each of the t x p
     # matrices, effectively applying the transform to the columns, which were the original
     # tubal fibres. then transpose back to original
     def M(X):
         _assert_t_and_order(X, t_)
-        if len(X.shape) == 2:
-            return (M_mat @ X.T).T
-        else:  # len(X.shape == 3)
+        if len(X.shape) == 3:
             return (M_mat @ X.transpose(0, 2, 1)).transpose(0, 2, 1)
+        elif len(X.shape) == 2:
+            return (M_mat @ X.T).T
+        else:  # len(X.shape == 1)
+            return M_mat @ X
 
     def Minv(X):
         _assert_t_and_order(X, t_)
-        if len(X.shape) == 2:
-            return (Minv_mat @ X.T).T
-        else:  # len(X.shape == 3)
+        if len(X.shape) == 3:
             return (Minv_mat @ X.transpose(0, 2, 1)).transpose(0, 2, 1)
+        elif len(X.shape) == 2:
+            return (Minv_mat @ X.T).T
+        else:  # len(X.shape == 1)
+            return Minv_mat @ X
 
     return M, Minv
 
 
 def generate_dctii_m_transform_pair(t, *, inplace=False, norm="ortho"):
     """Wrapper around scipy fft to generate functions to perform $\times_3 M$ operations
     on order-3 tensors, where $M$ is the (scaled) Discrete Cosine Transform.
```

### Comparing `tred-0.0.9/tred/_tensor_ops.py` & `tred-0.1.0/tred/_tensor_ops.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,97 +3,105 @@
 
 import numpy as np
 
 from ._utils import _singular_vals_tensor_to_mat
 
 
 def facewise_product(A, B):
-    """Facewise product s.t. $C_{:,:,i} = A_{:,:,i} B_{:,:,i}$.
+    """Facewise product s.t. $(C_{:,:,i} = A_{:,:,i} B_{:,:,i}$.
 
     Parameters
     ----------
-        A : ArrayLike of shape (a, b, d)
-            $a \times b \times d$ tensor representation
+        A : ndarray, shape (a, b, d)
+            Tensor represented in order-3 ndarray
 
-        B : ArrayLike of shape (b, c, d)
-            $b \times c \times d$ tensor representation
+        B : ndarray, shape (b, c, d)
+            Tensor represented in order-3 ndarray
 
     Returns
     -------
         C : ndarray, shape: (a, c, d)
-            facewise tensor product
+            Facewise tensor product
     """
     # return np.einsum('mpi,pli->mli', A, B)
     # the following is a quicker version of the above using numpy broadcasting
     return (A.transpose(2, 0, 1) @ B.transpose(2, 0, 1)).transpose(1, 2, 0)
 
 
 def m_product(A, B, M, Minv):
-    """Kilmer et al. (2021) tensor m-product for order-3 tensors. See [1]
-
-    NOTE: NOT USED so far in this package. We tend to keep variables in the transformed
-    space, and therefore directly use the facewise_product function.
+    """Kilmer et al. (2021) tensor m-product for order-3 tensors.
 
     Parameters
     ----------
-        A : ArrayLike of shape (a, b, d)
-            $a \times b \times d$ tensor representation
+        A : ndarray, shape (a, b, d)
+            Tensor represented in order-3 ndarray
 
-        B : ArrayLike of shape (b, c, d)
-            $b \times c \times d$ tensor representation
+        B : ndarray, shape (b, c, d)
+            Tensor represented in order-3 ndarray
 
         M : Callable[[ArrayLike], ndarray]
-            A function which, given some order-3 tensor, returns it under some $\times_3$
-            invertible transformation.
+            A function which, given some order-3 tensor, returns it under an orthogonal
+            tubal transformation
 
         MInv : Callable[[ArrayLike], ndarray]
-            The inverse transformation of M
+            A function implementing the inverse tubal transformation of M
 
     Returns
     -------
         m_product : ndarray, shape: (a, c, d)
             Tensor-tensor m-product as found in Kilmer et al. (2021)
+
+    References
+    ----------
+    Kilmer, M.E., Horesh, L., Avron, H. and Newman, E., 2021. Tensor-tensor
+    algebra for optimal representation and compression of multiway data. Proceedings
+    of the National Academy of Sciences, 118(28), p.e2015851118.
     """
     assert (
         A.shape[1] == B.shape[0] and A.shape[2] == B.shape[2]
     ), "Non conforming dimensions"
 
     return Minv(facewise_product(M(A), M(B)))
 
 
 def _rank_q_truncation_zero_out(hatU, hatS, hatV, *, q=None, sigma_q=None):
-    """Explicit rank-q truncation as in Mor et al. (2022). Truncate, via zeroing out, the
-    input arrays passed in by reference.
-
-    This will typically be called in the m-transformed ('hat') space.
+    """In-place explicit rank-q truncation as introduced in Mor et al. (2022). Truncates
+    tensors U, S, V from a tsvdm decomposition to achieve an explicit rank of q.
 
     Parameters
     ----------
-        hatU : ArrayLike of shape (n, k, t)
-            tensor U returned by tSVDM
+        hatU : ndarray, shape (n, k, t)
+            Tensor U from the tsvdm.
+
+        hatS : ndarray, shape (k, k, t) or (k, t)
+            Tensor S from the tsvdm, or represented in compact matrix form.
+
+        hatV : ndarray, shape (p, k, t)
+            Tensor V from the tSVDM
 
-        hatS : ArrayLike of shape (k, k, t) or (k, t)
-            singular values tensor, or matrix representation, from tSVDM
+        q : int or None, default=None
+            Target explicit rank for the truncation
 
-        hatV : ArrayLike of shape (p, k, t)
-            tensor V returned by tSVDM
+        sigma_q : float or None, default=None
+            The `q`-th largest singular value. This will not be checked, and assumed to
+            be a valid singular value in the inputted decomposition.
 
-        q : int
-            Explicit rank ``q``, of the truncation
-
-        sigma_q : float
-            If ``sigma_q`` is set, then the ``q`` input parameter will be ignored. Saves
-            computation time by passing in the q-th largest singular value, which
-            may be cheap from the calling state if a sorted array of singular values has
-            already been computed.
+            If `sigma_q` is set, then the `q` input parameter will be ignored. Saves
+            re-computation of the `q`-th largest singular value.
 
     Returns
     -------
-        None
-            Modifies inputs in-place
+        rho : ndarray, shape (q,)
+            The multi-rank which results from the choice of `q` (or `sigma_q`)
+
+    References
+    ----------
+    Mor, U., Cohen, Y., Valdés-Mas, R., Kviatcovsky, D., Elinav, E. and Avron,
+    H., 2022. Dimensionality reduction of longitudinal’omics data using modern
+    tensor factorizations. PLoS Computational Biology, 18(7), p.e1010212.
     """
     assert not (q is None and sigma_q is None), "Please specify either q or sigma_q"
 
     # assume hatS in matrix form
     if len(hatS.shape) == 3:
         hatS = _singular_vals_tensor_to_mat(hatS)
 
@@ -126,21 +134,18 @@
 
     return rho
 
 
 def _mode_1_unfold(tens, view=False):
     """Return mode-1 unfolding copy, as defined in Kolda et al.
 
-    NOTE: NOT USED so far in this package. Probably redundant later if we adopt a more
-    intuitive tensor package in Python (TensorLy?).
-
     References
     ----------
-    `Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
-    review, 51(3), pp.455-500.`
+    Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
+    review, 51(3), pp.455-500.
     """
     # unfold the n x p x t tensor into a n x pt 2d array (matrix), where each frontal
     # slice sits 'next' each other.
     #
     # NUMPY NOTES:
     # first transpose into a n-vertical-stack of t x p matrices. reshape is equivalent
     # to 'ravel'-ling first, before reshaping the vector (using the same memory format)
@@ -157,36 +162,30 @@
     else:
         return tens.copy().transpose(0, 2, 1).reshape((tens.shape[0], -1), order="C")
 
 
 def _mode_2_unfold(tens, view=False):
     """Return mode-2 unfolding copy, as defined in Kolda et al.
 
-    NOTE: NOT USED so far in this package. Probably redundant later if we adopt a more
-    intuitive tensor package in Python (TensorLy?).
-
     References
     ----------
-    `Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
-    review, 51(3), pp.455-500.`
+    Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
+    review, 51(3), pp.455-500.
     """
     if view:
         return tens.view().transpose(1, 2, 0).reshape((tens.shape[1], -1), order="C")
     else:
         return tens.copy().transpose(1, 2, 0).reshape((tens.shape[1], -1), order="C")
 
 
 def _mode_3_unfold(tens, view=False):
     """Return mode-3 unfolding copy, as defined in Kolda et al.
 
-    NOTE: Probably redundant later if we adopt a more intuitive tensor package in Python
-    (TensorLy?).
-
     References
     ----------
-    `Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
-    review, 51(3), pp.455-500.`
+    Kolda, T.G. and Bader, B.W., 2009. Tensor decompositions and applications. SIAM
+    review, 51(3), pp.455-500.
     """
     if view:
         return tens.view().transpose(2, 1, 0).reshape((tens.shape[2], -1), order="C")
     else:
         return tens.copy().transpose(2, 1, 0).reshape((tens.shape[2], -1), order="C")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tred-0.0.9/tred/_tensor_pca.py` & `tred-0.1.0/tred/_tensor_pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,46 +122,56 @@
 
     if M is None:  # and Minv is None - guaranteed by assertion
         M, Minv = generate_default_m_transform_pair(A.shape[-1])
 
     # transform the tensor to new space via the mode-3 product
     hatA = M(A)
 
-    # an appropriate transposition allows Numpys array broadcasting to work appropriately
-    # S_mat contains the singular values per matrix in the input matrix 'stack'
-    # we reshape into a sparse tensor
-    # (the transpose tensor stacks top to bottom, with t horizontal slices of size n by p)
+    # an appropriate transposition allows Numpys array broadcasting to do facewise svd's
+    # S_mat contains the singular values per matrix in the input stack of matrices
+    # (the transpose tensor stacks top to bottom, with t slices of size n by p)
     U_stack, S_mat, Vt_stack = np.linalg.svd(
         hatA.transpose(2, 0, 1), full_matrices=full_frontal_slices
     )
 
     hatU = U_stack.transpose(1, 2, 0)
     S_mat = S_mat.transpose()
     # the following is a call to .transpose(1, 2, 0) followed by a facewise transpose
     # defined by .transpose(1, 0, 2)
     hatV = Vt_stack.transpose(2, 1, 0)
 
+    # if we are transforming scipy's singular values matrix back into tensor form, make
+    # sure we use the correct dimensions corresponding to whether or not the tensor
+    # faces were truncated during svd
+    if not svals_matrix_form:
+        if full_frontal_slices:
+            desired_S_tens_shape = A.shape
+        else:
+            n, p, t = A.shape
+            k = min(n, p)
+            desired_S_tens_shape = (k, k, t)
+
     if keep_hats:
         return (
             hatU,
             # by default return S as n,p,t f-diagonal tensor, matching literature
             # (or) convert into compressed matrix of singular values of shape (k,t)
             S_mat
             if svals_matrix_form
-            else _singular_vals_mat_to_tensor(S_mat, *A.shape),
+            else _singular_vals_mat_to_tensor(S_mat, *desired_S_tens_shape),
             hatV,
         )
     else:
         return (
             Minv(hatU),
             # by default return S as n,p,t f-diagonal tensor, matching literature
             # (or) convert into compressed matrix of singular values of shape (k,t)
             Minv(S_mat)
             if svals_matrix_form
-            else _singular_vals_mat_to_tensor(Minv(S_mat), *A.shape),
+            else _singular_vals_mat_to_tensor(Minv(S_mat), *desired_S_tens_shape),
             Minv(hatV),
         )
 
 
 class TPCA(ClassNamePrefixFeaturesOutMixin, TransformerMixin, BaseEstimator):
     """t-SVDM tensor analogue of PCA using explicit rank truncation with explicit rank
     truncation from Mor et al. (2022), and underlying m-product framework from Kilmer et
```

### Comparing `tred-0.0.9/tred/_utils.py` & `tred-0.1.0/tred/_utils.py`

 * *Files identical despite different names*

### Comparing `tred-0.0.9/.gitignore` & `tred-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tred-0.0.9/LICENSE` & `tred-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tred-0.0.9/README.txt` & `tred-0.1.0/README.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 as possible. 
 
 For the underlying tensor-product framework and tensor t-SVDM, see [1]. 
 For the explicit rank truncation, and the TCAM algorithm, see [2]. 
 
 Use
 ---
-[MORE USER-FRIENDLY EXAMPLES WILL BE UP SOON]
+See examples folder for basic use.
 
 tred is on PyPI, simply run
         pip install --upgrade tred
 To use the package. 
 
 tred is in active development. But, most of the existing implementations are 
 covered by unit tests, and we aim to keep the API relatively stable. 
@@ -54,18 +54,14 @@
             pytest . 
     In the root to run the tests in the test folder.
 
     If opening pull requests, invoke:
             black . 
     In the root to autoformat code. 
 
-    To build an updated version of the docs, invoke:
-            pdoc --html --output-dir docs tred
-    In the root to generate the docs in html under a `docs` directory. 
-
 Much of the implementation and code practice mirrors that of scikit-learn. We
 adopt their utilities and general coding guidelines whenever we can. 
 
 For any interested contributors, please be very liberal in adding tests, both 
 for new and existing features. 
 
 Credit
```

### Comparing `tred-0.0.9/pyproject.toml` & `tred-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tred"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Brendan Lu", email="brendannlu5@gmail.com" },
 ]
 description = "Dimensionality reduction techniques for order-3 tensors"
 readme = "README.txt"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tred-0.0.9/PKG-INFO` & `tred-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tred
-Version: 0.0.9
+Version: 0.1.0
 Summary: Dimensionality reduction techniques for order-3 tensors
 Project-URL: Homepage, https://github.com/brendanlu/tred
 Project-URL: Issues, https://github.com/brendanlu/tred/issues
 Author-email: Brendan Lu <brendannlu5@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 as possible. 
 
 For the underlying tensor-product framework and tensor t-SVDM, see [1]. 
 For the explicit rank truncation, and the TCAM algorithm, see [2]. 
 
 Use
 ---
-[MORE USER-FRIENDLY EXAMPLES WILL BE UP SOON]
+See examples folder for basic use.
 
 tred is on PyPI, simply run
         pip install --upgrade tred
 To use the package. 
 
 tred is in active development. But, most of the existing implementations are 
 covered by unit tests, and we aim to keep the API relatively stable. 
@@ -70,18 +70,14 @@
             pytest . 
     In the root to run the tests in the test folder.
 
     If opening pull requests, invoke:
             black . 
     In the root to autoformat code. 
 
-    To build an updated version of the docs, invoke:
-            pdoc --html --output-dir docs tred
-    In the root to generate the docs in html under a `docs` directory. 
-
 Much of the implementation and code practice mirrors that of scikit-learn. We
 adopt their utilities and general coding guidelines whenever we can. 
 
 For any interested contributors, please be very liberal in adding tests, both 
 for new and existing features. 
 
 Credit
```

