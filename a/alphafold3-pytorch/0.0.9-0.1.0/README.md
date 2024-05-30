# Comparing `tmp/alphafold3_pytorch-0.0.9.tar.gz` & `tmp/alphafold3_pytorch-0.1.0.tar.gz`

## Comparing `alphafold3_pytorch-0.0.9.tar` & `alphafold3_pytorch-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.env.sample
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.github/workflows/test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0    80825 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/tests/test_af3.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/LICENSE
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/README.md
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.env.sample
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/Dockerfile
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0   106090 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/life.py
+-rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/trainer.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/tests/test_af3.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/tests/test_trainer.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/README.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.0.9/alphafold3.png` & `alphafold3_pytorch-0.1.0/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/.github/workflows/publish.yml` & `alphafold3_pytorch-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.1.0/alphafold3_pytorch/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     ElucidatedAtomDiffusion,
     InputFeatureEmbedder,
     ConfidenceHead,
     DistogramHead,
     Alphafold3
 )
 
+from alphafold3_pytorch.trainer import (
+    Trainer,
+    Alphafold3Input
+)
+
 __all__ = [
     Attention,
     Attend,
     RelativePositionEncoding,
     SmoothLDDTLoss,
     WeightedRigidAlign,
     ExpressCoordinatesInFrame,
@@ -54,9 +59,11 @@
     PairformerStack,
     DiffusionTransformer,
     DiffusionModule,
     ElucidatedAtomDiffusion,
     InputFeatureEmbedder,
     ConfidenceHead,
     DistogramHead,
-    Alphafold3
+    Alphafold3,
+    Alphafold3Input,
+    Trainer
 ]
```

### Comparing `alphafold3_pytorch-0.0.9/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.1.0/alphafold3_pytorch/alphafold3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,98 @@
+from __future__ import annotations
+
 """
 global ein notation:
 
 b - batch
+ba - batch with augmentation
 h - heads
 n - residue sequence length
 i - residue sequence length (source)
 j - residue sequence length (target)
 m - atom sequence length
+nw - windowed sequence length
 d - feature dimension
 ds - feature dimension (single)
 dp - feature dimension (pairwise)
 dap - feature dimension (atompair)
+dapi - feature dimension (atompair input)
 da - feature dimension (atom)
+dai - feature dimension (atom input)
 t - templates
 s - msa
+r - registers
 """
 
-from __future__ import annotations
+"""
+additional_residue_feats: [*, 10]:
+
+0: residue_index
+1: token_index
+2: asym_id
+3: entity_id
+4: sym_id
+5: restype (must be one hot encoded to 32)
+6: is_protein
+7: is_rna
+8: is_dna
+9: is_ligand
+"""
 
 from math import pi, sqrt
-from functools import partial
+from pathlib import Path
+from functools import partial, wraps
 from collections import namedtuple
 
 import torch
 from torch import nn, sigmoid
 from torch import Tensor
 import torch.nn.functional as F
 
 from torch.nn import (
     Module,
     ModuleList,
     Linear,
     Sequential,
 )
 
-from typing import Literal, Tuple
+from typing import Literal, Tuple, NamedTuple
 
 from alphafold3_pytorch.typing import (
     Float,
     Int,
     Bool,
     typecheck
 )
 
-from alphafold3_pytorch.attention import Attention
+from alphafold3_pytorch.attention import (
+    Attention,
+    pad_at_dim,
+    slice_at_dim,
+    pad_or_slice_to,
+    pad_to_multiple,
+    concat_neighboring_windows,
+    full_attn_bias_to_windowed,
+    full_pairwise_repr_to_windowed
+)
+
+from taylor_series_linear_attention import TaylorSeriesLinearAttn
 
 import einx
 from einops import rearrange, repeat, reduce, einsum, pack, unpack
 from einops.layers.torch import Rearrange
 
 from tqdm import tqdm
 
+from importlib.metadata import version
+
 # constants
 
+ADDITIONAL_RESIDUE_FEATS = 10
+
 LinearNoBias = partial(Linear, bias = False)
 
 # helper functions
 
 def exists(v):
     return v is not None
 
@@ -74,43 +110,149 @@
 
 def pack_one(t, pattern):
     return pack([t], pattern)
 
 def unpack_one(t, ps, pattern):
     return unpack(t, ps, pattern)[0]
 
-# Loss functions
+def maybe(fn):
+    @wraps(fn)
+    def inner(t, *args, **kwargs):
+        if not exists(t):
+            return None
+        return fn(t, *args, **kwargs)
+    return inner
+
+def save_args_and_kwargs(fn):
+    @wraps(fn)
+    def inner(self, *args, **kwargs):
+        self._args_and_kwargs = (args, kwargs)
+        self._version = version('alphafold3_pytorch')
+
+        return fn(self, *args, **kwargs)
+    return inner
+
+# packed atom representation functions
 
 @typecheck
-def calc_smooth_lddt_loss(
-    denoised: Float['b m 3'], 
-    ground_truth: Float['b m 3'], 
-    is_rna_per_atom: Float['b m'],
-    is_dna_per_atom: Float['b m']
-) -> Float[' b']:
-    
-    m, device = is_rna_per_atom.shape[-1], denoised.device
-    
-    dx_denoised = torch.cdist(denoised, denoised)
-    dx_gt = torch.cdist(ground_truth, ground_truth)
-    
-    ddx = torch.abs(dx_gt - dx_denoised)
-    eps = 0.25 * (
-        sigmoid(0.5 - ddx) + sigmoid(1 - ddx) + sigmoid(2 - ddx) + sigmoid(4 - ddx)
+def lens_to_mask(
+    lens: Int['b ...'],
+    max_len: int | None = None
+) -> Bool['... m']:
+
+    device = lens.device
+    if not exists(max_len):
+        max_len = lens.amax()
+    arange = torch.arange(max_len, device = device)
+    return einx.less('m, ... -> ... m', arange, lens)
+
+@typecheck
+def mean_pool_with_lens(
+    feats: Float['b m d'],
+    lens: Int['b n']
+) -> Float['b n d']:
+
+    seq_len = feats.shape[1]
+
+    mask = lens > 0
+    assert (lens.sum(dim = -1) <= seq_len).all(), 'one of the lengths given exceeds the total sequence length of the features passed in'
+
+    cumsum_feats = feats.cumsum(dim = 1)
+    cumsum_feats = F.pad(cumsum_feats, (0, 0, 1, 0), value = 0.)
+
+    cumsum_indices = lens.cumsum(dim = 1)
+    cumsum_indices = F.pad(cumsum_indices, (1, 0), value = 0)
+
+    sel_cumsum = einx.get_at('b [m] d, b n -> b n d', cumsum_feats, cumsum_indices)
+
+    # subtract cumsum at one index from the previous one
+    summed = sel_cumsum[:, 1:] - sel_cumsum[:, :-1]
+
+    avg = einx.divide('b n d, b n', summed, lens.clamp(min = 1))
+    avg = einx.where('b n, b n d, -> b n d', mask, avg, 0.)
+    return avg
+
+@typecheck
+def repeat_consecutive_with_lens(
+    feats: Float['b n ...'] | Bool['b n'] | Int['b n'],
+    lens: Int['b n'],
+) -> Float['b m ...'] | Bool['b m'] | Int['b m']:
+
+    device, dtype = feats.device, feats.dtype
+
+    batch, seq, *dims = feats.shape
+
+    # get mask from lens
+
+    mask = lens_to_mask(lens)
+
+    # derive arange
+
+    window_size = mask.shape[-1]
+    arange = torch.arange(window_size, device = device)
+
+    cumsum_len = lens.cumsum(dim = -1)
+    offsets = F.pad(cumsum_len, (1, -1), value = 0)
+    indices = einx.add('w, b n -> b n w', arange, offsets)
+
+    # create output tensor + a sink position on the very right (index max_len)
+
+    total_lens = lens.sum(dim = -1)
+    output_mask = lens_to_mask(total_lens)
+
+    max_len = total_lens.amax()
+
+    output_indices = torch.zeros((batch, max_len + 1), device = device, dtype = torch.long)
+
+    indices.masked_fill_(~mask, max_len) # scatter to sink position for padding
+    indices = rearrange(indices, 'b n w -> b (n w)')
+
+    # scatter
+
+    seq_arange = torch.arange(seq, device = device)
+    seq_arange = repeat(seq_arange, 'n -> (n w)', w = window_size)
+
+    output_indices = einx.set_at('b [m],  b nw, nw -> b [m]', output_indices, indices, seq_arange)
+
+    # remove sink
+
+    output_indices = output_indices[:, :-1]
+
+    # gather
+
+    output = einx.get_at('b [n] ..., b m -> b m ...', feats, output_indices)
+
+    # final mask
+
+    mask_value = False if dtype == torch.bool else 0
+
+    output = einx.where(
+        'b n, b n ..., -> b n ...',
+        output_mask, output, mask_value
     )
-    
-    is_nuc = is_rna_per_atom + is_dna_per_atom
-    mask = einx.multiply('b i, b j -> b i j', is_nuc, is_nuc)
-    c = (dx_gt < 30) * mask + (dx_gt < 15) * (1 - mask)
-    
-    eye = torch.eye(m, device = device)
-    num = einx.sum('b [...]', c * eps * (1 - eye)) / (m**2 - m)
-    den = einx.sum('b [...]', c * (1 - eye)) / (m**2 - m)
 
-    return 1. - num/den
+    return output
+
+def repeat_pairwise_consecutive_with_lens(
+    feats: Float['b n n dp'],
+    lens: Int['b n']
+) -> Float['b m m dp']:
+
+    repeated_lens = repeat(lens, 'b ... -> (b repeat) ...', repeat = feats.shape[1])
+    feats, ps = pack_one(feats, '* n dp')
+    feats = repeat_consecutive_with_lens(feats, repeated_lens)
+    feats = unpack_one(feats, ps, '* n dp')
+
+    feats = rearrange(feats, 'b i j dp -> b j i dp')
+    repeated_lens = repeat(lens, 'b ... -> (b repeat) ...', repeat = feats.shape[1])
+    feats, ps = pack_one(feats, '* n dp')
+    feats = repeat_consecutive_with_lens(feats, repeated_lens)
+    feats = unpack_one(feats, ps, '* n dp')
+    feats = rearrange(feats, 'b j i dp -> b i j dp')
+    return feats
 
 # linear and outer sum
 # for single repr -> pairwise pattern throughout this architecture
 
 class LinearNoBiasThenOuterSum(Module):
     def __init__(
         self,
@@ -323,36 +465,32 @@
         dropout_type: Literal['row', 'col'] | None = None
     ):
         super().__init__()
 
         dim_hidden = default(dim_hidden, dim)
         self.norm = nn.LayerNorm(dim)
 
-        self.left_proj = Linear(dim, dim_hidden)
-        self.right_proj = Linear(dim, dim_hidden)
+        self.left_right_proj = nn.Sequential(
+            LinearNoBias(dim, dim_hidden * 4),
+            nn.GLU(dim = -1)
+        )
+
+        self.left_right_gate = LinearNoBias(dim, dim_hidden * 2)
 
-        self.left_gate = Linear(dim, dim_hidden)
-        self.right_gate = Linear(dim, dim_hidden)
-        self.out_gate = Linear(dim, dim_hidden)
-
-        # initialize all gating to be identity
-
-        for gate in (self.left_gate, self.right_gate, self.out_gate):
-            nn.init.constant_(gate.weight, 0.)
-            nn.init.constant_(gate.bias, 1.)
+        self.out_gate = LinearNoBias(dim, dim_hidden)
 
         if mix == 'outgoing':
             self.mix_einsum_eq = '... i k d, ... j k d -> ... i j d'
         elif mix == 'incoming':
             self.mix_einsum_eq = '... k j d, ... k i d -> ... i j d'
 
         self.to_out_norm = nn.LayerNorm(dim_hidden)
 
         self.to_out = Sequential(
-            Linear(dim_hidden, dim),
+            LinearNoBias(dim_hidden, dim),
             Dropout(dropout, dropout_type = dropout_type)
         )
 
     @typecheck
     def forward(
         self,
         x: Float['b n n d'],
@@ -360,32 +498,27 @@
     ) -> Float['b n n d']:
 
         if exists(mask):
             mask = einx.logical_and('b i, b j -> b i j 1', mask, mask)
 
         x = self.norm(x)
 
-        left = self.left_proj(x)
-        right = self.right_proj(x)
+        left, right = self.left_right_proj(x).chunk(2, dim = -1)
 
         if exists(mask):
             left = left * mask
             right = right * mask
 
-        left_gate = self.left_gate(x).sigmoid()
-        right_gate = self.right_gate(x).sigmoid()
-        out_gate = self.out_gate(x).sigmoid()
-
-        left = left * left_gate
-        right = right * right_gate
-
         out = einsum(left, right, self.mix_einsum_eq)
 
         out = self.to_out_norm(out)
+
+        out_gate = self.out_gate(x).sigmoid()
         out = out * out_gate
+
         return self.to_out(out)
 
 # there are two types of attention in this paper, triangle and attention-pair-bias
 # they differ by how the attention bias is computed
 # triangle is axial attention w/ itself projected for bias
 
 class AttentionPairBias(Module):
@@ -395,43 +528,68 @@
         heads,
         dim_pairwise,
         window_size = None,
         **attn_kwargs
     ):
         super().__init__()
 
+        self.window_size = window_size
+
         self.attn = Attention(
             heads = heads,
             window_size = window_size,
             **attn_kwargs
         )
 
         # line 8 of Algorithm 24
 
         to_attn_bias_linear = LinearNoBias(dim_pairwise, heads)
         nn.init.zeros_(to_attn_bias_linear.weight)
 
         self.to_attn_bias = nn.Sequential(
             nn.LayerNorm(dim_pairwise),
             to_attn_bias_linear,
-            Rearrange('... i j h -> ... h i j')
+            Rearrange('b ... h -> b h ...')
         )
 
     @typecheck
     def forward(
         self,
         single_repr: Float['b n ds'],
         *,
-        pairwise_repr: Float['b n n dp'],
-        attn_bias: Float['b n n'] | None = None,
+        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*3) dp'],
+        attn_bias: Float['b n n'] | Float['b nw w (w*3)'] | None = None,
         **kwargs
     ) -> Float['b n ds']:
 
+        w, has_window_size = self.window_size, exists(self.window_size)
+
+        # take care of windowing logic
+        # for sequence-local atom transformer
+
+        windowed_pairwise = pairwise_repr.ndim == 5
+
+        windowed_attn_bias = None
+
         if exists(attn_bias):
-            attn_bias = rearrange(attn_bias, 'b i j -> b 1 i j')
+            windowed_attn_bias = attn_bias.shape[-1] != attn_bias.shape[-2]
+
+        if has_window_size:
+            if not windowed_pairwise:
+                pairwise_repr = full_pairwise_repr_to_windowed(pairwise_repr, window_size = w)
+            if exists(attn_bias):
+                attn_bias = full_attn_bias_to_windowed(attn_bias, window_size = w)
+        else:
+            assert not windowed_pairwise, 'cannot pass in windowed pairwise repr if no window_size given to AttentionPairBias'
+            assert not exists(windowed_attn_bias) or not windowed_attn_bias, 'cannot pass in windowed attention bias if no window_size set for AttentionPairBias'
+
+        # attention bias preparation with further addition from pairwise repr
+
+        if exists(attn_bias):
+            attn_bias = rearrange(attn_bias, 'b ... -> b 1 ...')
         else:
             attn_bias = 0.
 
         attn_bias = self.to_attn_bias(pairwise_repr) + attn_bias
 
         out = self.attn(
             single_repr,
@@ -474,18 +632,18 @@
 
         if self.need_transpose:
             pairwise_repr = rearrange(pairwise_repr, 'b i j d -> b j i d')
 
         attn_bias = self.to_attn_bias(pairwise_repr)
 
         batch_repeat = pairwise_repr.shape[1]
-        attn_bias = repeat(attn_bias, 'b ... -> (b r) ...', r = batch_repeat)
+        attn_bias = repeat(attn_bias, 'b ... -> (b repeat) ...', repeat = batch_repeat)
 
         if exists(mask):
-            mask = repeat(mask, 'b ... -> (b r) ...', r = batch_repeat)
+            mask = repeat(mask, 'b ... -> (b repeat) ...', repeat = batch_repeat)
 
         pairwise_repr, packed_shape = pack_one(pairwise_repr, '* n d')
 
         out = self.attn(
             pairwise_repr,
             mask = mask,
             attn_bias = attn_bias,
@@ -585,21 +743,20 @@
         a, b = self.to_hidden(msa).chunk(2, dim = -1)
 
         outer_product = einsum(a, b, 'b s i d, b s j e -> b i j d e s')
 
         # maybe masked mean for outer product
 
         if exists(msa_mask):
-            msa_mask = rearrange(msa_mask, 'b s -> b 1 1 1 s')
-            outer_product = outer_product * msa_mask
+            outer_product = einx.multiply('b i j d e s, b s -> b i j d e s', outer_product, msa_mask.float())
 
             num = reduce(outer_product, '... s -> ...', 'sum')
             den = reduce(msa_mask.float(), '... s -> ...', 'sum')
 
-            outer_product_mean = num / den.clamp(min = self.eps)
+            outer_product_mean = einx.divide('b i j d e, b', num, den.clamp(min = self.eps))
         else:
             outer_product_mean = reduce(outer_product, '... s -> ...', 'mean')
 
         # flatten
 
         outer_product_mean = rearrange(outer_product_mean, '... d e -> ... (d e)')
 
@@ -692,18 +849,21 @@
         depth = 4,
         dim_msa = 64,
         dim_msa_input = None,
         outer_product_mean_dim_hidden = 32,
         msa_pwa_dropout_row_prob = 0.15,
         msa_pwa_heads = 8,
         msa_pwa_dim_head = 32,
-        pairwise_block_kwargs: dict = dict()
+        pairwise_block_kwargs: dict = dict(),
+        max_num_msa: int | None = None
     ):
         super().__init__()
 
+        self.max_num_msa = default(max_num_msa, float('inf'))  # cap the number of MSAs, will do sample without replacement if exceeds
+
         self.msa_init_proj = LinearNoBias(dim_msa_input, dim_msa) if exists(dim_msa_input) else nn.Identity()
 
         self.single_to_msa_feats = LinearNoBias(dim_single, dim_msa)
 
         layers = ModuleList([])
 
         for _ in range(depth):
@@ -748,14 +908,37 @@
         single_repr: Float['b n ds'],
         pairwise_repr: Float['b n n dp'],
         msa: Float['b s n dm'],
         mask: Bool['b n'] | None = None,
         msa_mask: Bool['b s'] | None = None,
     ) -> Float['b n n dp']:
 
+        batch, num_msa, device = *msa.shape[:2], msa.device
+
+        # sample without replacement
+
+        if num_msa > self.max_num_msa:
+            rand = torch.randn((batch, num_msa), device = device)
+
+            if exists(msa_mask):
+                rand.masked_fill_(~msa_mask, max_neg_value(msa))
+
+            indices = rand.topk(self.max_num_msa, dim = -1).indices
+
+            msa = einx.get_at('b [s] n dm, b sampled -> b sampled n dm', msa, indices)
+
+            if exists(msa_mask):
+                msa_mask = einx.get_at('b [s], b sampled -> b sampled', msa_mask, indices)
+
+        # account for no msa
+
+        if exists(msa_mask):
+            has_msa = reduce(msa_mask, 'b s -> b', 'any')
+
+        # process msa
 
         msa = self.msa_init_proj(msa)
 
         single_msa_feats = self.single_to_msa_feats(single_repr)
 
         msa = rearrange(single_msa_feats, 'b n d -> b 1 n d') + msa
 
@@ -773,14 +956,20 @@
             msa = msa_pair_weighted_avg(msa = msa, pairwise_repr = pairwise_repr, mask = mask) + msa
             msa = msa_transition(msa) + msa            
 
             # pairwise block
 
             pairwise_repr = pairwise_block(pairwise_repr = pairwise_repr, mask = mask)
 
+        if exists(msa_mask):
+            pairwise_repr = einx.where(
+                'b, b ..., -> b ...',
+                has_msa, pairwise_repr, 0.
+            )
+
         return pairwise_repr
 
 # pairformer stack
 
 class PairformerStack(Module):
     """ Algorithm 17 """
 
@@ -789,14 +978,15 @@
         *,
         dim_single = 384,
         dim_pairwise = 128,
         depth = 48,
         pair_bias_attn_dim_head = 64,
         pair_bias_attn_heads = 16,
         dropout_row_prob = 0.25,
+        num_register_tokens = 0,
         pairwise_block_kwargs: dict = dict()
     ):
         super().__init__()
         layers = ModuleList([])
 
         pair_bias_attn_kwargs = dict(
             dim = dim_single,
@@ -822,53 +1012,70 @@
                 pairwise_block,
                 single_pre_ln(pair_bias_attn),
                 single_pre_ln(single_transition),
             ]))
 
         self.layers = layers
 
+        self.num_registers = num_register_tokens
+        self.has_registers = num_register_tokens > 0
+
+        if self.has_registers:
+            self.single_registers = nn.Parameter(torch.zeros(num_register_tokens, dim_single))
+            self.pairwise_row_registers = nn.Parameter(torch.zeros(num_register_tokens, dim_pairwise))
+            self.pairwise_col_registers = nn.Parameter(torch.zeros(num_register_tokens, dim_pairwise))
+
     @typecheck
     def forward(
         self,
         *,
         single_repr: Float['b n ds'],
         pairwise_repr: Float['b n n dp'],
         mask: Bool['b n'] | None = None
 
     ) -> Tuple[Float['b n ds'], Float['b n n dp']]:
 
+        # prepend register tokens
+
+        if self.has_registers:
+            batch_size, num_registers = single_repr.shape[0], self.num_registers
+            single_registers = repeat(self.single_registers, 'r d -> b r d', b = batch_size)
+            single_repr = torch.cat((single_registers, single_repr), dim = 1)
+
+            row_registers = repeat(self.pairwise_row_registers, 'r d -> b r n d', b = batch_size, n = pairwise_repr.shape[-2])
+            pairwise_repr = torch.cat((row_registers, pairwise_repr), dim = 1)
+            col_registers = repeat(self.pairwise_col_registers, 'r d -> b n r d', b = batch_size, n = pairwise_repr.shape[1])
+            pairwise_repr = torch.cat((col_registers, pairwise_repr), dim = 2)
+
+            if exists(mask):
+                mask = F.pad(mask, (num_registers, 0), value = True)
+
+        # main transformer block layers
+
         for (
             pairwise_block,
             pair_bias_attn,
             single_transition
         ) in self.layers:
 
             pairwise_repr = pairwise_block(pairwise_repr = pairwise_repr, mask = mask)
 
             single_repr = pair_bias_attn(single_repr, pairwise_repr = pairwise_repr, mask = mask) + single_repr
             single_repr = single_transition(single_repr) + single_repr
 
+        # splice out registers
+
+        if self.has_registers:
+            single_repr = single_repr[:, num_registers:]
+            pairwise_repr = pairwise_repr[:, num_registers:, num_registers:]
+
         return single_repr, pairwise_repr
 
 # embedding related
 
-"""
-additional_residue_feats: [*, rf]:
-    0: residue_index
-    1: token_index
-    2: asym_id
-    3: entity_id
-    4: sym_id 
-    5: restype (must be one hot encoded to 32)
-    6: is_protein
-    7: is_rna
-    8: is_dna
-    9: is_ligand
-"""
-
 class RelativePositionEncoding(Module):
     """ Algorithm 3 """
     
     def __init__(
         self,
         *,
         r_max = 32,
@@ -882,15 +1089,15 @@
         dim_input = (2*r_max+2) + (2*r_max+2) + 1 + (2*s_max+2)
         self.out_embedder = LinearNoBias(dim_input, dim_out)
 
     @typecheck
     def forward(
         self,
         *,
-        additional_residue_feats: Float['b n rf']
+        additional_residue_feats: Float[f'b n {ADDITIONAL_RESIDUE_FEATS}']
     ) -> Float['b n n dp']:
 
         device = additional_residue_feats.device
         assert additional_residue_feats.shape[-1] >= 5
 
         res_idx, token_idx, asym_id, entity_id, sym_id = additional_residue_feats[..., :5].unbind(dim = -1)
         
@@ -917,20 +1124,18 @@
         d_chain = torch.where(
             ~mask_same_chain, 
             torch.clip(diff_sym_id + self.s_max, 0, 2*self.s_max),
             2*self.s_max + 1
         )
         
         def onehot(x, bins):
-            x, packed_shape = pack_one(x, '*')
-            dist_from_bins = einx.subtract('i, j -> i j', x, bins)
-            indexes = dist_from_bins.abs().min(dim = 1, keepdim = True).indices
-            indexes = rearrange(indexes.long(), 'i j -> (i j) 1')
-            one_hots = torch.zeros(indexes.shape[0], len(bins)).scatter_(1, indexes, 1)
-            return unpack_one(one_hots, packed_shape, '* d')
+            dist_from_bins = einx.subtract('... i, j -> ... i j', x, bins)
+            indices = dist_from_bins.abs().min(dim = -1, keepdim = True).indices
+            one_hots = F.one_hot(indices.long(), num_classes = len(bins))
+            return one_hots.float()
 
         r_arange = torch.arange(2*self.r_max + 2, device = device)
         s_arange = torch.arange(2*self.s_max + 2, device = device)
 
         a_rel_pos = onehot(d_res, r_arange)
         a_rel_token = onehot(d_token, r_arange)
         a_rel_chain = onehot(d_chain, s_arange)
@@ -1002,14 +1207,16 @@
         pairwise_repr = self.pairwise_to_embed_input(pairwise_repr)
         pairwise_repr = rearrange(pairwise_repr, 'b i j d -> b 1 i j d')
 
         v = self.template_feats_to_embed_input(templates) + pairwise_repr
 
         v, merged_batch_ps = pack_one(v, '* i j d')
 
+        has_templates = reduce(template_mask, 'b t -> b', 'any')
+
         if exists(mask):
             mask = repeat(mask, 'b n -> (b t) n', t = num_templates)
 
         for block in self.pairformer_stack:
             v = block(
                 pairwise_repr = v,
                 mask = mask
@@ -1017,25 +1224,32 @@
 
         u = self.final_norm(v)
 
         u = unpack_one(u, merged_batch_ps, '* i jk d')
 
         # masked mean pool template repr
 
-        u = u.masked_fill(
-            ~rearrange(template_mask, 'b t -> b t 1 1 1'),
-            0.
+        u = einx.where(
+            'b t, b t ..., -> b t ...',
+            template_mask, u, 0.
         )
 
         num = reduce(u, 'b t i j d -> b i j d', 'sum')
-        den = reduce(template_mask.float(), 'b t -> b 1 1 1', 'sum')
+        den = reduce(template_mask.float(), 'b t -> b', 'sum')
+
+        avg_template_repr = einx.divide('b i j d, b -> b i j d', num, den.clamp(min = self.eps))
 
-        avg_template_repr = num / den.clamp(min = self.eps)
+        out = self.to_out(avg_template_repr)
 
-        return self.to_out(avg_template_repr)
+        out = einx.where(
+            'b, b ..., -> b ...',
+            has_templates, out, 0.
+        )
+
+        return out
 
 # diffusion related
 # both diffusion transformer as well as atom encoder / decoder
 
 class FourierEmbedding(Module):
     """ Algorithm 22 """
 
@@ -1166,23 +1380,41 @@
         depth,
         heads,
         dim = 384,
         dim_single_cond = None,
         dim_pairwise = 128,
         attn_window_size = None,
         attn_pair_bias_kwargs: dict = dict(),
-        serial = False
+        num_register_tokens = 0,
+        serial = False,
+        use_linear_attn = False,
+        linear_attn_kwargs = dict(
+            heads = 8,
+            dim_head = 16
+        )
     ):
         super().__init__()
+        self.attn_window_size = attn_window_size
+
         dim_single_cond = default(dim_single_cond, dim)
 
         layers = ModuleList([])
 
         for _ in range(depth):
 
+            linear_attn = None
+
+            if use_linear_attn:
+                linear_attn = TaylorSeriesLinearAttn(
+                    dim = dim,
+                    prenorm = True,
+                    gate_value_heads = True,
+                    **linear_attn_kwargs
+                )
+
             pair_bias_attn = AttentionPairBias(
                 dim = dim,
                 dim_pairwise = dim_pairwise,
                 heads = heads,
                 window_size = attn_window_size,
                 **attn_pair_bias_kwargs
             )
@@ -1200,34 +1432,71 @@
             conditionable_transition = ConditionWrapper(
                 transition,
                 dim = dim,
                 dim_cond = dim_single_cond
             )
 
             layers.append(ModuleList([
+                linear_attn,
                 conditionable_pair_bias,
                 conditionable_transition
             ]))
 
         self.layers = layers
 
         self.serial = serial
 
+        self.has_registers = num_register_tokens > 0
+        self.num_registers = num_register_tokens
+
+        if self.has_registers:
+            assert not exists(attn_window_size), 'register tokens disabled for windowed attention'
+
+            self.registers = nn.Parameter(torch.zeros(num_register_tokens, dim))
+
     @typecheck
     def forward(
         self,
         noised_repr: Float['b n d'],
         *,
         single_repr: Float['b n ds'],
-        pairwise_repr: Float['b n n dp'],
+        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*3) dp'],
         mask: Bool['b n'] | None = None
     ):
+        w = self.attn_window_size
+        has_windows = exists(w)
+
         serial = self.serial
 
-        for attn, transition in self.layers:
+        # handle windowing
+
+        pairwise_is_windowed = pairwise_repr.ndim == 5
+
+        if has_windows and not pairwise_is_windowed:
+            pairwise_repr = full_pairwise_repr_to_windowed(pairwise_repr, window_size = w)
+
+        # register tokens
+
+        if self.has_registers:
+            num_registers = self.num_registers
+            registers = repeat(self.registers, 'r d -> b r d', b = noised_repr.shape[0])
+            noised_repr, registers_ps = pack((registers, noised_repr), 'b * d')
+
+            single_repr = F.pad(single_repr, (0, 0, num_registers, 0), value = 0.)
+            pairwise_repr = F.pad(pairwise_repr, (0, 0, num_registers, 0, num_registers, 0), value = 0.)
+
+            if exists(mask):
+                mask = F.pad(mask, (num_registers, 0), value = True)
+
+        # main transformer
+
+        for linear_attn, attn, transition in self.layers:
+
+            if exists(linear_attn):
+                noised_repr = linear_attn(noised_repr, mask = mask) + noised_repr
 
             attn_out = attn(
                 noised_repr,
                 cond = single_repr,
                 pairwise_repr = pairwise_repr,
                 mask = mask
             )
@@ -1241,58 +1510,46 @@
             )
 
             if not serial:
                 ff_out = ff_out + attn_out
 
             noised_repr = noised_repr + ff_out
 
+        # splice out registers
+
+        if self.has_registers:
+            _, noised_repr = unpack(noised_repr, registers_ps, 'b * d')
+
         return noised_repr
 
 class AtomToTokenPooler(Module):
     def __init__(
         self,
         dim,
-        dim_out = None,
-        atoms_per_window = 27
+        dim_out = None
     ):
         super().__init__()
         dim_out = default(dim_out, dim)
 
         self.proj = nn.Sequential(
             LinearNoBias(dim, dim_out),
             nn.ReLU()
         )
 
-        self.atoms_per_window = atoms_per_window
-
     @typecheck
     def forward(
         self,
         *,
         atom_feats: Float['b m da'],
-        atom_mask: Bool['b m']
+        atom_mask: Bool['b m'],
+        residue_atom_lens: Int['b n']
     ) -> Float['b n ds']:
-        w = self.atoms_per_window
 
         atom_feats = self.proj(atom_feats)
-
-        # masked mean pool the atom feats for each residue, for the token transformer
-        # this is basically a simple 2-level hierarchical transformer
-
-        windowed_atom_feats = rearrange(atom_feats, 'b (n w) da -> b n w da', w = w)
-        windowed_atom_mask = rearrange(atom_mask, 'b (n w) -> b n w', w = w)
-
-        assert windowed_atom_mask.any(dim = -1).all(), 'atom mask must contain one valid atom for each window'
-
-        windowed_atom_feats = windowed_atom_feats.masked_fill(windowed_atom_mask[..., None], 0.)
-
-        num = reduce(windowed_atom_feats, 'b n w d -> b n d', 'sum')
-        den = reduce(windowed_atom_mask.float(), 'b n w -> b n 1', 'sum')
-
-        tokens = num / den
+        tokens = mean_pool_with_lens(atom_feats, residue_atom_lens)
         return tokens
 
 class DiffusionModule(Module):
     """ Algorithm 20 """
 
     @typecheck
     def __init__(
@@ -1317,15 +1574,23 @@
         ),
         atom_encoder_depth = 3,
         atom_encoder_heads = 4,
         token_transformer_depth = 24,
         token_transformer_heads = 16,
         atom_decoder_depth = 3,
         atom_decoder_heads = 4,
-        serial = False
+        serial = False,
+        atom_encoder_kwargs: dict = dict(),
+        atom_decoder_kwargs: dict = dict(),
+        token_transformer_kwargs: dict = dict(),
+        use_linear_attn = False,
+        linear_attn_kwargs: dict = dict(
+            heads = 8,
+            dim_head = 16
+        )
     ):
         super().__init__()
 
         self.atoms_per_window = atoms_per_window
 
         # conditioning
 
@@ -1354,15 +1619,15 @@
         self.pairwise_repr_to_atompair_feat_cond = nn.Sequential(
             nn.LayerNorm(dim_pairwise),
             LinearNoBias(dim_pairwise, dim_atompair)
         )
 
         self.atom_repr_to_atompair_feat_cond = nn.Sequential(
             nn.LayerNorm(dim_atom),
-            LinearNoBiasThenOuterSum(dim_atom, dim_atompair),
+            LinearNoBias(dim_atom, dim_atompair * 2),
             nn.ReLU()
         )
 
         self.atompair_feats_mlp = nn.Sequential(
             LinearNoBias(dim_atompair, dim_atompair),
             nn.ReLU(),
             LinearNoBias(dim_atompair, dim_atompair),
@@ -1373,21 +1638,23 @@
         self.atom_encoder = DiffusionTransformer(
             dim = dim_atom,
             dim_single_cond = dim_atom,
             dim_pairwise = dim_atompair,
             attn_window_size = atoms_per_window,
             depth = atom_encoder_depth,
             heads = atom_encoder_heads,
-            serial = serial
+            serial = serial,
+            use_linear_attn = use_linear_attn,
+            linear_attn_kwargs = linear_attn_kwargs,
+            **atom_encoder_kwargs
         )
 
         self.atom_feats_to_pooled_token = AtomToTokenPooler(
             dim = dim_atom,
-            dim_out = dim_token,
-            atoms_per_window = atoms_per_window
+            dim_out = dim_token
         )
 
         # token attention related modules
 
         self.cond_tokens_with_cond_single = nn.Sequential(
             nn.LayerNorm(dim_single),
             LinearNoBias(dim_single, dim_token)
@@ -1395,15 +1662,16 @@
 
         self.token_transformer = DiffusionTransformer(
             dim = dim_token,
             dim_single_cond = dim_single,
             dim_pairwise = dim_pairwise,
             depth = token_transformer_depth,
             heads = token_transformer_heads,
-            serial = serial
+            serial = serial,
+            **token_transformer_kwargs
         )
 
         self.attended_token_norm = nn.LayerNorm(dim_token)
 
         # atom attention decoding related modules
 
         self.tokens_to_atom_decoder_input_cond = LinearNoBias(dim_token, dim_atom)
@@ -1411,43 +1679,46 @@
         self.atom_decoder = DiffusionTransformer(
             dim = dim_atom,
             dim_single_cond = dim_atom,
             dim_pairwise = dim_atompair,
             attn_window_size = atoms_per_window,
             depth = atom_decoder_depth,
             heads = atom_decoder_heads,
-            serial = serial
+            serial = serial,
+            use_linear_attn = use_linear_attn,
+            linear_attn_kwargs = linear_attn_kwargs,
+            **atom_decoder_kwargs
         )
 
         self.atom_feat_to_atom_pos_update = nn.Sequential(
             nn.LayerNorm(dim_atom),
             LinearNoBias(dim_atom, 3)
         )
 
     @typecheck
     def forward(
         self,
         noised_atom_pos: Float['b m 3'],
         *,
         atom_feats: Float['b m da'],
-        atompair_feats: Float['b m m dap'],
+        atompair_feats: Float['b m m dap'] | Float['b nw w (w*3) dap'],
         atom_mask: Bool['b m'],
         times: Float[' b'],
         mask: Bool['b n'],
         single_trunk_repr: Float['b n dst'],
         single_inputs_repr: Float['b n dsi'],
         pairwise_trunk: Float['b n n dpt'],
         pairwise_rel_pos_feats: Float['b n n dpr'],
+        residue_atom_lens: Int['b n']
     ):
         w = self.atoms_per_window
+        device = noised_atom_pos.device
 
-        # in the paper, it seems they pack the atom feats
-        # but in this impl, will just use windows for simplicity when communicating between atom and residue resolutions. bit less efficient
-
-        assert divisible_by(noised_atom_pos.shape[-2], w)
+        batch_size, seq_len = single_trunk_repr.shape[:2]
+        atom_seq_len = atom_feats.shape[1]
 
         conditioned_single_repr = self.single_conditioner(
             times = times,
             single_trunk_repr = single_trunk_repr,
             single_inputs_repr = single_inputs_repr
         )
 
@@ -1464,27 +1735,60 @@
 
         atom_feats = self.atom_pos_to_atom_feat(noised_atom_pos) + atom_feats
 
         # condition atom feats cond (cl) with single repr
 
         single_repr_cond = self.single_repr_to_atom_feat_cond(conditioned_single_repr)
 
-        single_repr_cond = repeat(single_repr_cond, 'b n ds -> b (n w) ds', w = w)
+        single_repr_cond = repeat_consecutive_with_lens(single_repr_cond, residue_atom_lens)
+        single_repr_cond = pad_or_slice_to(single_repr_cond, length = atom_feats_cond.shape[1], dim = 1)
+
         atom_feats_cond = single_repr_cond + atom_feats_cond
 
+        # window the atom pair features before passing to atom encoder and decoder if necessary
+
+        atompair_is_windowed = atompair_feats.ndim == 5
+
+        if not atompair_is_windowed:
+            atompair_feats = full_pairwise_repr_to_windowed(atompair_feats, window_size = self.atoms_per_window)
+
         # condition atompair feats with pairwise repr
 
         pairwise_repr_cond = self.pairwise_repr_to_atompair_feat_cond(conditioned_pairwise_repr)
-        pairwise_repr_cond = repeat(pairwise_repr_cond, 'b i j dp -> b (i w1) (j w2) dp', w1 = w, w2 = w)
+
+        indices = torch.arange(seq_len, device = device)
+        indices = repeat(indices, 'n -> b n', b = batch_size)
+
+        indices = repeat_consecutive_with_lens(indices, residue_atom_lens)
+        indices = pad_or_slice_to(indices, atom_seq_len, dim = -1)
+        indices = pad_to_multiple(indices, w, dim = -1)
+
+        row_indices = col_indices = indices
+        row_indices = rearrange(row_indices, 'b (n w) -> b n w 1', w = w)
+        col_indices = rearrange(col_indices, 'b (n w) -> b n 1 w', w = w)
+
+        col_indices = concat_neighboring_windows(col_indices, dim_seq = 1, dim_window = -1)
+        row_indices, col_indices = torch.broadcast_tensors(row_indices, col_indices)
+
+        pairwise_repr_cond = einx.get_at('b [i j] dap, b nw w1 w2, b nw w1 w2 -> b nw w1 w2 dap', pairwise_repr_cond, row_indices, col_indices)
+
         atompair_feats = pairwise_repr_cond + atompair_feats
 
         # condition atompair feats further with single atom repr
 
         atom_repr_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
-        atompair_feats = atom_repr_cond + atompair_feats
+        atom_repr_cond = pad_to_multiple(atom_repr_cond, w, dim = 1)
+        atom_repr_cond = rearrange(atom_repr_cond, 'b (n w) dap -> b n w dap', w = w)
+
+        atom_repr_cond_row, atom_repr_cond_col = atom_repr_cond.chunk(2, dim = -1)
+
+        atom_repr_cond_col = concat_neighboring_windows(atom_repr_cond_col, dim_seq = 1, dim_window = 2)
+
+        atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_row)
+        atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_col)
 
         # furthermore, they did one more MLP on the atompair feats for attention biasing in atom transformer
 
         atompair_feats = self.atompair_feats_mlp(atompair_feats) + atompair_feats
 
         # atom encoder
 
@@ -1495,16 +1799,18 @@
             pairwise_repr = atompair_feats
         )
 
         atom_feats_skip = atom_feats
 
         tokens = self.atom_feats_to_pooled_token(
             atom_feats = atom_feats,
-            atom_mask = atom_mask
+            atom_mask = atom_mask,
+            residue_atom_lens = residue_atom_lens
         )
+
         # token transformer
 
         tokens = self.cond_tokens_with_cond_single(conditioned_single_repr) + tokens
 
         self.token_transformer(
             tokens,
             mask = mask,
@@ -1513,15 +1819,17 @@
         )
 
         tokens = self.attended_token_norm(tokens)
 
         # atom decoder
 
         atom_decoder_input = self.tokens_to_atom_decoder_input_cond(tokens)
-        atom_decoder_input = repeat(atom_decoder_input, 'b n da -> b (n w) da', w = w)
+
+        atom_decoder_input = repeat_consecutive_with_lens(atom_decoder_input, residue_atom_lens)
+        atom_decoder_input = pad_or_slice_to(atom_decoder_input, length = atom_feats_skip.shape[1], dim = 1)
 
         atom_decoder_input = atom_decoder_input + atom_feats_skip
 
         atom_feats = self.atom_decoder(
             atom_decoder_input,
             mask = atom_mask,
             single_repr = atom_feats_cond,
@@ -1532,14 +1840,25 @@
 
         return atom_pos_update
 
 # elucidated diffusion model adapted for atom position diffusing
 # from Karras et al.
 # https://arxiv.org/abs/2206.00364
 
+class DiffusionLossBreakdown(NamedTuple):
+    diffusion_mse: Float['']
+    diffusion_bond: Float['']
+    diffusion_smooth_lddt: Float['']
+
+class ElucidatedAtomDiffusionReturn(NamedTuple):
+    loss: Float['']
+    denoised_atom_pos: Float['ba m 3']
+    loss_breakdown: DiffusionLossBreakdown
+    noise_sigmas: Float[' ba']
+
 class ElucidatedAtomDiffusion(Module):
     @typecheck
     def __init__(
         self,
         net: DiffusionModule,
         *,
         num_sample_steps = 32, # number of sampling steps
@@ -1549,14 +1868,16 @@
         rho = 7,               # controls the sampling schedule
         P_mean = -1.2,         # mean of log-normal distribution from which noise is drawn for training
         P_std = 1.2,           # standard deviation of log-normal distribution from which noise is drawn for training
         S_churn = 80,          # parameters for stochastic sampling - depends on dataset, Table 5 in apper
         S_tmin = 0.05,
         S_tmax = 50,
         S_noise = 1.003,
+        smooth_lddt_loss_kwargs: dict = dict(),
+        weighted_rigid_align_kwargs: dict = dict()
     ):
         super().__init__()
         self.net = net
 
         # parameters
 
         self.sigma_min = sigma_min
@@ -1571,14 +1892,24 @@
         self.num_sample_steps = num_sample_steps  # otherwise known as N in the paper
 
         self.S_churn = S_churn
         self.S_tmin = S_tmin
         self.S_tmax = S_tmax
         self.S_noise = S_noise
 
+        # weighted rigid align
+
+        self.weighted_rigid_align = WeightedRigidAlign(**weighted_rigid_align_kwargs)
+
+        # smooth lddt loss
+
+        self.smooth_lddt_loss = SmoothLDDTLoss(**smooth_lddt_loss_kwargs)
+
+        self.register_buffer('zero', torch.tensor(0.), persistent = False)
+
     @property
     def device(self):
         return next(self.net.parameters()).device
 
     # derived preconditioning params - Table 1
 
     def c_skip(self, sigma):
@@ -1640,17 +1971,17 @@
 
         sigmas = F.pad(sigmas, (0, 1), value = 0.) # last step is sigma value of 0.
         return sigmas
 
     @torch.no_grad()
     def sample(
         self,
-        atom_mask: Bool['b m'],
+        atom_mask: Bool['b m'] | None = None,
         num_sample_steps = None,
-        clamp = True,
+        clamp = False,
         **network_condition_kwargs
     ):
         num_sample_steps = default(num_sample_steps, self.num_sample_steps)
 
         shape = (*atom_mask.shape, 3)
 
         network_condition_kwargs.update(atom_mask = atom_mask)
@@ -1693,126 +2024,194 @@
             if sigma_next != 0:
                 model_output_next = self.preconditioned_network_forward(atom_pos_next, sigma_next, clamp = clamp, network_condition_kwargs = network_condition_kwargs)
                 denoised_prime_over_sigma = (atom_pos_next - model_output_next) / sigma_next
                 atom_pos_next = atom_pos_hat + 0.5 * (sigma_next - sigma_hat) * (denoised_over_sigma + denoised_prime_over_sigma)
 
             atom_pos = atom_pos_next
 
-        atom_pos = atom_pos.clamp(-1., 1.)
+        if clamp:
+            atom_pos = atom_pos.clamp(-1., 1.)
+
         return atom_pos
 
     # training
 
     def loss_weight(self, sigma):
         return (sigma ** 2 + self.sigma_data ** 2) * (sigma * self.sigma_data) ** -2
 
     def noise_distribution(self, batch_size):
         return (self.P_mean + self.P_std * torch.randn((batch_size,), device = self.device)).exp()
 
     def forward(
         self,
-        normalized_atom_pos: Float['b m 3'],
+        atom_pos_ground_truth: Float['b m 3'],
         atom_mask: Bool['b m'],
+        atom_feats: Float['b m da'],
+        atompair_feats: Float['b m m dap'],
+        mask: Bool['b n'],
+        single_trunk_repr: Float['b n dst'],
+        single_inputs_repr: Float['b n dsi'],
+        pairwise_trunk: Float['b n n dpt'],
+        pairwise_rel_pos_feats: Float['b n n dpr'],
+        residue_atom_lens: Int['b n'],
         return_denoised_pos = False,
-        additional_residue_feats: Float['b n rf'] | None = None,
+        additional_residue_feats: Float[f'b n {ADDITIONAL_RESIDUE_FEATS}'] | None = None,
         add_smooth_lddt_loss = False,
         add_bond_loss = False,
-        **network_condition_kwargs
-    ) -> Float[''] | Tuple[Float[''], Float['b m 3']]:
+        nucleotide_loss_weight = 5.,
+        ligand_loss_weight = 10.,
+        return_loss_breakdown = False,
+    ) -> ElucidatedAtomDiffusionReturn:
+
+        # diffusion loss
 
-        batch_size = normalized_atom_pos.shape[0]
+        batch_size = atom_pos_ground_truth.shape[0]
 
         sigmas = self.noise_distribution(batch_size)
         padded_sigmas = rearrange(sigmas, 'b -> b 1 1')
 
-        noise = torch.randn_like(normalized_atom_pos)
+        noise = torch.randn_like(atom_pos_ground_truth)
 
-        noised_atom_pos = normalized_atom_pos + padded_sigmas * noise  # alphas are 1. in the paper
-
-        network_condition_kwargs.update(atom_mask = atom_mask)
+        noised_atom_pos = atom_pos_ground_truth + padded_sigmas * noise  # alphas are 1. in the paper
 
         denoised_atom_pos = self.preconditioned_network_forward(
             noised_atom_pos,
             sigmas,
-            network_condition_kwargs = network_condition_kwargs
+            network_condition_kwargs = dict(
+                atom_feats = atom_feats,
+                atom_mask = atom_mask,
+                atompair_feats = atompair_feats,
+                mask = mask,
+                single_trunk_repr = single_trunk_repr,
+                single_inputs_repr = single_inputs_repr,
+                pairwise_trunk = pairwise_trunk,
+                pairwise_rel_pos_feats = pairwise_rel_pos_feats,
+                residue_atom_lens = residue_atom_lens
+            )
+        )
+
+        total_loss = 0.
+
+        # if additional residue feats is provided
+        # calculate the weights for mse loss (wl)
+
+        align_weights = atom_pos_ground_truth.new_ones(atom_pos_ground_truth.shape[:2])
+
+        if exists(additional_residue_feats):
+            w = self.net.atoms_per_window
+
+            is_nucleotide_or_ligand_fields = (additional_residue_feats[..., 7:] != 0.).unbind(dim = -1)
+
+            is_nucleotide_or_ligand_fields = tuple(repeat_consecutive_with_lens(t, residue_atom_lens) for t in is_nucleotide_or_ligand_fields)
+            is_nucleotide_or_ligand_fields = tuple(pad_or_slice_to(t, length = align_weights.shape[-1], dim = -1) for t in is_nucleotide_or_ligand_fields)
+
+            atom_is_dna, atom_is_rna, atom_is_ligand = is_nucleotide_or_ligand_fields
+
+            # section 3.7.1 equation 4
+
+            # upweighting of nucleotide and ligand atoms is additive per equation 4
+
+            align_weights = torch.where(atom_is_dna | atom_is_rna, 1 + nucleotide_loss_weight, align_weights)
+            align_weights = torch.where(atom_is_ligand, 1 + ligand_loss_weight, align_weights)
+
+        # section 3.7.1 equation 2 - weighted rigid aligned ground truth
+
+        atom_pos_aligned_ground_truth = self.weighted_rigid_align(
+            atom_pos_ground_truth,
+            denoised_atom_pos,
+            align_weights,
+            mask = atom_mask
         )
 
         # main diffusion mse loss
 
-        losses = F.mse_loss(denoised_atom_pos, normalized_atom_pos, reduction = 'none')
+        losses = F.mse_loss(denoised_atom_pos, atom_pos_aligned_ground_truth, reduction = 'none') / 3.
+        losses = einx.multiply('b m c, b m -> b m c',  losses, align_weights)
+
+        # regular loss weight as defined in EDM paper
 
         loss_weights = self.loss_weight(padded_sigmas)
 
         losses = losses * loss_weights
 
-        loss = losses[atom_mask].mean()
+        # account for atom mask
+
+        mse_loss = losses[atom_mask].mean()
+
+        total_loss = total_loss + mse_loss
 
         # proposed extra bond loss during finetuning
 
+        bond_loss = self.zero
+
         if add_bond_loss:
             atompair_mask = einx.logical_and('b i, b j -> b i j', atom_mask, atom_mask)
 
             denoised_cdist = torch.cdist(denoised_atom_pos, denoised_atom_pos, p = 2)
-            normalized_cdist = torch.cdist(normalized_atom_pos, normalized_atom_pos, p = 2)
+            normalized_cdist = torch.cdist(atom_pos_ground_truth, atom_pos_ground_truth, p = 2)
 
             bond_losses = F.mse_loss(denoised_cdist, normalized_cdist, reduction = 'none')
             bond_losses = bond_losses * loss_weights
 
             bond_loss = bond_losses[atompair_mask].mean()
 
-            loss = loss + bond_loss
+            total_loss = total_loss + bond_loss
 
         # proposed auxiliary smooth lddt loss
 
+        smooth_lddt_loss = self.zero
+
         if add_smooth_lddt_loss:
             assert exists(additional_residue_feats)
-            w = self.net.atoms_per_window
-
-            is_dna, is_rna = additional_residue_feats[..., 7], additional_residue_feats[..., 8]
-            atom_is_dna, atom_is_rna = tuple(repeat(t, 'b n -> b (n w)', w = w) for t in (is_dna, is_rna))
 
-            smooth_lddt_loss = calc_smooth_lddt_loss(
+            smooth_lddt_loss = self.smooth_lddt_loss(
                 denoised_atom_pos,
-                normalized_atom_pos,
+                atom_pos_ground_truth,
                 atom_is_dna,
-                atom_is_rna
-            ).mean()
+                atom_is_rna,
+                coords_mask = atom_mask
+            )
 
-            loss = loss + smooth_lddt_loss
+            total_loss = total_loss + smooth_lddt_loss
 
-        if not return_denoised_pos:
-            return loss
+        # calculate loss breakdown
 
-        return loss, denoised_atom_pos
+        loss_breakdown = DiffusionLossBreakdown(mse_loss, bond_loss, smooth_lddt_loss)
 
+        return ElucidatedAtomDiffusionReturn(total_loss, denoised_atom_pos, loss_breakdown, sigmas)
 
 # modules todo
 
 class SmoothLDDTLoss(Module):
     """ Algorithm 27 """
 
     @typecheck
-    def __init__(self, nucleic_acid_cutoff: float = 30.0, other_cutoff: float = 15.0):
+    def __init__(
+        self,
+        nucleic_acid_cutoff: float = 30.0,
+        other_cutoff: float = 15.0
+    ):
         super().__init__()
         self.nucleic_acid_cutoff = nucleic_acid_cutoff
         self.other_cutoff = other_cutoff
 
     @typecheck
     def forward(
         self,
         pred_coords: Float['b n 3'],
         true_coords: Float['b n 3'],
         is_dna: Bool['b n'],
-        is_rna: Bool['b n']
+        is_rna: Bool['b n'],
+        coords_mask: Bool['b n'] | None = None,
     ) -> Float['']:
         """
-        pred_coords: predicted coordinates (b, n, 3)
-        true_coords: true coordinates (b, n, 3)
-        is_dna: boolean tensor indicating DNA atoms (b, n)
-        is_rna: boolean tensor indicating RNA atoms (b, n)
+        pred_coords: predicted coordinates
+        true_coords: true coordinates
+        is_dna: boolean tensor indicating DNA atoms
+        is_rna: boolean tensor indicating RNA atoms
         """
         # Compute distances between all pairs of atoms
         pred_dists = torch.cdist(pred_coords, pred_coords)
         true_dists = torch.cdist(true_coords, true_coords)
 
         # Compute distance difference for all pairs of atoms
         dist_diff = torch.abs(true_dists - pred_dists)
@@ -1823,139 +2222,175 @@
             F.sigmoid(1.0 - dist_diff) +
             F.sigmoid(2.0 - dist_diff) +
             F.sigmoid(4.0 - dist_diff)
         ) / 4.0
 
         # Restrict to bespoke inclusion radius
         is_nucleotide = is_dna | is_rna
-        is_nucleotide_pair = is_nucleotide.unsqueeze(-1) & is_nucleotide.unsqueeze(-2)
+        is_nucleotide_pair = einx.logical_and('b i, b j -> b i j', is_nucleotide, is_nucleotide)
+
         inclusion_radius = torch.where(
             is_nucleotide_pair,
             true_dists < self.nucleic_acid_cutoff,
             true_dists < self.other_cutoff
         )
 
         # Compute mean, avoiding self term
-        mask = torch.logical_and(inclusion_radius, torch.logical_not(torch.eye(pred_coords.shape[1], dtype=torch.bool, device=pred_coords.device)))
+        mask = inclusion_radius & ~torch.eye(pred_coords.shape[1], dtype=torch.bool, device=pred_coords.device)
+
+        # Take into account variable lengthed atoms in batch
+        if exists(coords_mask):
+            paired_coords_mask = einx.logical_and('b i, b j -> b i j', coords_mask, coords_mask)
+            mask = mask & paired_coords_mask
+
+        # Calculate masked averaging
         lddt_sum = (eps * mask).sum(dim=(-1, -2))
         lddt_count = mask.sum(dim=(-1, -2))
         lddt = lddt_sum / lddt_count.clamp(min=1)
 
-        return 1 - lddt.mean()
+        return 1. - lddt.mean()
 
 class WeightedRigidAlign(Module):
     """ Algorithm 28 """
-    def __init__(self):
-        super().__init__()
 
     @typecheck
     def forward(
         self,
-        pred_coords: Float['b n 3'],
-        true_coords: Float['b n 3'],
-        weights: Float['b n']
+        pred_coords: Float['b n 3'],       # predicted coordinates
+        true_coords: Float['b n 3'],       # true coordinates
+        weights: Float['b n'],             # weights for each atom
+        mask: Bool['b n'] | None = None    # mask for variable lengths
     ) -> Float['b n 3']:
-        """
-        pred_coords: predicted coordinates (b, n, 3)
-        true_coords: true coordinates (b, n, 3)
-        weights: weights for each atom (b, n)
-        """
+        batch_size, num_points, dim = pred_coords.shape
+
+        if exists(mask):
+            # zero out all predicted and true coordinates where not an atom
+            pred_coords = einx.where('b n, b n c, -> b n c', mask, pred_coords, 0.)
+            true_coords = einx.where('b n, b n c, -> b n c', mask, true_coords, 0.)
+            weights = einx.where('b n, b n, -> b n', mask, weights, 0.)
+
+        # Take care of weights broadcasting for coordinate dimension
+        weights = rearrange(weights, 'b n -> b n 1')
 
         # Compute weighted centroids
-        pred_centroid = (pred_coords * weights.unsqueeze(-1)).sum(dim=1) / weights.sum(dim=1, keepdim=True)
-        true_centroid = (true_coords * weights.unsqueeze(-1)).sum(dim=1) / weights.sum(dim=1, keepdim=True)
+        pred_centroid = (pred_coords * weights).sum(dim=1, keepdim=True) / weights.sum(dim=1, keepdim=True)
+        true_centroid = (true_coords * weights).sum(dim=1, keepdim=True) / weights.sum(dim=1, keepdim=True)
 
         # Center the coordinates
-        pred_coords_centered = pred_coords - pred_centroid.unsqueeze(1)
-        true_coords_centered = true_coords - true_centroid.unsqueeze(1)
+        pred_coords_centered = pred_coords - pred_centroid
+        true_coords_centered = true_coords - true_centroid
+
+        if num_points < (dim + 1):
+            print(
+                "Warning: The size of one of the point clouds is <= dim+1. "
+                + "`WeightedRigidAlign` cannot return a unique rotation."
+            )
 
         # Compute the weighted covariance matrix
-        cov_matrix = torch.einsum('bni,bnj->bij', true_coords_centered * weights.unsqueeze(-1), pred_coords_centered)
+        cov_matrix = einsum(weights * true_coords_centered, pred_coords_centered, 'b n i, b n j -> b i j')
 
         # Compute the SVD of the covariance matrix
-        U, _, V = torch.svd(cov_matrix)
+        U, S, V = torch.svd(cov_matrix)
+
+        # Catch ambiguous rotation by checking the magnitude of singular values
+        if (S.abs() <= 1e-15).any() and not (num_points < (dim + 1)):
+            print(
+                "Warning: Excessively low rank of "
+                + "cross-correlation between aligned point clouds. "
+                + "`WeightedRigidAlign` cannot return a unique rotation."
+            )
 
         # Compute the rotation matrix
-        rot_matrix = torch.einsum('bij,bjk->bik', U, V)
+        rot_matrix = einsum(U, V, 'b i j, b k j -> b i k')
 
         # Ensure proper rotation matrix with determinant 1
-        det = torch.det(rot_matrix)
-        det_mask = det < 0
-        V_fixed = V.clone()
-        V_fixed[det_mask, :, -1] *= -1
-        rot_matrix[det_mask] = torch.einsum('bij,bjk->bik', U[det_mask], V_fixed[det_mask])
+        F = torch.eye(dim, dtype=cov_matrix.dtype, device=cov_matrix.device)[None].repeat(batch_size, 1, 1)
+        F[:, -1, -1] = torch.det(rot_matrix)
+        rot_matrix = einsum(U, F, V, "b i j, b j k, b l k -> b i l")
 
         # Apply the rotation and translation
-        aligned_coords = torch.einsum('bni,bij->bnj', pred_coords_centered, rot_matrix) + true_centroid.unsqueeze(1)
+        aligned_coords = einsum(pred_coords_centered, rot_matrix, 'b n i, b j i -> b n j') + true_centroid
+        aligned_coords.detach_()
 
-        return aligned_coords.detach()
+        return aligned_coords
 
 class ExpressCoordinatesInFrame(Module):
     """ Algorithm  29 """
 
-    def __init__(self, eps = 1e-8):
+    def __init__(
+        self,
+        eps = 1e-8
+    ):
         super().__init__()
         self.eps = eps
 
     @typecheck
     def forward(
         self,
         coords: Float['b m 3'],
         frame: Float['b m 3 3'] | Float['b 3 3'] | Float['3 3']
     ) -> Float['b m 3']:
         """
-        coords: coordinates to be expressed in the given frame (b, 3)
-        frame: frame defined by three points (b, 3, 3)
+        coords: coordinates to be expressed in the given frame
+        frame: frame defined by three points
         """
 
         if frame.ndim == 2:
             frame = rearrange(frame, 'fr fc -> 1 1 fr fc')
         elif frame.ndim == 3:
             frame = rearrange(frame, 'b fr fc -> b 1 fr fc')
 
-        # Extract frame points
-        a, b, c = frame.unbind(dim = -1)
-
-        # Compute unit vectors of the frame
-        e1 = F.normalize(a - b, dim = -1, eps = self.eps)
-        e2 = F.normalize(c - b, dim = -1, eps = self.eps)
-        e3 = torch.cross(e1, e2, dim = -1)
-
-        # Express coordinates in the frame basis
-        v = coords - b
-
-        transformed_coords = torch.stack([
-            einsum(v, e1, '... i, ... i -> ...'),
-            einsum(v, e2, '... i, ... i -> ...'),
-            einsum(v, e3, '... i, ... i -> ...')
-        ], dim = -1)
+        # Extract frame atoms
+        a, b, c = frame.unbind(dim=-1)
+        w1 = F.normalize(a - b, dim=-1, eps=self.eps)
+        w2 = F.normalize(c - b, dim=-1, eps=self.eps)
+
+        # Build orthonormal basis
+        e1 = F.normalize(w1 + w2, dim=-1, eps=self.eps)
+        e2 = F.normalize(w2 - w1, dim=-1, eps=self.eps)
+        e3 = torch.cross(e1, e2, dim=-1)
+
+        # Project onto frame basis
+        d = coords - b
+        transformed_coords = torch.stack(
+            [
+                einsum(d, e1, '... i, ... i -> ...'),
+                einsum(d, e2, '... i, ... i -> ...'),
+                einsum(d, e3, '... i, ... i -> ...'),
+            ],
+            dim=-1,
+        )
 
         return transformed_coords
 
 class ComputeAlignmentError(Module):
     """ Algorithm 30 """
+
     @typecheck
-    def __init__(self, eps: float = 1e-8):
+    def __init__(
+        self,
+        eps: float = 1e-8
+    ):
         super().__init__()
         self.eps = eps
         self.express_coordinates_in_frame = ExpressCoordinatesInFrame()
 
     @typecheck
     def forward(
         self,
         pred_coords: Float['b n 3'],
         true_coords: Float['b n 3'],
         pred_frames: Float['b n 3 3'],
         true_frames: Float['b n 3 3']
     ) -> Float['b n']:
         """
-        pred_coords: predicted coordinates (b, n, 3)
-        true_coords: true coordinates (b, n, 3)
-        pred_frames: predicted frames (b, n, 3, 3)
-        true_frames: true frames (b, n, 3, 3)
+        pred_coords: predicted coordinates
+        true_coords: true coordinates
+        pred_frames: predicted frames
+        true_frames: true frames
         """
         # Express predicted coordinates in predicted frames
         pred_coords_transformed = self.express_coordinates_in_frame(pred_coords, pred_frames)
 
         # Express true coordinates in true frames
         true_coords_transformed = self.express_coordinates_in_frame(true_coords, true_frames)
 
@@ -1964,103 +2399,115 @@
             torch.sum((pred_coords_transformed - true_coords_transformed) ** 2, dim=-1) + self.eps
         )
 
         return alignment_errors
 
 class CentreRandomAugmentation(Module):
     """ Algorithm 19 """
+
     @typecheck
     def __init__(self, trans_scale: float = 1.0):
         super().__init__()
         self.trans_scale = trans_scale
+        self.register_buffer('dummy', torch.tensor(0), persistent = False)
+
+    @property
+    def device(self):
+        return self.dummy.device
 
     @typecheck
     def forward(self, coords: Float['b n 3']) -> Float['b n 3']:
         """
-        coords: coordinates to be augmented (b, n, 3)
+        coords: coordinates to be augmented
         """
+        batch_size = coords.shape[0]
+
         # Center the coordinates
         centered_coords = coords - coords.mean(dim=1, keepdim=True)
 
         # Generate random rotation matrix
-        rotation_matrix = self._random_rotation_matrix(coords.device)
+        rotation_matrix = self._random_rotation_matrix(batch_size)
 
         # Generate random translation vector
-        translation_vector = self._random_translation_vector(coords.device)
+        translation_vector = self._random_translation_vector(batch_size)
+        translation_vector = rearrange(translation_vector, 'b c -> b 1 c')
 
         # Apply rotation and translation
-        augmented_coords = torch.einsum('bni,ij->bnj', centered_coords, rotation_matrix) + translation_vector
+        augmented_coords = einsum(centered_coords, rotation_matrix, 'b n i, b j i -> b n j') + translation_vector
 
         return augmented_coords
 
     @typecheck
-    def _random_rotation_matrix(self, device: torch.device) -> Float['3 3']:
+    def _random_rotation_matrix(self, batch_size: int) -> Float['b 3 3']:
         # Generate random rotation angles
-        angles = torch.rand(3, device=device) * 2 * torch.pi
+        angles = torch.rand((batch_size, 3), device = self.device) * 2 * torch.pi
 
         # Compute sine and cosine of angles
         sin_angles = torch.sin(angles)
         cos_angles = torch.cos(angles)
 
         # Construct rotation matrix
-        rotation_matrix = torch.eye(3, device=device)
-        rotation_matrix[0, 0] = cos_angles[0] * cos_angles[1]
-        rotation_matrix[0, 1] = cos_angles[0] * sin_angles[1] * sin_angles[2] - sin_angles[0] * cos_angles[2]
-        rotation_matrix[0, 2] = cos_angles[0] * sin_angles[1] * cos_angles[2] + sin_angles[0] * sin_angles[2]
-        rotation_matrix[1, 0] = sin_angles[0] * cos_angles[1]
-        rotation_matrix[1, 1] = sin_angles[0] * sin_angles[1] * sin_angles[2] + cos_angles[0] * cos_angles[2]
-        rotation_matrix[1, 2] = sin_angles[0] * sin_angles[1] * cos_angles[2] - cos_angles[0] * sin_angles[2]
-        rotation_matrix[2, 0] = -sin_angles[1]
-        rotation_matrix[2, 1] = cos_angles[1] * sin_angles[2]
-        rotation_matrix[2, 2] = cos_angles[1] * cos_angles[2]
+        eye = torch.eye(3, device = self.device)
+        rotation_matrix = repeat(eye, 'i j -> b i j', b = batch_size).clone()
+
+        rotation_matrix[:, 0, 0] = cos_angles[:, 0] * cos_angles[:, 1]
+        rotation_matrix[:, 0, 1] = cos_angles[:, 0] * sin_angles[:, 1] * sin_angles[:, 2] - sin_angles[:, 0] * cos_angles[:, 2]
+        rotation_matrix[:, 0, 2] = cos_angles[:, 0] * sin_angles[:, 1] * cos_angles[:, 2] + sin_angles[:, 0] * sin_angles[:, 2]
+        rotation_matrix[:, 1, 0] = sin_angles[:, 0] * cos_angles[:, 1]
+        rotation_matrix[:, 1, 1] = sin_angles[:, 0] * sin_angles[:, 1] * sin_angles[:, 2] + cos_angles[:, 0] * cos_angles[:, 2]
+        rotation_matrix[:, 1, 2] = sin_angles[:, 0] * sin_angles[:, 1] * cos_angles[:, 2] - cos_angles[:, 0] * sin_angles[:, 2]
+        rotation_matrix[:, 2, 0] = -sin_angles[:, 1]
+        rotation_matrix[:, 2, 1] = cos_angles[:, 1] * sin_angles[:, 2]
+        rotation_matrix[:, 2, 2] = cos_angles[:, 1] * cos_angles[:, 2]
 
         return rotation_matrix
 
     @typecheck
-    def _random_translation_vector(self, device: torch.device) -> Float['3']:
+    def _random_translation_vector(self, batch_size: int) -> Float['b 3']:
         # Generate random translation vector
-        translation_vector = torch.randn(3, device=device) * self.trans_scale
+        translation_vector = torch.randn((batch_size, 3), device = self.device) * self.trans_scale
         return translation_vector
 
 # input embedder
 
-EmbeddedInputs = namedtuple('EmbeddedInputs', [
-    'single_inputs',
-    'single_init',
-    'pairwise_init',
-    'atom_feats',
-    'atompair_feats'
-])
+class EmbeddedInputs(NamedTuple):
+    single_inputs: Float['b n ds']
+    single_init: Float['b n ds']
+    pairwise_init: Float['b n n dp']
+    atom_feats: Float['b m da']
+    atompair_feats: Float['b m m dap']
 
 class InputFeatureEmbedder(Module):
     """ Algorithm 2 """
 
     def __init__(
         self,
         *,
         dim_atom_inputs,
-        dim_additional_residue_feats,
+        dim_atompair_inputs = 5,
         atoms_per_window = 27,
         dim_atom = 128,
         dim_atompair = 16,
         dim_token = 384,
         dim_single = 384,
         dim_pairwise = 128,
         atom_transformer_blocks = 3,
         atom_transformer_heads = 4,
-        atom_transformer_kwargs: dict = dict()
+        atom_transformer_kwargs: dict = dict(),
     ):
         super().__init__()
         self.atoms_per_window = atoms_per_window
 
         self.to_atom_feats = LinearNoBias(dim_atom_inputs, dim_atom)
 
+        self.to_atompair_feats = LinearNoBias(dim_atompair_inputs, dim_atompair)
+
         self.atom_repr_to_atompair_feat_cond = nn.Sequential(
             nn.LayerNorm(dim_atom),
-            LinearNoBiasThenOuterSum(dim_atom, dim_atompair),
+            LinearNoBias(dim_atom, dim_atompair * 2),
             nn.ReLU()
         )
 
         self.atompair_feats_mlp = nn.Sequential(
             LinearNoBias(dim_atompair, dim_atompair),
             nn.ReLU(),
             LinearNoBias(dim_atompair, dim_atompair),
@@ -2076,61 +2523,75 @@
             dim_pairwise = dim_atompair,
             attn_window_size = atoms_per_window,
             **atom_transformer_kwargs
         )
 
         self.atom_feats_to_pooled_token = AtomToTokenPooler(
             dim = dim_atom,
-            dim_out = dim_token,
-            atoms_per_window = atoms_per_window
+            dim_out = dim_token
         )
 
-        dim_single_input = dim_token + dim_additional_residue_feats
-
-        self.dim_additional_residue_feats = dim_additional_residue_feats
+        dim_single_input = dim_token + ADDITIONAL_RESIDUE_FEATS
 
         self.single_input_to_single_init = LinearNoBias(dim_single_input, dim_single)
         self.single_input_to_pairwise_init = LinearNoBiasThenOuterSum(dim_single_input, dim_pairwise)
 
     @typecheck
     def forward(
         self,
         *,
         atom_inputs: Float['b m dai'],
+        atompair_inputs: Float['b m m dapi'] | Float['b nw w1 w2 dapi'],
         atom_mask: Bool['b m'],
-        atompair_feats: Float['b m m dap'],
-        additional_residue_feats: Float['b n rf'],
-    ) -> EmbeddedInputs[
-        Float['b n ds'],
-        Float['b n ds'],
-        Float['b n n dp'],
-        Float['b m da'],
-        Float['b m m dap']
-    ]:
+        additional_residue_feats: Float[f'b n {ADDITIONAL_RESIDUE_FEATS}'],
+        residue_atom_lens: Int['b n'],
+
+    ) -> EmbeddedInputs:
 
-        assert additional_residue_feats.shape[-1] == self.dim_additional_residue_feats
+        assert additional_residue_feats.shape[-1] == ADDITIONAL_RESIDUE_FEATS
 
         w = self.atoms_per_window
 
         atom_feats = self.to_atom_feats(atom_inputs)
+        atompair_feats = self.to_atompair_feats(atompair_inputs)
+
+        # window the atom pair features before passing to atom encoder and decoder
+
+        is_windowed = atompair_inputs.ndim == 5
+
+        if not is_windowed:
+            atompair_feats = full_pairwise_repr_to_windowed(atompair_feats, window_size = w)
+
+        # condition atompair with atom repr
 
         atom_feats_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
-        atompair_feats = atom_feats_cond + atompair_feats
+
+        atom_feats_cond = pad_to_multiple(atom_feats_cond, w, dim = 1)
+        atom_feats_cond = rearrange(atom_feats_cond, 'b (nw w) dap -> b nw w dap', w = w)
+
+        atom_feats_cond_row, atom_feats_cond_col = atom_feats_cond.chunk(2, dim = -1)
+        atom_feats_cond_col = concat_neighboring_windows(atom_feats_cond_col, dim_seq = 1, dim_window = -2)
+
+        atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap',atompair_feats, atom_feats_cond_row)
+        atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap',atompair_feats, atom_feats_cond_col)
+
+        # initial atom transformer
 
         atom_feats = self.atom_transformer(
             atom_feats,
             single_repr = atom_feats,
             pairwise_repr = atompair_feats
         )
 
         atompair_feats = self.atompair_feats_mlp(atompair_feats) + atompair_feats
 
         single_inputs = self.atom_feats_to_pooled_token(
             atom_feats = atom_feats,
-            atom_mask = atom_mask
+            atom_mask = atom_mask,
+            residue_atom_lens = residue_atom_lens
         )
 
         single_inputs = torch.cat((single_inputs, additional_residue_feats), dim = -1)
 
         single_init = self.single_input_to_single_init(single_inputs)
         pairwise_init = self.single_input_to_pairwise_init(single_inputs)
 
@@ -2161,30 +2622,29 @@
     ) -> Float['b l n n']:
 
         logits = self.to_distogram_logits(pairwise_repr)
         return logits
 
 # confidence head
 
-ConfidenceHeadLogits = namedtuple('ConfidenceHeadLogits', [
-    'pae',
-    'pde',
-    'plddt',
-    'resolved'
-])
+class ConfidenceHeadLogits(NamedTuple):
+    pae: Float['b pae n n'] | None
+    pde: Float['b pde n n']
+    plddt: Float['b plddt n']
+    resolved: Float['b 2 n']
 
 class ConfidenceHead(Module):
     """ Algorithm 31 """
 
     @typecheck
     def __init__(
         self,
         *,
         dim_single_inputs,
-        atompair_dist_bins: Float['d'],
+        atompair_dist_bins: Float[' d'],
         dim_single = 384,
         dim_pairwise = 128,
         num_plddt_bins = 50,
         num_pde_bins = 64,
         num_pae_bins = 64,
         pairformer_depth = 4,
         pairformer_kwargs: dict = dict()
@@ -2237,20 +2697,15 @@
         single_inputs_repr: Float['b n dsi'],
         single_repr: Float['b n ds'],
         pairwise_repr: Float['b n n dp'],
         pred_atom_pos: Float['b n 3'],
         mask: Bool['b n'] | None = None,
         return_pae_logits = True
 
-    ) -> ConfidenceHeadLogits[
-        Float['b pae n n'] | None,
-        Float['b pde n n'],
-        Float['b plddt n'],
-        Float['b resolved n']
-    ]:
+    ) -> ConfidenceHeadLogits:
 
         pairwise_repr = pairwise_repr + self.single_inputs_to_pairwise(single_inputs_repr)
 
         # interatomic distances - embed and add to pairwise
 
         interatom_dist = torch.cdist(pred_atom_pos, pred_atom_pos, p = 2)
 
@@ -2283,47 +2738,54 @@
 
         # return all logits
 
         return ConfidenceHeadLogits(pae_logits, pde_logits, plddt_logits, resolved_logits)
 
 # main class
 
-LossBreakdown = namedtuple('LossBreakdown', [
-    'distogram',
-    'pae',
-    'pde',
-    'plddt',
-    'resolved'
-])
+class LossBreakdown(NamedTuple):
+    total_loss: Float['']
+    total_diffusion: Float['']
+    distogram: Float['']
+    pae: Float['']
+    pde: Float['']
+    plddt: Float['']
+    resolved: Float['']
+    confidence: Float['']
+    diffusion_mse: Float['']
+    diffusion_bond: Float['']
+    diffusion_smooth_lddt: Float['']
 
 class Alphafold3(Module):
     """ Algorithm 1 """
 
+    @save_args_and_kwargs
     @typecheck
     def __init__(
         self,
         *,
         dim_atom_inputs,
-        dim_additional_residue_feats,
         dim_template_feats,
         dim_template_model = 64,
         atoms_per_window = 27,
         dim_atom = 128,
+        dim_atompair_inputs = 5,
         dim_atompair = 16,
         dim_input_embedder_token = 384,
         dim_single = 384,
         dim_pairwise = 128,
         dim_token = 768,
-        atompair_dist_bins: Float[' dist_bins'] = torch.linspace(3, 20, 37),
+        distance_bins: Float[' dist_bins'] = torch.linspace(3, 20, 38),
         ignore_index = -1,
-        num_dist_bins = 38,
+        num_dist_bins: int | None = None,
         num_plddt_bins = 50,
         num_pde_bins = 64,
         num_pae_bins = 64,
         sigma_data = 16,
+        diffusion_num_augmentations = 4,
         loss_confidence_weight = 1e-4,
         loss_distogram_weight = 1e-2,
         loss_diffusion_weight = 4.,
         input_embedder_kwargs: dict = dict(
             atom_transformer_blocks = 3,
             atom_transformer_heads = 4,
             atom_transformer_kwargs = dict()
@@ -2365,57 +2827,74 @@
                 num_transitions = 2
             ),
             atom_encoder_depth = 3,
             atom_encoder_heads = 4,
             token_transformer_depth = 24,
             token_transformer_heads = 16,
             atom_decoder_depth = 3,
-            atom_decoder_heads = 4
+            atom_decoder_heads = 4,
+            serial = True # believe they have an error on Algorithm 23. lacking a residual - default to serial architecture until further news
         ),
         edm_kwargs: dict = dict(
             sigma_min = 0.002,
             sigma_max = 80,
             rho = 7,
             P_mean = -1.2,
             P_std = 1.2,
             S_churn = 80,
             S_tmin = 0.05,
             S_tmax = 50,
             S_noise = 1.003,
-        )
+        ),
+        augment_kwargs: dict = dict()
     ):
         super().__init__()
 
+        # atoms per window
+
         self.atoms_per_window = atoms_per_window
 
+        # augmentation
+
+        self.num_augmentations = diffusion_num_augmentations
+        self.augmenter = CentreRandomAugmentation(**augment_kwargs)
+
         # input feature embedder
 
         self.input_embedder = InputFeatureEmbedder(
             dim_atom_inputs = dim_atom_inputs,
-            dim_additional_residue_feats = dim_additional_residue_feats,
+            dim_atompair_inputs = dim_atompair_inputs,
             atoms_per_window = atoms_per_window,
             dim_atom = dim_atom,
             dim_atompair = dim_atompair,
             dim_token = dim_input_embedder_token,
             dim_single = dim_single,
             dim_pairwise = dim_pairwise,
             **input_embedder_kwargs
         )
 
-        dim_single_inputs = dim_input_embedder_token + dim_additional_residue_feats
+        dim_single_inputs = dim_input_embedder_token + ADDITIONAL_RESIDUE_FEATS
 
         # relative positional encoding
         # used by pairwise in main alphafold2 trunk
         # and also in the diffusion module separately from alphafold3
 
         self.relative_position_encoding = RelativePositionEncoding(
             dim_out = dim_pairwise,
             **relative_position_encoding_kwargs
         )
 
+        # token bonds
+        # Algorithm 1 - line 5
+
+        self.token_bond_to_pairwise_feat = nn.Sequential(
+            Rearrange('... -> ... 1'),
+            LinearNoBias(1, dim_pairwise)
+        )
+
         # templates
 
         self.template_embedder = TemplateEmbedder(
             dim_template_feats = dim_template_feats,
             dim = dim_template_model,
             dim_pairwise = dim_pairwise,
             **template_embedder_kwargs
@@ -2468,22 +2947,27 @@
             self.diffusion_module,
             sigma_data = sigma_data,
             **edm_kwargs
         )
 
         # logit heads
 
+        self.register_buffer('distance_bins', distance_bins)
+        num_dist_bins = default(num_dist_bins, len(distance_bins))
+
+        assert len(distance_bins) == num_dist_bins, '`distance_bins` must have a length equal to the `num_dist_bins` passed in'
+
         self.distogram_head = DistogramHead(
             dim_pairwise = dim_pairwise,
             num_dist_bins = num_dist_bins
         )
 
         self.confidence_head = ConfidenceHead(
             dim_single_inputs = dim_single_inputs,
-            atompair_dist_bins = atompair_dist_bins,
+            atompair_dist_bins = distance_bins,
             dim_single = dim_single,
             dim_pairwise = dim_pairwise,
             num_plddt_bins = num_plddt_bins,
             num_pde_bins = num_pde_bins,
             num_pae_bins = num_pae_bins,
             **confidence_head_kwargs
         )
@@ -2497,65 +2981,174 @@
 
         self.register_buffer('zero', torch.tensor(0.), persistent = False)
 
     @property
     def device(self):
         return self.zero.device
 
+    @property
+    def state_dict_with_init_args(self):
+        return dict(
+            version = self._version,
+            init_args_and_kwargs = self._args_and_kwargs,
+            state_dict = self.state_dict()
+        )
+
+    @typecheck
+    def save(self, path: str | Path, overwrite = False):
+        if isinstance(path, str):
+            path = Path(path)
+
+        assert not path.is_dir() and (not path.exists() or overwrite)
+
+        path.parent.mkdir(exist_ok = True, parents = True)
+
+        package = dict(
+            model = self.state_dict_with_init_args
+        )
+
+        torch.save(package, str(path))
+
+    @typecheck
+    def load(self, path: str | Path, strict = False):
+        if isinstance(path, str):
+            path = Path(path)
+
+        assert path.exists() and not path.is_dir()
+
+        package = torch.load(str(path), map_location = 'cpu')
+
+        model_package = package['model']
+        current_version = version('alphafold3_pytorch')
+
+        if model_package['version'] != current_version:
+            print(f'loading a saved model from version {model_package["version"]} but you are on version {current_version}')
+
+        self.load_state_dict(model_package['state_dict'], strict = strict)
+
+    @staticmethod
+    @typecheck
+    def init_and_load(path: str | Path):
+        if isinstance(path, str):
+            path = Path(path)
+
+        assert path.exists() and not path.is_dir()
+
+        package = torch.load(str(path), map_location = 'cpu')
+
+        model_package = package['model']
+
+        args, kwargs = model_package['init_args_and_kwargs']
+        alphafold3 = Alphafold3(*args, **kwargs)
+
+        alphafold3.load(path)
+        return alphafold3
+
     @typecheck
     def forward(
         self,
         *,
         atom_inputs: Float['b m dai'],
-        atom_mask: Bool['b m'],
-        atompair_feats: Float['b m m dap'],
-        additional_residue_feats: Float['b n rf'],
-        msa: Float['b s n d'],
-        templates: Float['b t n n dt'],
-        template_mask: Bool['b t'],
+        atompair_inputs: Float['b m m dapi'] | Float['b nw w1 w2 dapi'],
+        additional_residue_feats: Float[f'b n {ADDITIONAL_RESIDUE_FEATS}'],
+        residue_atom_lens: Int['b n'],
+        atom_mask: Bool['b m'] | None = None,
+        token_bond: Bool['b n n'] | None = None,
+        msa: Float['b s n d'] | None = None,
+        msa_mask: Bool['b s'] | None = None,
+        templates: Float['b t n n dt'] | None = None,
+        template_mask: Bool['b t'] | None = None,
         num_recycling_steps: int = 1,
         diffusion_add_bond_loss: bool = False,
+        diffusion_add_smooth_lddt_loss: bool = False,
         residue_atom_indices: Int['b n'] | None = None,
         num_sample_steps: int | None = None,
         atom_pos: Float['b m 3'] | None = None,
         distance_labels: Int['b n n'] | None = None,
         pae_labels: Int['b n n'] | None = None,
         pde_labels: Int['b n n'] | None = None,
         plddt_labels: Int['b n'] | None = None,
         resolved_labels: Int['b n'] | None = None,
-    ) -> Float['b m 3'] | Float['']:
+        return_loss_breakdown = False,
+        return_loss_if_possible: bool = True,
+        num_rollout_steps: int = 20,
+    ) -> Float['b m 3'] | Float[''] | Tuple[Float[''], LossBreakdown]:
 
-        w = self.atoms_per_window
+        atom_seq_len = atom_inputs.shape[-2]
+
+        assert exists(residue_atom_lens) or exists(atom_mask)
+
+        # if atompair inputs are not windowed, window it
+
+        is_atompair_inputs_windowed = atompair_inputs.ndim == 5
+
+        if not is_atompair_inputs_windowed:
+            atompair_inputs = full_pairwise_repr_to_windowed(atompair_inputs, window_size = self.atoms_per_window)
+
+        # handle atom mask
+
+        total_atoms = residue_atom_lens.sum(dim = -1)
+        atom_mask = lens_to_mask(total_atoms, max_len = atom_seq_len)
+
+        # handle offsets for residue atom indices
+
+        if exists(residue_atom_indices):
+            residue_atom_indices += F.pad(residue_atom_lens, (-1, 1), value = 0)
+
+        # get atom sequence length and residue sequence length depending on whether using packed atomic seq
+
+        seq_len = residue_atom_lens.shape[-1]
 
         # embed inputs
 
         (
             single_inputs,
             single_init,
             pairwise_init,
             atom_feats,
             atompair_feats
         ) = self.input_embedder(
             atom_inputs = atom_inputs,
+            atompair_inputs = atompair_inputs,
             atom_mask = atom_mask,
-            atompair_feats = atompair_feats,
-            additional_residue_feats = additional_residue_feats
+            additional_residue_feats = additional_residue_feats,
+            residue_atom_lens = residue_atom_lens
         )
 
         # relative positional encoding
 
         relative_position_encoding = self.relative_position_encoding(
             additional_residue_feats = additional_residue_feats
         )
 
         pairwise_init = pairwise_init + relative_position_encoding
 
-        # pairwise mask
+        # token bond features
+
+        if exists(token_bond):
+            # well do some precautionary standardization
+            # (1) mask out diagonal - token to itself does not count as a bond
+            # (2) symmetrize, in case it is not already symmetrical (could also throw an error)
+
+            token_bond = token_bond | rearrange(token_bond, 'b i j -> b j i')
+            diagonal = torch.eye(seq_len, device = self.device, dtype = torch.bool)
+            token_bond.masked_fill_(diagonal, False)
+        else:
+            seq_arange = torch.arange(seq_len, device = self.device)
+            token_bond = einx.subtract('i, j -> i j', seq_arange, seq_arange).abs() == 1
+
+        token_bond_feats = self.token_bond_to_pairwise_feat(token_bond.float())
 
-        mask = reduce(atom_mask, 'b (n w) -> b n', w = w, reduction = 'any')
+        pairwise_init = pairwise_init + token_bond_feats
+
+        # residue mask and pairwise mask
+
+        total_atoms = residue_atom_lens.sum(dim = -1)
+        mask = lens_to_mask(total_atoms, max_len = seq_len)
+    
         pairwise_mask = einx.logical_and('b i, b j -> b i j', mask, mask)
 
         # init recycled single and pairwise
 
         recycled_pairwise = recycled_single = None
         single = pairwise = None
 
@@ -2576,33 +3169,36 @@
             single = single_init + recycled_single
             pairwise = pairwise_init + recycled_pairwise
 
             # else go through main transformer trunk from alphafold2
 
             # templates
 
-            embedded_template = self.template_embedder(
-                templates = templates,
-                template_mask = template_mask,
-                pairwise_repr = pairwise,
-                mask = mask
-            )
+            if exists(templates):
+                embedded_template = self.template_embedder(
+                    templates = templates,
+                    template_mask = template_mask,
+                    pairwise_repr = pairwise,
+                    mask = mask
+                )
 
-            pairwise = embedded_template + pairwise
+                pairwise = embedded_template + pairwise
 
             # msa
 
-            embedded_msa = self.msa_module(
-                msa = msa,
-                single_repr = single,
-                pairwise_repr = pairwise,
-                mask = mask
-            )
+            if exists(msa):
+                embedded_msa = self.msa_module(
+                    msa = msa,
+                    single_repr = single,
+                    pairwise_repr = pairwise,
+                    mask = mask,
+                    msa_mask = msa_mask
+                )
 
-            pairwise = embedded_msa + pairwise
+                pairwise = embedded_msa + pairwise
 
             # main attention trunk (pairformer)
 
             single, pairwise = self.pairformer(
                 single_repr = single,
                 pairwise_repr = pairwise,
                 mask = mask
@@ -2616,79 +3212,154 @@
         confidence_head_labels = (pae_labels, pde_labels, plddt_labels, resolved_labels)
         all_labels = (distance_labels, *confidence_head_labels)
 
         has_labels = any([*map(exists, all_labels)])
 
         return_loss = atom_pos_given or has_labels
 
-        # setup all the data necessary for conditioning the diffusion module
-
-        diffusion_cond = dict(
-            atom_feats = atom_feats,
-            atompair_feats = atompair_feats,
-            atom_mask = atom_mask,
-            mask = mask,
-            single_trunk_repr = single,
-            single_inputs_repr = single_inputs,
-            pairwise_trunk = pairwise,
-            pairwise_rel_pos_feats = relative_position_encoding
-        )
-
         # if neither atom positions or any labels are passed in, sample a structure and return
 
-        if not return_loss:
+        if not return_loss_if_possible or not return_loss:
             return self.edm.sample(
                 num_sample_steps = num_sample_steps,
-                **diffusion_cond
+                atom_feats = atom_feats,
+                atompair_feats = atompair_feats,
+                atom_mask = atom_mask,
+                mask = mask,
+                single_trunk_repr = single,
+                single_inputs_repr = single_inputs,
+                pairwise_trunk = pairwise,
+                pairwise_rel_pos_feats = relative_position_encoding,
+                residue_atom_lens = residue_atom_lens
             )
 
         # losses default to 0
 
         distogram_loss = diffusion_loss = confidence_loss = pae_loss = pde_loss = plddt_loss = resolved_loss = self.zero
 
-        # otherwise, noise and make it learn to denoise
-
-        if exists(atom_pos):
-            diffusion_loss, denoised_atom_pos = self.edm(
-                atom_pos,
-                additional_residue_feats = additional_residue_feats,
-                add_smooth_lddt_loss = True,
-                return_denoised_pos = True,
-                add_bond_loss = diffusion_add_bond_loss,
-                **diffusion_cond
-            )
-
-        # calculate all logits and losses
+        # calculate distogram logits and losses
 
         ignore = self.ignore_index
 
         # distogram head
 
+        if not exists(distance_labels) and atom_pos_given and exists(residue_atom_indices):
+
+            residue_pos = einx.get_at('b [m] c, b n -> b n c', atom_pos, residue_atom_indices)
+            residue_dist = torch.cdist(residue_pos, residue_pos, p = 2)
+            dist_from_dist_bins = einx.subtract('b m dist, dist_bins -> b m dist dist_bins', residue_dist, self.distance_bins).abs()
+            distance_labels = dist_from_dist_bins.argmin(dim = -1)
+
         if exists(distance_labels):
             distance_labels = torch.where(pairwise_mask, distance_labels, ignore)
             distogram_logits = self.distogram_head(pairwise)
             distogram_loss = F.cross_entropy(distogram_logits, distance_labels, ignore_index = ignore)
 
+        # otherwise, noise and make it learn to denoise
+
+        calc_diffusion_loss = exists(atom_pos)
+
+        if calc_diffusion_loss:
+
+            num_augs = self.num_augmentations
+
+            # take care of augmentation
+            # they did 48 during training, as the trunk did the heavy lifting
+
+            if num_augs > 1:
+                (
+                    atom_pos,
+                    atom_mask,
+                    atom_feats,
+                    atompair_feats,
+                    mask,
+                    pairwise_mask,
+                    single,
+                    single_inputs,
+                    pairwise,
+                    relative_position_encoding,
+                    additional_residue_feats,
+                    residue_atom_indices,
+                    residue_atom_lens,
+                    pae_labels,
+                    pde_labels,
+                    plddt_labels,
+                    resolved_labels,
+
+                ) = tuple(
+                    maybe(repeat)(t, 'b ... -> (b a) ...', a = num_augs)
+                    for t in (
+                        atom_pos,
+                        atom_mask,
+                        atom_feats,
+                        atompair_feats,
+                        mask,
+                        pairwise_mask,
+                        single,
+                        single_inputs,
+                        pairwise,
+                        relative_position_encoding,
+                        additional_residue_feats,
+                        residue_atom_indices,
+                        residue_atom_lens,
+                        pae_labels,
+                        pde_labels,
+                        plddt_labels,
+                        resolved_labels
+                    )
+                )
+
+                atom_pos = self.augmenter(atom_pos)
+
+            diffusion_loss, denoised_atom_pos, diffusion_loss_breakdown, _ = self.edm(
+                atom_pos,
+                additional_residue_feats = additional_residue_feats,
+                add_smooth_lddt_loss = diffusion_add_smooth_lddt_loss,
+                add_bond_loss = diffusion_add_bond_loss,
+                atom_feats = atom_feats,
+                atompair_feats = atompair_feats,
+                atom_mask = atom_mask,
+                mask = mask,
+                single_trunk_repr = single,
+                single_inputs_repr = single_inputs,
+                pairwise_trunk = pairwise,
+                pairwise_rel_pos_feats = relative_position_encoding,
+                residue_atom_lens = residue_atom_lens,
+                return_denoised_pos = True,
+            )
+
         # confidence head
 
         should_call_confidence_head = any([*map(exists, confidence_head_labels)])
         return_pae_logits = exists(pae_labels)
 
-        if should_call_confidence_head:
-            assert exists(atom_pos), 'diffusion module needs to have been called'
+        if calc_diffusion_loss and should_call_confidence_head:
 
-            assert exists(residue_atom_indices)
+            # rollout
 
-            pred_atom_pos = einx.get_at('b (n [w]) c, b n -> b n c', denoised_atom_pos, residue_atom_indices)
+            pred_atom_pos = self.edm.sample(
+                num_sample_steps = num_rollout_steps,
+                atom_feats = atom_feats,
+                atompair_feats = atompair_feats,
+                atom_mask = atom_mask,
+                mask = mask,
+                single_trunk_repr = single,
+                single_inputs_repr = single_inputs,
+                pairwise_trunk = pairwise,
+                pairwise_rel_pos_feats = relative_position_encoding,
+                residue_atom_lens = residue_atom_lens
+            )
+
+            pred_atom_pos = einx.get_at('b [m] c, b n -> b n c', denoised_atom_pos, residue_atom_indices)
 
             logits = self.confidence_head(
-                single_repr = single,
-                single_inputs_repr = single_inputs,
-                pairwise_repr = pairwise,
-                pred_atom_pos = pred_atom_pos,
+                single_repr = single.detach(),
+                single_inputs_repr = single_inputs.detach(),
+                pairwise_repr = pairwise.detach(),
+                pred_atom_pos = pred_atom_pos.detach(),
                 mask = mask,
                 return_pae_logits = return_pae_logits
             )
 
             if exists(pae_labels):
                 pae_labels = torch.where(pairwise_mask, pae_labels, ignore)
                 pae_loss = F.cross_entropy(logits.pae, pae_labels, ignore_index = ignore)
@@ -2711,8 +3382,23 @@
 
         loss = (
             distogram_loss * self.loss_distogram_weight +
             diffusion_loss * self.loss_diffusion_weight +
             confidence_loss * self.loss_confidence_weight
         )
 
-        return loss
+        if not return_loss_breakdown:
+            return loss
+
+        loss_breakdown = LossBreakdown(
+            total_loss = loss,
+            total_diffusion = diffusion_loss,
+            pae = pae_loss,
+            pde = pde_loss,
+            plddt = plddt_loss,
+            resolved = resolved_loss,
+            distogram = distogram_loss,
+            confidence = confidence_loss,
+            **diffusion_loss_breakdown._asdict()
+        )
+
+        return loss, loss_breakdown
```

### Comparing `alphafold3_pytorch-0.0.9/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.1.0/alphafold3_pytorch/attention.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
-from typing import NamedTuple
+from typing import NamedTuple, Tuple
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 from torch.nn import Module
 
 import einx
 from einops import einsum, repeat, rearrange, pack, unpack
 from einops.layers.torch import Rearrange
 
-from alphafold3_pytorch.typing import Float, Int, Bool, typecheck
+from alphafold3_pytorch.typing import (
+    Float,
+    Int,
+    Bool,
+    typecheck
+)
 
 # constants
 
 class Config(NamedTuple):
     enable_flash: bool
     enable_math: bool
     enable_mem_efficient: bool
@@ -32,14 +37,124 @@
 
 def pack_one(t, pattern):
     return pack([t], pattern)
 
 def unpack_one(t, ps, pattern):
     return unpack(t, ps, pattern)[0]
 
+@typecheck
+def pad_at_dim(
+    t,
+    pad: Tuple[int, int],
+    *,
+    dim = -1,
+    value = 0.
+):
+    dims_from_right = (- dim - 1) if dim < 0 else (t.ndim - dim - 1)
+    zeros = ((0, 0) * dims_from_right)
+    return F.pad(t, (*zeros, *pad), value = value)
+
+@typecheck
+def slice_at_dim(
+    t: Tensor,
+    dim_slice: slice,
+    *,
+    dim: int
+):
+    dim += (t.ndim if dim < 0 else 0)
+    colons = [slice(None)] * t.ndim
+    colons[dim] = dim_slice
+    return t[tuple(colons)]
+
+@typecheck
+def pad_or_slice_to(
+    t: Tensor,
+    length: int,
+    *,
+    dim: int,
+    pad_value = 0
+):
+    curr_length = t.shape[dim]
+
+    if curr_length < length:
+        t = pad_at_dim(t, (0, length - curr_length), dim = dim, value = pad_value)
+    elif curr_length > length:
+        t = slice_at_dim(t, slice(0, length), dim = dim)
+
+    return t
+
+@typecheck
+def pad_to_multiple(
+    t: Tensor,
+    multiple: int,
+    *,
+    dim = -1,
+    value = 0.
+):
+    seq_len = t.shape[dim]
+    padding_needed = (multiple - (seq_len % multiple)) % multiple
+
+    if padding_needed == 0:
+        return t
+
+    return pad_at_dim(t, (0, padding_needed), dim = dim, value = value)
+
+@typecheck
+def concat_neighboring_windows(
+    t: Tensor,
+    *,
+    dim_seq: int,
+    dim_window: int
+):
+    t = pad_at_dim(t, (1, 1), dim = dim_seq, value = 0.)
+
+    t = torch.cat((
+        slice_at_dim(t, slice(None, -2), dim = dim_seq),
+        slice_at_dim(t, slice(1, -1), dim = dim_seq),
+        slice_at_dim(t, slice(2, None), dim = dim_seq)
+    ), dim = dim_window)
+
+    return t
+
+# for changing full attention bias matrix to a local windowed one for atom attention
+
+@typecheck
+def full_pairwise_repr_to_windowed(
+    pairwise_repr: Float['... m m dp'],
+    window_size: int
+) -> Float['... n w (w*3) dp']:
+
+    seq_len, device = pairwise_repr.shape[-2], pairwise_repr.device
+
+    padding_needed = (window_size - (seq_len % window_size)) % window_size
+    pairwise_repr = F.pad(pairwise_repr, (0, 0, 0, padding_needed, 0, padding_needed), value = 0.)
+    pairwise_repr = rearrange(pairwise_repr, '... (i w1) (j w2) d -> ... i j w1 w2 d', w1 = window_size, w2 = window_size)
+    pairwise_repr = concat_neighboring_windows(pairwise_repr, dim_seq = -4, dim_window = -2)
+
+    # get the diagonal
+
+    n = torch.arange(pairwise_repr.shape[-4], device = device)
+
+    pairwise_repr = einx.get_at(
+        '... [i j] w1 w2 d, n, n -> ... n w1 w2 d',
+        pairwise_repr, n, n
+    )
+
+    return pairwise_repr
+
+@typecheck
+def full_attn_bias_to_windowed(
+    attn_bias: Float['... m m'],
+    window_size: int
+) -> Float['... n w (w*3)']:
+
+    attn_bias = rearrange(attn_bias, '... -> ... 1')
+    attn_bias = full_pairwise_repr_to_windowed(attn_bias, window_size = window_size)
+    return rearrange(attn_bias, '... 1 -> ...')
+
 # multi-head attention
 
 class Attention(Module):
     @typecheck
     def __init__(
         self,
         *,
@@ -96,15 +211,15 @@
 
     @typecheck
     def forward(
         self,
         seq: Float['b i d'],
         mask: Bool['b n']| None = None,
         context: Float['b j d'] | None = None,
-        attn_bias: Float['... i j'] | None = None
+        attn_bias: Float['... i j'] | Float['... nw w (w*3)'] | None = None
 
     ) -> Float['b i d']:
 
         q = self.to_q(seq)
 
         context_seq = default(context, seq)
         k, v = self.to_kv(context_seq).chunk(2, dim = -1)
@@ -197,70 +312,55 @@
     @typecheck
     def local_attn(
         self,
         q: Float['b h n d'],
         k: Float['b h n d'],
         v: Float['b h n d'],
         mask: Bool['b n'] | None = None,
-        attn_bias: Float['... n n'] | None = None
+        attn_bias: Float['... n n'] | Float['... nw w (w*3)'] | None = None
     ) -> Float['b h n d']:
         """
         simple local attention with a radius of 1 window size
         """
 
         window_size, batch, seq_len, device = self.window_size, q.shape[0], q.shape[-2], q.device
 
         # constitute mask if not given
 
         if not exists(mask):
             mask = torch.ones((batch, seq_len), device = device, dtype = torch.bool)
 
         # pad to multiple of window size if needed
 
-        padding_needed = (window_size - (seq_len % window_size)) % window_size        
+        padding_needed = (window_size - (seq_len % window_size)) % window_size
 
         if padding_needed > 0:
-            q, k, v = tuple(F.pad(t, (0, 0, 0, padding_needed), value = 0.) for t in (q, k, v))
+            q, k, v = tuple(pad_at_dim(t, (0, padding_needed), value = 0., dim = -2) for t in (q, k, v))
             mask = F.pad(mask, (0, padding_needed), value = False)
 
         # break into windows
 
         q, k, v = tuple(rearrange(t, 'b h (n w) d -> b h n w d', w = window_size) for t in (q, k, v))
         mask = rearrange(mask, 'b (n w) -> b n w', w = window_size)
 
         # just do radius of 1 for now
         # perhaps not even necessary, and could try shifted windows (a la Swin)
 
-        k, v = tuple(F.pad(t, (0, 0, 1, 1)) for t in (k, v))
+        k, v = tuple(pad_at_dim(t, (1, 1), dim = -2) for t in (k, v))
         mask = F.pad(mask, (1, 1), value = False)
 
         k, v = tuple(torch.cat((t[..., :-2, :], t[..., 1:-1, :], t[..., 2:, :]), dim = -2) for t in (k, v))
         mask = torch.cat((mask[..., :-2], mask[..., 1:-1], mask[..., 2:]), dim = -1)
 
         # handle attention bias (inefficiently)
 
-        if exists(attn_bias):
-            attn_bias = F.pad(attn_bias, (0, padding_needed, 0, padding_needed), value = 0.)
-            attn_bias = rearrange(attn_bias, '... (i w1) (j w2) -> ... i j w1 w2', w1 = window_size, w2 = window_size)
-            attn_bias = F.pad(attn_bias, (0, 0, 0, 0, 1, 1), value = 0.)
-
-            attn_bias = torch.cat((
-                attn_bias[..., :-2, :, :],
-                attn_bias[..., 1:-1, :, :],
-                attn_bias[..., 2:, :, :]
-            ), dim = -1)
-
-            attn_bias, ps = pack_one(attn_bias, '* i j w1 w2')
-
-            merged_batch = attn_bias.shape[0]
-            diag_mask = torch.eye(attn_bias.shape[1], device = device, dtype = torch.bool)
-            diag_mask = repeat(diag_mask, 'i j -> b i j', b = merged_batch)
+        is_full_attn_bias = attn_bias.shape[-1] == attn_bias.shape[-2]
 
-            attn_bias = rearrange(attn_bias[diag_mask], '(b n) i j -> b n i j', b = merged_batch)
-            attn_bias = unpack_one(attn_bias, ps, '* n i j')
+        if exists(attn_bias) and is_full_attn_bias:
+            attn_bias = full_attn_bias_to_windowed(attn_bias, window_size = window_size)
 
         # carry out attention as usual
 
         scale = q.shape[-1] ** -0.5
 
         q = q * scale
 
@@ -295,23 +395,30 @@
     @typecheck
     def forward(
         self,
         q: Float['b h i d'],
         k: Float['b h j d'],
         v: Float['b h j d'],
         mask: Bool['b j'] | None = None,
-        attn_bias: Float['... i j'] | None = None,
+        attn_bias: Float['... i j'] | Float['... nw w (w*3)'] | None = None,
     ) -> Float['b h i d']:
 
+        is_windowed_attn_bias = None
+
+        if exists(attn_bias):
+            is_windowed_attn_bias = attn_bias.shape[-1] != attn_bias.shape[-2]
+
         # local windowed attention
         # todo (handle attn bias efficiently)
 
         if self.is_local_attn:
             return self.local_attn(q, k, v, mask = mask, attn_bias = attn_bias)
 
+        assert not exists(is_windowed_attn_bias) or not is_windowed_attn_bias
+
         # forward to using flash attention if applicable
 
         can_use_flash = self.flash and not exists(attn_bias), 'flash attention does not support attention bias with gradients'
 
         if can_use_flash:
             return self.flash_attn(q, k, v, mask = mask)
```

### Comparing `alphafold3_pytorch-0.0.9/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.1.0/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.1.0/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/tests/test_af3.py` & `alphafold3_pytorch-0.1.0/tests/test_af3.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,54 +21,93 @@
     InputFeatureEmbedder,
     ConfidenceHead,
     DistogramHead,
     Alphafold3,
 )
 
 from alphafold3_pytorch.alphafold3 import (
-    calc_smooth_lddt_loss
+    mean_pool_with_lens,
+    repeat_consecutive_with_lens,
+    full_pairwise_repr_to_windowed
 )
 
-def test_calc_smooth_lddt_loss():
-    denoised = torch.randn(8, 100, 3)
-    ground_truth = torch.randn(8, 100, 3)
-    is_rna_per_atom = torch.randint(0, 2, (8, 100)).float()
-    is_dna_per_atom = torch.randint(0, 2, (8, 100)).float()
-    
-    loss = calc_smooth_lddt_loss(
-        denoised, 
-        ground_truth, 
-        is_rna_per_atom, 
-        is_dna_per_atom
-    )
-
-    assert torch.all(loss <= 1) and torch.all(loss >= 0)
-
-# ToDo tests
+def test_mean_pool_with_lens():
+    seq = torch.tensor([[[1.], [1.], [1.], [2.], [2.], [2.], [2.], [1.], [1.]]])
+    lens = torch.tensor([[3, 4, 2]]).long()
+    pooled = mean_pool_with_lens(seq, lens)
+
+    assert torch.allclose(pooled, torch.tensor([[[1.], [2.], [1.]]]))
+
+def test_repeat_consecutive_with_lens():
+    seq = torch.tensor([[[1.], [2.], [4.]], [[1.], [2.], [4.]]])
+    lens = torch.tensor([[3, 4, 2], [2, 5, 1]]).long()
+    repeated = repeat_consecutive_with_lens(seq, lens)
+    assert torch.allclose(repeated, torch.tensor([[[1.], [1.], [1.], [2.], [2.], [2.], [2.], [4.], [4.]], [[1.], [1.], [2.], [2.], [2.], [2.], [2.], [4.], [0.]]]))
 
 def test_smooth_lddt_loss():
     pred_coords = torch.randn(2, 100, 3)
     true_coords = torch.randn(2, 100, 3)
     is_dna = torch.randint(0, 2, (2, 100)).bool()
     is_rna = torch.randint(0, 2, (2, 100)).bool()
 
     loss_fn = SmoothLDDTLoss()
     loss = loss_fn(pred_coords, true_coords, is_dna, is_rna)
 
     assert loss.numel() == 1
 
 def test_weighted_rigid_align():
     pred_coords = torch.randn(2, 100, 3)
+    weights = torch.rand(2, 100)
+
+    align_fn = WeightedRigidAlign()
+    aligned_coords = align_fn(pred_coords, pred_coords, weights)
+
+    # `pred_coords` should match itself without any change after alignment
+
+    rmsd = torch.sqrt(((pred_coords - aligned_coords) ** 2).sum(dim=-1).mean(dim=-1))
+    assert (rmsd < 1e-5).all()
+
+    random_augment_fn = CentreRandomAugmentation()
+    aligned_coords = align_fn(random_augment_fn(pred_coords), pred_coords, weights)
+
+    # `pred_coords` should match a random augmentation of itself after alignment
+
+    rmsd = torch.sqrt(((pred_coords - aligned_coords) ** 2).sum(dim=-1).mean(dim=-1))
+    assert (rmsd < 1e-5).all()
+
+def test_weighted_rigid_align_with_mask():
+    pred_coords = torch.randn(2, 100, 3)
     true_coords = torch.randn(2, 100, 3)
     weights = torch.rand(2, 100)
+    mask = torch.randint(0, 2, (2, 100)).bool()
 
     align_fn = WeightedRigidAlign()
-    aligned_coords = align_fn(pred_coords, true_coords, weights)
 
-    assert aligned_coords.shape == pred_coords.shape
+    # with mask
+
+    aligned_coords = align_fn(pred_coords, true_coords, weights, mask = mask)
+
+    # do it one sample at a time without make
+
+    all_aligned_coords = []
+
+    for one_mask, one_pred_coords, one_true_coords, one_weight in zip(mask, pred_coords, true_coords, weights):
+        one_aligned_coords = align_fn(
+            one_pred_coords[one_mask][None, ...],
+            one_true_coords[one_mask][None, ...],
+            one_weight[one_mask][None, ...]
+        )
+
+        all_aligned_coords.append(one_aligned_coords.squeeze(0))
+
+    aligned_coords_without_mask = torch.cat(all_aligned_coords, dim = 0)
+
+    # both ways should come out with about the same results
+
+    assert torch.allclose(aligned_coords[mask], aligned_coords_without_mask, atol=1e-5)
 
 def test_express_coordinates_in_frame():
     batch_size = 2
     num_coords = 100
     coords = torch.randn(batch_size, num_coords, 3)
     frame = torch.randn(batch_size, num_coords, 3, 3)
 
@@ -85,22 +124,23 @@
     broadcastable_batch_and_seq_frame = torch.randn(3, 3)
     transformed_coords = express_fn(coords, broadcastable_batch_and_seq_frame)
 
     assert transformed_coords.shape == (batch_size, num_coords, 3)
 
 def test_compute_alignment_error():
     pred_coords = torch.randn(2, 100, 3)
-    true_coords = torch.randn(2, 100, 3)
     pred_frames = torch.randn(2, 100, 3, 3)
-    true_frames = torch.randn(2, 100, 3, 3)
+
+    # `pred_coords` should match itself in frame basis
 
     error_fn = ComputeAlignmentError()
-    alignment_errors = error_fn(pred_coords, true_coords, pred_frames, true_frames)
+    alignment_errors = error_fn(pred_coords, pred_coords, pred_frames, pred_frames)
 
     assert alignment_errors.shape == (2, 100)
+    assert (alignment_errors.mean(-1) < 1e-3).all()
 
 def test_centre_random_augmentation():
     coords = torch.randn(2, 100, 3)
 
     augmentation_fn = CentreRandomAugmentation()
     augmented_coords = augmentation_fn(coords)
 
@@ -109,15 +149,16 @@
 
 def test_pairformer():
     single = torch.randn(2, 16, 384)
     pairwise = torch.randn(2, 16, 16, 128)
     mask = torch.randint(0, 2, (2, 16)).bool()
 
     pairformer = PairformerStack(
-        depth = 4
+        depth = 4,
+        num_register_tokens = 4,
     )
 
     single_out, pairwise_out = pairformer(
         single_repr = single,
         pairwise_repr = pairwise,
         mask = mask
     )
@@ -128,35 +169,38 @@
 def test_msa_module():
 
     single = torch.randn(2, 16, 384)
     pairwise = torch.randn(2, 16, 16, 128)
     msa = torch.randn(2, 7, 16, 64)
     mask = torch.randint(0, 2, (2, 16)).bool()
 
-    msa_module = MSAModule()
+    msa_module = MSAModule(
+        max_num_msa = 3 # will randomly select 3 out of the MSAs, accounting for mask, using sample without replacement
+    )
 
     pairwise_out = msa_module(
         msa = msa,
         single_repr = single,
         pairwise_repr = pairwise,
         mask = mask
     )
 
     assert pairwise.shape == pairwise_out.shape
 
-
-def test_diffusion_transformer():
+@pytest.mark.parametrize('use_linear_attn', (False, True))
+def test_diffusion_transformer(use_linear_attn):
 
     single = torch.randn(2, 16, 384)
     pairwise = torch.randn(2, 16, 16, 128)
     mask = torch.randint(0, 2, (2, 16)).bool()
 
     diffusion_transformer = DiffusionTransformer(
         depth = 2,
-        heads = 16
+        heads = 16,
+        use_linear_attn = use_linear_attn
     )
 
     single_out = diffusion_transformer(
         single,
         single_repr = single,
         pairwise_repr = pairwise,
         mask = mask
@@ -177,15 +221,17 @@
 
     out = attn(atoms, attn_bias = attn_bias)
     assert out.shape == atoms.shape
 
 def test_diffusion_module():
 
     seq_len = 16
-    atom_seq_len = 27 * 16
+
+    residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+    atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
 
     noised_atom_pos = torch.randn(2, atom_seq_len, 3)
     atom_feats = torch.randn(2, atom_seq_len, 128)
     atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
     atom_mask = torch.ones((2, atom_seq_len)).bool()
 
     times = torch.randn(2,)
@@ -198,61 +244,67 @@
 
     diffusion_module = DiffusionModule(
         atoms_per_window = 27,
         dim_pairwise_trunk = 128,
         dim_pairwise_rel_pos_feats = 12,
         atom_encoder_depth = 1,
         atom_decoder_depth = 1,
-        token_transformer_depth = 1
+        token_transformer_depth = 1,
+        token_transformer_kwargs = dict(
+            num_register_tokens = 2
+        )
     )
 
     atom_pos_update = diffusion_module(
         noised_atom_pos,
         times = times,
         atom_feats = atom_feats,
         atompair_feats = atompair_feats,
         atom_mask = atom_mask,
         mask = mask,
         single_trunk_repr = single_trunk_repr,
         single_inputs_repr = single_inputs_repr,
         pairwise_trunk = pairwise_trunk,
-        pairwise_rel_pos_feats = pairwise_rel_pos_feats
+        pairwise_rel_pos_feats = pairwise_rel_pos_feats,
+        residue_atom_lens = residue_atom_lens
     )
 
     assert noised_atom_pos.shape == atom_pos_update.shape
 
     edm = ElucidatedAtomDiffusion(
         diffusion_module,
         num_sample_steps = 2
     )
 
-    loss = edm(
+    edm_return = edm(
         noised_atom_pos,
         atom_feats = atom_feats,
         atompair_feats = atompair_feats,
         atom_mask = atom_mask,
         mask = mask,
         single_trunk_repr = single_trunk_repr,
         single_inputs_repr = single_inputs_repr,
         pairwise_trunk = pairwise_trunk,
         pairwise_rel_pos_feats = pairwise_rel_pos_feats,
+        residue_atom_lens = residue_atom_lens,
         add_bond_loss = True
     )
 
-    assert loss.numel() == 1
+    assert edm_return.loss.numel() == 1
 
     sampled_atom_pos = edm.sample(
         atom_mask = atom_mask,
         atom_feats = atom_feats,
         atompair_feats = atompair_feats,
         mask = mask,
         single_trunk_repr = single_trunk_repr,
         single_inputs_repr = single_inputs_repr,
         pairwise_trunk = pairwise_trunk,
-        pairwise_rel_pos_feats = pairwise_rel_pos_feats
+        pairwise_rel_pos_feats = pairwise_rel_pos_feats,
+        residue_atom_lens = residue_atom_lens
     )
 
     assert sampled_atom_pos.shape == noised_atom_pos.shape
     
 def test_relative_position_encoding():
     additional_residue_feats = torch.randn(8, 100, 10)
 
@@ -301,66 +353,79 @@
         pairwise_repr = pairwise_repr,
         pred_atom_pos = pred_atom_pos,
         mask = mask
     )
 
 def test_input_embedder():
 
-    atom_seq_len = 16 * 27
+    residue_atom_lens = torch.randint(0, 3, (2, 16))
+    atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
     atom_inputs = torch.randn(2, atom_seq_len, 77)
+    atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len, 5)
+
     atom_mask = torch.ones((2, atom_seq_len)).bool()
-    atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-    additional_residue_feats = torch.randn(2, 16, 33)
+    additional_residue_feats = torch.randn(2, 16, 10)
 
     embedder = InputFeatureEmbedder(
         dim_atom_inputs = 77,
-        dim_additional_residue_feats = 33
     )
 
     embedder(
         atom_inputs = atom_inputs,
         atom_mask = atom_mask,
-        atompair_feats = atompair_feats,
+        atompair_inputs = atompair_inputs,
+        residue_atom_lens = residue_atom_lens,
         additional_residue_feats = additional_residue_feats
     )
 
 def test_distogram_head():
     pairwise_repr = torch.randn(2, 16, 16, 128)
 
     distogram_head = DistogramHead(dim_pairwise = 128)
 
     logits = distogram_head(pairwise_repr)
 
-
-def test_alphafold3():
+@pytest.mark.parametrize('window_atompair_inputs', (True, False))
+def test_alphafold3(
+    window_atompair_inputs: bool
+):
     seq_len = 16
-    atom_seq_len = seq_len * 27
+    atoms_per_window = 27
+
+    residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+    atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
+
+    token_bond = torch.randint(0, 2, (2, seq_len, seq_len)).bool()
 
     atom_inputs = torch.randn(2, atom_seq_len, 77)
-    atom_mask = torch.ones((2, atom_seq_len)).bool()
-    atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-    additional_residue_feats = torch.randn(2, seq_len, 33)
+
+    atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len, 5)
+
+    if window_atompair_inputs:
+        atompair_inputs = full_pairwise_repr_to_windowed(atompair_inputs, window_size = atoms_per_window)
+
+    additional_residue_feats = torch.randn(2, seq_len, 10)
 
     template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
     template_mask = torch.ones((2, 2)).bool()
 
     msa = torch.randn(2, 7, seq_len, 64)
+    msa_mask = torch.ones((2, 7)).bool()
 
     atom_pos = torch.randn(2, atom_seq_len, 3)
-    residue_atom_indices = torch.randint(0, 27, (2, seq_len))
+    residue_atom_indices = residue_atom_lens - 1
 
-    distance_labels = torch.randint(0, 38, (2, seq_len, seq_len))
     pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
     pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
     plddt_labels = torch.randint(0, 50, (2, seq_len))
     resolved_labels = torch.randint(0, 2, (2, seq_len))
 
     alphafold3 = Alphafold3(
         dim_atom_inputs = 77,
-        dim_additional_residue_feats = 33,
+        atoms_per_window = atoms_per_window,
         dim_template_feats = 44,
         num_dist_bins = 38,
         confidence_head_kwargs = dict(
             pairformer_depth = 1
         ),
         template_embedder_kwargs = dict(
             pairformer_stack_depth = 1
@@ -374,39 +439,101 @@
         diffusion_module_kwargs = dict(
             atom_encoder_depth = 1,
             token_transformer_depth = 1,
             atom_decoder_depth = 1,
         ),
     )
 
-    loss = alphafold3(
+    loss, breakdown = alphafold3(
         num_recycling_steps = 2,
         atom_inputs = atom_inputs,
-        atom_mask = atom_mask,
-        atompair_feats = atompair_feats,
+        residue_atom_lens = residue_atom_lens,
+        atompair_inputs = atompair_inputs,
         additional_residue_feats = additional_residue_feats,
+        token_bond = token_bond,
         msa = msa,
+        msa_mask = msa_mask,
         templates = template_feats,
         template_mask = template_mask,
         atom_pos = atom_pos,
         residue_atom_indices = residue_atom_indices,
-        distance_labels = distance_labels,
         pae_labels = pae_labels,
         pde_labels = pde_labels,
         plddt_labels = plddt_labels,
-        resolved_labels = resolved_labels
+        resolved_labels = resolved_labels,
+        diffusion_add_smooth_lddt_loss = True,
+        return_loss_breakdown = True
     )
 
     loss.backward()
 
     sampled_atom_pos = alphafold3(
         num_sample_steps = 16,
         atom_inputs = atom_inputs,
-        atom_mask = atom_mask,
-        atompair_feats = atompair_feats,
+        residue_atom_lens = residue_atom_lens,
+        atompair_inputs = atompair_inputs,
         additional_residue_feats = additional_residue_feats,
         msa = msa,
         templates = template_feats,
         template_mask = template_mask,
     )
 
     assert sampled_atom_pos.ndim == 3
+
+def test_alphafold3_without_msa_and_templates():
+    seq_len = 16
+    residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+    atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
+
+    atom_inputs = torch.randn(2, atom_seq_len, 77)
+    atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len, 5)
+    additional_residue_feats = torch.randn(2, seq_len, 10)
+
+    atom_pos = torch.randn(2, atom_seq_len, 3)
+    residue_atom_indices = residue_atom_lens - 1
+
+    distance_labels = torch.randint(0, 38, (2, seq_len, seq_len))
+    pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+    pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+    plddt_labels = torch.randint(0, 50, (2, seq_len))
+    resolved_labels = torch.randint(0, 2, (2, seq_len))
+
+    alphafold3 = Alphafold3(
+        dim_atom_inputs = 77,
+        dim_template_feats = 44,
+        num_dist_bins = 38,
+        confidence_head_kwargs = dict(
+            pairformer_depth = 1
+        ),
+        template_embedder_kwargs = dict(
+            pairformer_stack_depth = 1
+        ),
+        msa_module_kwargs = dict(
+            depth = 1
+        ),
+        pairformer_stack = dict(
+            depth = 2
+        ),
+        diffusion_module_kwargs = dict(
+            atom_encoder_depth = 1,
+            token_transformer_depth = 1,
+            atom_decoder_depth = 1,
+        ),
+    )
+
+    loss, breakdown = alphafold3(
+        num_recycling_steps = 2,
+        atom_inputs = atom_inputs,
+        residue_atom_lens = residue_atom_lens,
+        atompair_inputs = atompair_inputs,
+        additional_residue_feats = additional_residue_feats,
+        atom_pos = atom_pos,
+        residue_atom_indices = residue_atom_indices,
+        distance_labels = distance_labels,
+        pae_labels = pae_labels,
+        pde_labels = pde_labels,
+        plddt_labels = plddt_labels,
+        resolved_labels = resolved_labels,
+        return_loss_breakdown = True
+    )
+
+    loss.backward()
```

### Comparing `alphafold3_pytorch-0.0.9/.gitignore` & `alphafold3_pytorch-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/LICENSE` & `alphafold3_pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.9/README.md` & `alphafold3_pytorch-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,80 @@
-<img src="./alphafold3.png" width="450px"></img>
+<img src="./alphafold3.png" width="500px"></img>
 
-## Alphafold 3 - Pytorch (wip)
+## Alphafold 3 - Pytorch
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
 - <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
 
+- <a href="https://github.com/amorehead">Alex</a> for fixing various issues in the transcribed algorithms
+
+- <a href="https://github.com/gitabtion">Heng</a> for pointing out inconsistencies with the paper and pull requesting the solutions
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
 
 ```python
 import torch
 from alphafold3_pytorch import Alphafold3
 
 alphafold3 = Alphafold3(
     dim_atom_inputs = 77,
-    dim_additional_residue_feats = 33,
     dim_template_feats = 44
 )
 
 # mock inputs
 
 seq_len = 16
-atom_seq_len = seq_len * 27
+residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
 
 atom_inputs = torch.randn(2, atom_seq_len, 77)
-atom_mask = torch.ones((2, atom_seq_len)).bool()
-atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-additional_residue_feats = torch.randn(2, seq_len, 33)
+atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len, 5)
+
+additional_residue_feats = torch.randn(2, seq_len, 10)
 
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
+msa_mask = torch.ones((2, 7)).bool()
 
 # required for training, but omitted on inference
 
 atom_pos = torch.randn(2, atom_seq_len, 3)
-residue_atom_indices = torch.randint(0, 27, (2, seq_len))
+residue_atom_indices = residue_atom_lens - 1 # last atom, as an example
 
 distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
 pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
 pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
 plddt_labels = torch.randint(0, 50, (2, seq_len))
 resolved_labels = torch.randint(0, 2, (2, seq_len))
 
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
-    atom_mask = atom_mask,
-    atompair_feats = atompair_feats,
+    atompair_inputs = atompair_inputs,
+    residue_atom_lens = residue_atom_lens,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
+    msa_mask = msa_mask,
     templates = template_feats,
     template_mask = template_mask,
     atom_pos = atom_pos,
     residue_atom_indices = residue_atom_indices,
     distance_labels = distance_labels,
     pae_labels = pae_labels,
     pde_labels = pde_labels,
@@ -80,23 +86,24 @@
 
 # after much training ...
 
 sampled_atom_pos = alphafold3(
     num_recycling_steps = 4,
     num_sample_steps = 16,
     atom_inputs = atom_inputs,
-    atom_mask = atom_mask,
-    atompair_feats = atompair_feats,
+    atompair_inputs = atompair_inputs,
+    residue_atom_lens = residue_atom_lens,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
+    msa_mask = msa_mask,
     templates = template_feats,
     template_mask = template_mask
 )
 
-sampled_atom_pos.shape # (2, 16 * 27, 3)
+sampled_atom_pos.shape # (2, <atom_seqlen>, 3)
 ```
 
 ## Contributing
 
 At the project root, run
 
 ```bash
@@ -105,14 +112,27 @@
 
 Then, add your module to `alphafold3_pytorch/alphafold3.py`, add your tests to `tests/test_af3.py`, and submit a pull request. You can run the tests locally with
 
 ```bash
 $ pytest tests/
 ```
 
+## Docker
+
+### Build Docker Container
+```bash
+docker build -t af3 .
+```
+
+### Run Container
+```bash
+## With GPUs
+docker run  --gpus all -it af3
+```
+
 ## Citations
 
 ```bibtex
 @article{Abramson2024-fj,
   title    = "Accurate structure prediction of biomolecular interactions with
               {AlphaFold} 3",
   author   = "Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans,
@@ -132,7 +152,27 @@
               {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet
               and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
   journal  = "Nature",
   month    = "May",
   year     =  2024
 }
 ```
+
+```bibtex
+@inproceedings{Darcet2023VisionTN,
+    title   = {Vision Transformers Need Registers},
+    author  = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal and Piotr Bojanowski},
+    year    = {2023},
+    url     = {https://api.semanticscholar.org/CorpusID:263134283}
+}
+```
+
+```bibtex
+@article{Arora2024SimpleLA,
+    title   = {Simple linear attention language models balance the recall-throughput tradeoff},
+    author  = {Simran Arora and Sabri Eyuboglu and Michael Zhang and Aman Timalsina and Silas Alberti and Dylan Zinsley and James Zou and Atri Rudra and Christopher R'e},
+    journal = {ArXiv},
+    year    = {2024},
+    volume  = {abs/2402.18668},
+    url     = {https://api.semanticscholar.org/CorpusID:268063190}
+}
+```
```

#### html2text {}

```diff
@@ -1,51 +1,66 @@
-[./alphafold3.png]## Alphafold 3 - Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3
-in Pytorch Getting a fair number of emails. You can chat with me about this
-work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional
-Encoding and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid
-Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random
-Augmentation modules! ## Install ```bash $ pip install alphafold3-pytorch ```
-## Usage ```python import torch from alphafold3_pytorch import Alphafold3
-alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_additional_residue_feats =
-33, dim_template_feats = 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len
-* 27 atom_inputs = torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2,
-atom_seq_len)).bool() atompair_feats = torch.randn(2, atom_seq_len,
-atom_seq_len, 16) additional_residue_feats = torch.randn(2, seq_len, 33)
+[./alphafold3.png]## Alphafold 3 - Pytorch Implementation of _A_l_p_h_a_f_o_l_d_ _3 in
+Pytorch Getting a fair number of emails. You can chat with me about this work
+_h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional Encoding
+and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid Align,
+Express Coordinates In Frame, Compute Alignment Error, and Centre Random
+Augmentation modules! - _A_l_e_x for fixing various issues in the transcribed
+algorithms - _H_e_n_g for pointing out inconsistencies with the paper and pull
+requesting the solutions ## Install ```bash $ pip install alphafold3-pytorch
+``` ## Usage ```python import torch from alphafold3_pytorch import Alphafold3
+alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock
+inputs seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+atom_seq_len = residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn
+(2, atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len,
+atom_seq_len, 5) additional_residue_feats = torch.randn(2, seq_len, 10)
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
-torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) # required for
-training, but omitted on inference atom_pos = torch.randn(2, atom_seq_len, 3)
-residue_atom_indices = torch.randint(0, 27, (2, seq_len)) distance_labels =
+torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) msa_mask =
+torch.ones((2, 7)).bool() # required for training, but omitted on inference
+atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
+residue_atom_lens - 1 # last atom, as an example distance_labels =
 torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
 (2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
 plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
 torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
-( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask = atom_mask,
-atompair_feats = atompair_feats, additional_residue_feats =
-additional_residue_feats, msa = msa, templates = template_feats, template_mask
-= template_mask, atom_pos = atom_pos, residue_atom_indices =
-residue_atom_indices, distance_labels = distance_labels, pae_labels =
-pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
-resolved_labels = resolved_labels ) loss.backward() # after much training ...
-sampled_atom_pos = alphafold3( num_recycling_steps = 4, num_sample_steps = 16,
-atom_inputs = atom_inputs, atom_mask = atom_mask, atompair_feats =
-atompair_feats, additional_residue_feats = additional_residue_feats, msa = msa,
-templates = template_feats, template_mask = template_mask )
-sampled_atom_pos.shape # (2, 16 * 27, 3) ``` ## Contributing At the project
-root, run ```bash $ sh ./contribute.sh ``` Then, add your module to
-`alphafold3_pytorch/alphafold3.py`, add your tests to `tests/test_af3.py`, and
-submit a pull request. You can run the tests locally with ```bash $ pytest
-tests/ ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
-structure prediction of biomolecular interactions with {AlphaFold} 3", author =
-"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
-Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
-Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
-David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
-Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
-Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
-and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
-Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
-Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
-Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
-Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
-D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
-Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
-journal = "Nature", month = "May", year = 2024 } ```
+( num_recycling_steps = 2, atom_inputs = atom_inputs, atompair_inputs =
+atompair_inputs, residue_atom_lens = residue_atom_lens,
+additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
+msa_mask, templates = template_feats, template_mask = template_mask, atom_pos =
+atom_pos, residue_atom_indices = residue_atom_indices, distance_labels =
+distance_labels, pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels
+= plddt_labels, resolved_labels = resolved_labels ) loss.backward() # after
+much training ... sampled_atom_pos = alphafold3( num_recycling_steps = 4,
+num_sample_steps = 16, atom_inputs = atom_inputs, atompair_inputs =
+atompair_inputs, residue_atom_lens = residue_atom_lens,
+additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
+msa_mask, templates = template_feats, template_mask = template_mask )
+sampled_atom_pos.shape # (2, , 3) ``` ## Contributing At the project root, run
+```bash $ sh ./contribute.sh ``` Then, add your module to `alphafold3_pytorch/
+alphafold3.py`, add your tests to `tests/test_af3.py`, and submit a pull
+request. You can run the tests locally with ```bash $ pytest tests/ ``` ##
+Docker ### Build Docker Container ```bash docker build -t af3 . ``` ### Run
+Container ```bash ## With GPUs docker run --gpus all -it af3 ``` ## Citations
+```bibtex @article{Abramson2024-fj, title = "Accurate structure prediction of
+biomolecular interactions with {AlphaFold} 3", author = "Abramson, Josh and
+Adler, Jonas and Dunger, Jack and Evans, Richard and Green, Tim and Pritzel,
+Alexander and Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and
+Bambrick, Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-
+Chun and O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and
+Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and
+Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex and Cherepanov,
+Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and
+Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and
+Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and
+Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok
+and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski,
+Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and
+Jaderberg, Max and Hassabis, Demis and Jumper, John M", journal = "Nature",
+month = "May", year = 2024 } ``` ```bibtex @inproceedings{Darcet2023VisionTN,
+title = {Vision Transformers Need Registers}, author = {Timoth'ee Darcet and
+Maxime Oquab and Julien Mairal and Piotr Bojanowski}, year = {2023}, url =
+{https://api.semanticscholar.org/CorpusID:263134283} } ``` ```bibtex @article
+{Arora2024SimpleLA, title = {Simple linear attention language models balance
+the recall-throughput tradeoff}, author = {Simran Arora and Sabri Eyuboglu and
+Michael Zhang and Aman Timalsina and Silas Alberti and Dylan Zinsley and James
+Zou and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year = {2024},
+volume = {abs/2402.18668}, url = {https://api.semanticscholar.org/CorpusID:
+268063190} } ```
```

### Comparing `alphafold3_pytorch-0.0.9/pyproject.toml` & `alphafold3_pytorch-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.0.9"
+version = "0.1.0"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
@@ -22,16 +22,19 @@
     'Programming Language :: Python :: 3.8',
 ]
 
 dependencies = [
     "beartype",
     "einops>=0.8.0",
     "einx>=0.2.2",
+    "ema-pytorch>=0.4.8",
     "environs",
     "jaxtyping>=0.2.28",
+    "lightning>=2.2.5",
+    "taylor-series-linear-attention>=0.1.9",
     "torch>=2.1",
     "tqdm",
 ]
 
 [project.urls]
 Homepage = "https://pypi.org/project/alphafold3-pytorch/"
 Repository = "https://github.com/lucidrains/alphafold3-pytorch"
```

### Comparing `alphafold3_pytorch-0.0.9/PKG-INFO` & `alphafold3_pytorch-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.0.9
+Version: 0.1.0
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -33,90 +33,99 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Requires-Dist: beartype
 Requires-Dist: einops>=0.8.0
 Requires-Dist: einx>=0.2.2
+Requires-Dist: ema-pytorch>=0.4.8
 Requires-Dist: environs
 Requires-Dist: jaxtyping>=0.2.28
+Requires-Dist: lightning>=2.2.5
+Requires-Dist: taylor-series-linear-attention>=0.1.9
 Requires-Dist: torch>=2.1
 Requires-Dist: tqdm
 Provides-Extra: examples
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-<img src="./alphafold3.png" width="450px"></img>
+<img src="./alphafold3.png" width="500px"></img>
 
-## Alphafold 3 - Pytorch (wip)
+## Alphafold 3 - Pytorch
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
 - <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
 
+- <a href="https://github.com/amorehead">Alex</a> for fixing various issues in the transcribed algorithms
+
+- <a href="https://github.com/gitabtion">Heng</a> for pointing out inconsistencies with the paper and pull requesting the solutions
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
 
 ```python
 import torch
 from alphafold3_pytorch import Alphafold3
 
 alphafold3 = Alphafold3(
     dim_atom_inputs = 77,
-    dim_additional_residue_feats = 33,
     dim_template_feats = 44
 )
 
 # mock inputs
 
 seq_len = 16
-atom_seq_len = seq_len * 27
+residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+atom_seq_len = residue_atom_lens.sum(dim = -1).amax()
 
 atom_inputs = torch.randn(2, atom_seq_len, 77)
-atom_mask = torch.ones((2, atom_seq_len)).bool()
-atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-additional_residue_feats = torch.randn(2, seq_len, 33)
+atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len, 5)
+
+additional_residue_feats = torch.randn(2, seq_len, 10)
 
 template_feats = torch.randn(2, 2, seq_len, seq_len, 44)
 template_mask = torch.ones((2, 2)).bool()
 
 msa = torch.randn(2, 7, seq_len, 64)
+msa_mask = torch.ones((2, 7)).bool()
 
 # required for training, but omitted on inference
 
 atom_pos = torch.randn(2, atom_seq_len, 3)
-residue_atom_indices = torch.randint(0, 27, (2, seq_len))
+residue_atom_indices = residue_atom_lens - 1 # last atom, as an example
 
 distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
 pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
 pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
 plddt_labels = torch.randint(0, 50, (2, seq_len))
 resolved_labels = torch.randint(0, 2, (2, seq_len))
 
 # train
 
 loss = alphafold3(
     num_recycling_steps = 2,
     atom_inputs = atom_inputs,
-    atom_mask = atom_mask,
-    atompair_feats = atompair_feats,
+    atompair_inputs = atompair_inputs,
+    residue_atom_lens = residue_atom_lens,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
+    msa_mask = msa_mask,
     templates = template_feats,
     template_mask = template_mask,
     atom_pos = atom_pos,
     residue_atom_indices = residue_atom_indices,
     distance_labels = distance_labels,
     pae_labels = pae_labels,
     pde_labels = pde_labels,
@@ -128,23 +137,24 @@
 
 # after much training ...
 
 sampled_atom_pos = alphafold3(
     num_recycling_steps = 4,
     num_sample_steps = 16,
     atom_inputs = atom_inputs,
-    atom_mask = atom_mask,
-    atompair_feats = atompair_feats,
+    atompair_inputs = atompair_inputs,
+    residue_atom_lens = residue_atom_lens,
     additional_residue_feats = additional_residue_feats,
     msa = msa,
+    msa_mask = msa_mask,
     templates = template_feats,
     template_mask = template_mask
 )
 
-sampled_atom_pos.shape # (2, 16 * 27, 3)
+sampled_atom_pos.shape # (2, <atom_seqlen>, 3)
 ```
 
 ## Contributing
 
 At the project root, run
 
 ```bash
@@ -153,14 +163,27 @@
 
 Then, add your module to `alphafold3_pytorch/alphafold3.py`, add your tests to `tests/test_af3.py`, and submit a pull request. You can run the tests locally with
 
 ```bash
 $ pytest tests/
 ```
 
+## Docker
+
+### Build Docker Container
+```bash
+docker build -t af3 .
+```
+
+### Run Container
+```bash
+## With GPUs
+docker run  --gpus all -it af3
+```
+
 ## Citations
 
 ```bibtex
 @article{Abramson2024-fj,
   title    = "Accurate structure prediction of biomolecular interactions with
               {AlphaFold} 3",
   author   = "Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans,
@@ -180,7 +203,27 @@
               {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet
               and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
   journal  = "Nature",
   month    = "May",
   year     =  2024
 }
 ```
+
+```bibtex
+@inproceedings{Darcet2023VisionTN,
+    title   = {Vision Transformers Need Registers},
+    author  = {Timoth'ee Darcet and Maxime Oquab and Julien Mairal and Piotr Bojanowski},
+    year    = {2023},
+    url     = {https://api.semanticscholar.org/CorpusID:263134283}
+}
+```
+
+```bibtex
+@article{Arora2024SimpleLA,
+    title   = {Simple linear attention language models balance the recall-throughput tradeoff},
+    author  = {Simran Arora and Sabri Eyuboglu and Michael Zhang and Aman Timalsina and Silas Alberti and Dylan Zinsley and James Zou and Atri Rudra and Christopher R'e},
+    journal = {ArXiv},
+    year    = {2024},
+    volume  = {abs/2402.18668},
+    url     = {https://api.semanticscholar.org/CorpusID:268063190}
+}
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.9 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.0 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -18,61 +18,78 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. License-File: LICENSE Keywords: artificial
 intelligence,deep learning,protein structure prediction Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8 Requires-Dist: beartype Requires-Dist:
-einops>=0.8.0 Requires-Dist: einx>=0.2.2 Requires-Dist: environs Requires-Dist:
-jaxtyping>=0.2.28 Requires-Dist: torch>=2.1 Requires-Dist: tqdm Provides-Extra:
-examples Provides-Extra: test Requires-Dist: pytest; extra == 'test'
-Description-Content-Type: text/markdown [./alphafold3.png]## Alphafold 3 -
-Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3 in Pytorch Getting a fair number of
-emails. You can chat with me about this work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for
-contributing the Relative Positional Encoding and the Smooth LDDT Loss! -
-_F_e_l_i_p_e for contributing Weighted Rigid Align, Express Coordinates In Frame,
-Compute Alignment Error, and Centre Random Augmentation modules! ## Install
-```bash $ pip install alphafold3-pytorch ``` ## Usage ```python import torch
-from alphafold3_pytorch import Alphafold3 alphafold3 = Alphafold3
-( dim_atom_inputs = 77, dim_additional_residue_feats = 33, dim_template_feats =
-44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len * 27 atom_inputs =
-torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2, atom_seq_len)).bool
-() atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-additional_residue_feats = torch.randn(2, seq_len, 33) template_feats =
-torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
-() msa = torch.randn(2, 7, seq_len, 64) # required for training, but omitted on
-inference atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
-torch.randint(0, 27, (2, seq_len)) distance_labels = torch.randint(0, 37, (2,
-seq_len, seq_len)) pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
-pde_labels = torch.randint(0, 64, (2, seq_len, seq_len)) plddt_labels =
-torch.randint(0, 50, (2, seq_len)) resolved_labels = torch.randint(0, 2, (2,
-seq_len)) # train loss = alphafold3( num_recycling_steps = 2, atom_inputs =
-atom_inputs, atom_mask = atom_mask, atompair_feats = atompair_feats,
-additional_residue_feats = additional_residue_feats, msa = msa, templates =
-template_feats, template_mask = template_mask, atom_pos = atom_pos,
-residue_atom_indices = residue_atom_indices, distance_labels = distance_labels,
-pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
-resolved_labels = resolved_labels ) loss.backward() # after much training ...
-sampled_atom_pos = alphafold3( num_recycling_steps = 4, num_sample_steps = 16,
-atom_inputs = atom_inputs, atom_mask = atom_mask, atompair_feats =
-atompair_feats, additional_residue_feats = additional_residue_feats, msa = msa,
-templates = template_feats, template_mask = template_mask )
-sampled_atom_pos.shape # (2, 16 * 27, 3) ``` ## Contributing At the project
-root, run ```bash $ sh ./contribute.sh ``` Then, add your module to
-`alphafold3_pytorch/alphafold3.py`, add your tests to `tests/test_af3.py`, and
-submit a pull request. You can run the tests locally with ```bash $ pytest
-tests/ ``` ## Citations ```bibtex @article{Abramson2024-fj, title = "Accurate
-structure prediction of biomolecular interactions with {AlphaFold} 3", author =
-"Abramson, Josh and Adler, Jonas and Dunger, Jack and Evans, Richard and Green,
-Tim and Pritzel, Alexander and Ronneberger, Olaf and Willmore, Lindsay and
-Ballard, Andrew J and Bambrick, Joshua and Bodenstein, Sebastian W and Evans,
-David A and Hung, Chia-Chun and O'Neill, Michael and Reiman, David and
-Tunyasuvunakool, Kathryn and Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and
-Arvaniti, Eirini and Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex
-and Cherepanov, Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and
-Cowie, Andrew and Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and
-Jain, Rishub and Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and
-Potapenko, Anna and Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and
-Thillaisundaram, Ashok and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen
-D and Zielinski, Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and
-Kohli, Pushmeet and Jaderberg, Max and Hassabis, Demis and Jumper, John M",
-journal = "Nature", month = "May", year = 2024 } ```
+einops>=0.8.0 Requires-Dist: einx>=0.2.2 Requires-Dist: ema-pytorch>=0.4.8
+Requires-Dist: environs Requires-Dist: jaxtyping>=0.2.28 Requires-Dist:
+lightning>=2.2.5 Requires-Dist: taylor-series-linear-attention>=0.1.9 Requires-
+Dist: torch>=2.1 Requires-Dist: tqdm Provides-Extra: examples Provides-Extra:
+test Requires-Dist: pytest; extra == 'test' Description-Content-Type: text/
+markdown [./alphafold3.png]## Alphafold 3 - Pytorch Implementation of _A_l_p_h_a_f_o_l_d
+_3 in Pytorch Getting a fair number of emails. You can chat with me about this
+work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional
+Encoding and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid
+Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random
+Augmentation modules! - _A_l_e_x for fixing various issues in the transcribed
+algorithms - _H_e_n_g for pointing out inconsistencies with the paper and pull
+requesting the solutions ## Install ```bash $ pip install alphafold3-pytorch
+``` ## Usage ```python import torch from alphafold3_pytorch import Alphafold3
+alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock
+inputs seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len))
+atom_seq_len = residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn
+(2, atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len,
+atom_seq_len, 5) additional_residue_feats = torch.randn(2, seq_len, 10)
+template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
+torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) msa_mask =
+torch.ones((2, 7)).bool() # required for training, but omitted on inference
+atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
+residue_atom_lens - 1 # last atom, as an example distance_labels =
+torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
+(2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
+torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
+( num_recycling_steps = 2, atom_inputs = atom_inputs, atompair_inputs =
+atompair_inputs, residue_atom_lens = residue_atom_lens,
+additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
+msa_mask, templates = template_feats, template_mask = template_mask, atom_pos =
+atom_pos, residue_atom_indices = residue_atom_indices, distance_labels =
+distance_labels, pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels
+= plddt_labels, resolved_labels = resolved_labels ) loss.backward() # after
+much training ... sampled_atom_pos = alphafold3( num_recycling_steps = 4,
+num_sample_steps = 16, atom_inputs = atom_inputs, atompair_inputs =
+atompair_inputs, residue_atom_lens = residue_atom_lens,
+additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
+msa_mask, templates = template_feats, template_mask = template_mask )
+sampled_atom_pos.shape # (2, , 3) ``` ## Contributing At the project root, run
+```bash $ sh ./contribute.sh ``` Then, add your module to `alphafold3_pytorch/
+alphafold3.py`, add your tests to `tests/test_af3.py`, and submit a pull
+request. You can run the tests locally with ```bash $ pytest tests/ ``` ##
+Docker ### Build Docker Container ```bash docker build -t af3 . ``` ### Run
+Container ```bash ## With GPUs docker run --gpus all -it af3 ``` ## Citations
+```bibtex @article{Abramson2024-fj, title = "Accurate structure prediction of
+biomolecular interactions with {AlphaFold} 3", author = "Abramson, Josh and
+Adler, Jonas and Dunger, Jack and Evans, Richard and Green, Tim and Pritzel,
+Alexander and Ronneberger, Olaf and Willmore, Lindsay and Ballard, Andrew J and
+Bambrick, Joshua and Bodenstein, Sebastian W and Evans, David A and Hung, Chia-
+Chun and O'Neill, Michael and Reiman, David and Tunyasuvunakool, Kathryn and
+Wu, Zachary and {\v Z}emgulyt{\.e}, Akvil{\.e} and Arvaniti, Eirini and
+Beattie, Charles and Bertolli, Ottavia and Bridgland, Alex and Cherepanov,
+Alexey and Congreve, Miles and Cowen-Rivers, Alexander I and Cowie, Andrew and
+Figurnov, Michael and Fuchs, Fabian B and Gladman, Hannah and Jain, Rishub and
+Khan, Yousuf A and Low, Caroline M R and Perlin, Kuba and Potapenko, Anna and
+Savy, Pascal and Singh, Sukhdeep and Stecula, Adrian and Thillaisundaram, Ashok
+and Tong, Catherine and Yakneen, Sergei and Zhong, Ellen D and Zielinski,
+Michal and {\v Z}{\'\i}dek, Augustin and Bapst, Victor and Kohli, Pushmeet and
+Jaderberg, Max and Hassabis, Demis and Jumper, John M", journal = "Nature",
+month = "May", year = 2024 } ``` ```bibtex @inproceedings{Darcet2023VisionTN,
+title = {Vision Transformers Need Registers}, author = {Timoth'ee Darcet and
+Maxime Oquab and Julien Mairal and Piotr Bojanowski}, year = {2023}, url =
+{https://api.semanticscholar.org/CorpusID:263134283} } ``` ```bibtex @article
+{Arora2024SimpleLA, title = {Simple linear attention language models balance
+the recall-throughput tradeoff}, author = {Simran Arora and Sabri Eyuboglu and
+Michael Zhang and Aman Timalsina and Silas Alberti and Dylan Zinsley and James
+Zou and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year = {2024},
+volume = {abs/2402.18668}, url = {https://api.semanticscholar.org/CorpusID:
+268063190} } ```
```

