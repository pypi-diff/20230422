# Comparing `tmp/high_order_layers_torch-1.3.2.tar.gz` & `tmp/high_order_layers_torch-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "high_order_layers_torch-1.3.2.tar", max compression
+gzip compressed data, was "high_order_layers_torch-1.3.3.tar", max compression
```

## Comparing `high_order_layers_torch-1.3.2.tar` & `high_order_layers_torch-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-1.3.2/LICENSE
--rw-r--r--   0        0        0    12291 2023-02-19 15:47:30.961232 high_order_layers_torch-1.3.2/README.md
--rw-r--r--   0        0        0    14898 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.2/high_order_layers_torch/Basis.py
--rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.2/high_order_layers_torch/FunctionalConvolution.py
--rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.2/high_order_layers_torch/FunctionalConvolutionTranspose.py
--rw-r--r--   0        0        0     3688 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.2/high_order_layers_torch/LagrangePolynomial.py
--rw-r--r--   0        0        0    22480 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.2/high_order_layers_torch/PolynomialLayers.py
--rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.2/high_order_layers_torch/ProductLayer.py
--rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-1.3.2/high_order_layers_torch/__init__.py
--rw-r--r--   0        0        0    21912 2023-03-27 02:58:09.788164 high_order_layers_torch-1.3.2/high_order_layers_torch/attentions.py
--rw-r--r--   0        0        0     6776 2023-02-24 04:06:47.654887 high_order_layers_torch-1.3.2/high_order_layers_torch/layers.py
--rw-r--r--   0        0        0     7239 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.2/high_order_layers_torch/modules.py
--rw-r--r--   0        0        0    33107 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.2/high_order_layers_torch/networks.py
--rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.2/high_order_layers_torch/positional_embeddings.py
--rw-r--r--   0        0        0     3280 2023-02-24 04:49:25.106704 high_order_layers_torch-1.3.2/high_order_layers_torch/utils.py
--rw-r--r--   0        0        0      731 2023-03-29 03:01:25.149905 high_order_layers_torch-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.2/setup.py
--rw-r--r--   0        0        0    13053 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-12-01 04:11:06.990013 high_order_layers_torch-1.3.3/LICENSE
+-rw-r--r--   0        0        0    10636 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/README.md
+-rw-r--r--   0        0        0    14898 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/Basis.py
+-rw-r--r--   0        0        0    17551 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolution.py
+-rw-r--r--   0        0        0     5189 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolutionTranspose.py
+-rw-r--r--   0        0        0     3688 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/LagrangePolynomial.py
+-rw-r--r--   0        0        0    22480 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.3/high_order_layers_torch/PolynomialLayers.py
+-rw-r--r--   0        0        0     1656 2022-12-03 04:01:25.774253 high_order_layers_torch-1.3.3/high_order_layers_torch/ProductLayer.py
+-rw-r--r--   0        0        0        0 2020-12-01 04:11:06.994012 high_order_layers_torch-1.3.3/high_order_layers_torch/__init__.py
+-rw-r--r--   0        0        0    22990 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/high_order_layers_torch/attentions.py
+-rw-r--r--   0        0        0     8098 2023-04-22 03:25:58.265287 high_order_layers_torch-1.3.3/high_order_layers_torch/layers.py
+-rw-r--r--   0        0        0     7239 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.3/high_order_layers_torch/modules.py
+-rw-r--r--   0        0        0    33107 2023-03-27 02:51:35.852043 high_order_layers_torch-1.3.3/high_order_layers_torch/networks.py
+-rw-r--r--   0        0        0     2488 2022-12-03 04:01:25.778253 high_order_layers_torch-1.3.3/high_order_layers_torch/positional_embeddings.py
+-rw-r--r--   0        0        0     3282 2023-04-21 03:06:49.131515 high_order_layers_torch-1.3.3/high_order_layers_torch/utils.py
+-rw-r--r--   0        0        0      731 2023-04-22 03:28:57.406819 high_order_layers_torch-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.3/setup.py
+-rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 high_order_layers_torch-1.3.3/PKG-INFO
```

### Comparing `high_order_layers_torch-1.3.2/LICENSE` & `high_order_layers_torch-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/README.md` & `high_order_layers_torch-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: high-order-layers-torch
+Version: 1.3.3
+Summary: High order layers in pytorch
+License: MIT
+Author: jloverich
+Author-email: john.loverich@gmail.com
+Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: hydra-core (>=1.2.0,<2.0.0)
+Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: torch-optimizer (>=0.3.0,<0.4.0)
+Requires-Dist: torchmetrics (>=0.10.2,<0.11.0)
+Requires-Dist: torchvision (>=0.15.1,<0.16.0)
+Description-Content-Type: text/markdown
+
 ![Build Status](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)
 
 # Piecewise Polynomial and Fourier Layers in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
 Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant.  Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models.  This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.
@@ -12,27 +33,17 @@
 
 In the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.
 
 <img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">
 
 ## Why
 
-Using higher order polynomial representations might allow networks with much fewer total weights. In physics, higher order methods
-can be much more efficient. Spectral and discontinuous galerkin methods are examples of this.  Note that a standard neural network with relu activations is piecewise linear.  Here there are no bias weights and the "non-linearity" is in the synapse.  Also, I've included discontinuous
-layers, in physics there are many problems that are discontinuous (most non-linear hyperbolic conservation laws form discontinuities) in this case the method becomes a subgradient descent.
-
-In addition, it's well known that the dendrites are also computational units in neurons, for example [Dendritic action potentials and computation in human layer 2/3 cortical neurons](https://science.sciencemag.org/content/367/6473/83) and this is a simple way to add more computational power into the artificial neural network model. In addition it's been shown that a single pyramidal has the same computational capacity as a 5 to 8 layer convolutional NN, [Single cortical neurons as deep artificial neural networks](https://www.sciencedirect.com/science/article/abs/pii/S0896627321005018?dgcid=author)
-
+Using higher order polynomial representations might allow networks with much fewer total weights.
 
 
-## Speed
-Solving with relu layers is faster, however, sparsity may mean that there is a speed advantage in using the piecewise polynomial approach
-when there are many segments.  There do seem to be situations where the piecewise polynomial approach is significantly better than
-standard relu layers.  Also, combining these layers with standard relu inputs, or using piecewise polynomial layer as inputs especially for implicit representation type problems (or as "positional embeddings") and in natural language problems seems to be useful.
-
 ## Fully Connected Layer Types
 All polynomials are Lagrange polynomials with Chebyshev interpolation points.
 
 A helper function is provided in selecting and switching between these layers
 
 ```python
 from high_order_layers_torch.layers import *
@@ -242,7 +253,8 @@
   title = {High Order Layers Torch},
   year = {2020},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/jloveric/high-order-layers-torch}},
 }
 ```
+
```

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/Basis.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/Basis.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/FunctionalConvolution.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolution.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/FunctionalConvolutionTranspose.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/FunctionalConvolutionTranspose.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/LagrangePolynomial.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/LagrangePolynomial.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/PolynomialLayers.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/PolynomialLayers.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/ProductLayer.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/ProductLayer.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/attentions.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/attentions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,70 +21,81 @@
         - **key** (batch, k_len, d_model): tensor containing projection vector for encoder.
         - **value** (batch, v_len, d_model): tensor containing features of the encoded input sequence.
         - **mask** (-): tensor containing indices to be masked
     Returns: context, attn
         - **context**: tensor containing the context vector from attention mechanism.
         - **attn**: tensor containing the attention (alignment) from the encoder outputs.
     """
+
     def __init__(self, dim: int):
         super(ScaledDotProductAttention, self).__init__()
         self.sqrt_dim = np.sqrt(dim)
 
-    def forward(self, query: Tensor, key: Tensor, value: Tensor, mask: Optional[Tensor] = None) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self, query: Tensor, key: Tensor, value: Tensor, mask: Optional[Tensor] = None
+    ) -> Tuple[Tensor, Tensor]:
         score = torch.bmm(query, key.transpose(1, 2)) / self.sqrt_dim
 
         if mask is not None:
-            score.masked_fill_(mask.view(score.size()), -float('Inf'))
+            score.masked_fill_(mask.view(score.size()), -float("Inf"))
 
         attn = F.softmax(score, -1)
         context = torch.bmm(attn, value)
         return context, attn
 
 
 class DotProductAttention(nn.Module):
     """
     Compute the dot products of the query with all values and apply a softmax function to obtain the weights on the values
     """
+
     def __init__(self, hidden_dim):
         super(DotProductAttention, self).__init__()
 
     def forward(self, query: Tensor, value: Tensor) -> Tuple[Tensor, Tensor]:
         batch_size, hidden_dim, input_size = query.size(0), query.size(2), value.size(1)
 
         score = torch.bmm(query, value.transpose(1, 2))
-        attn = F.softmax(score.view(-1, input_size), dim=1).view(batch_size, -1, input_size)
+        attn = F.softmax(score.view(-1, input_size), dim=1).view(
+            batch_size, -1, input_size
+        )
         context = torch.bmm(attn, value)
 
         return context, attn
 
 
 class AdditiveAttention(nn.Module):
     """
-     Applies a additive attention (bahdanau) mechanism on the output features from the decoder.
-     Additive attention proposed in "Neural Machine Translation by Jointly Learning to Align and Translate" paper.
-     Args:
-         hidden_dim (int): dimesion of hidden state vector
-     Inputs: query, value
-         - **query** (batch_size, q_len, hidden_dim): tensor containing the output features from the decoder.
-         - **value** (batch_size, v_len, hidden_dim): tensor containing features of the encoded input sequence.
-     Returns: context, attn
-         - **context**: tensor containing the context vector from attention mechanism.
-         - **attn**: tensor containing the alignment from the encoder outputs.
-     Reference:
-         - **Neural Machine Translation by Jointly Learning to Align and Translate**: https://arxiv.org/abs/1409.0473
+    Applies a additive attention (bahdanau) mechanism on the output features from the decoder.
+    Additive attention proposed in "Neural Machine Translation by Jointly Learning to Align and Translate" paper.
+    Args:
+        hidden_dim (int): dimesion of hidden state vector
+    Inputs: query, value
+        - **query** (batch_size, q_len, hidden_dim): tensor containing the output features from the decoder.
+        - **value** (batch_size, v_len, hidden_dim): tensor containing features of the encoded input sequence.
+    Returns: context, attn
+        - **context**: tensor containing the context vector from attention mechanism.
+        - **attn**: tensor containing the alignment from the encoder outputs.
+    Reference:
+        - **Neural Machine Translation by Jointly Learning to Align and Translate**: https://arxiv.org/abs/1409.0473
     """
+
     def __init__(self, hidden_dim: int) -> None:
         super(AdditiveAttention, self).__init__()
         self.query_proj = nn.Linear(hidden_dim, hidden_dim, bias=False)
         self.key_proj = nn.Linear(hidden_dim, hidden_dim, bias=False)
         self.bias = nn.Parameter(torch.rand(hidden_dim).uniform_(-0.1, 0.1))
         self.score_proj = nn.Linear(hidden_dim, 1)
 
-    def forward(self, query: Tensor, key: Tensor, value: Tensor) -> Tuple[Tensor, Tensor]:
-        score = self.score_proj(torch.tanh(self.key_proj(key) + self.query_proj(query) + self.bias)).squeeze(-1)
+    def forward(
+        self, query: Tensor, key: Tensor, value: Tensor
+    ) -> Tuple[Tensor, Tensor]:
+        score = self.score_proj(
+            torch.tanh(self.key_proj(key) + self.query_proj(query) + self.bias)
+        ).squeeze(-1)
         attn = F.softmax(score, dim=-1)
         context = torch.bmm(attn.unsqueeze(1), value)
         return context, attn
 
 
 class LocationAwareAttention(nn.Module):
     """
@@ -102,46 +113,59 @@
     Returns: output, attn
         - **output** (batch, output_len, dimensions): tensor containing the feature from encoder outputs
         - **attn** (batch * num_heads, v_len): tensor containing the attention (alignment) from the encoder outputs.
     Reference:
         - **Attention-Based Models for Speech Recognition**: https://arxiv.org/abs/1506.07503
         - **ClovaCall**: https://github.com/clovaai/ClovaCall/blob/master/las.pytorch/models/attention.py
     """
+
     def __init__(self, hidden_dim: int, smoothing: bool = True) -> None:
         super(LocationAwareAttention, self).__init__()
         self.hidden_dim = hidden_dim
-        self.conv1d = nn.Conv1d(in_channels=1, out_channels=hidden_dim, kernel_size=3, padding=1)
+        self.conv1d = nn.Conv1d(
+            in_channels=1, out_channels=hidden_dim, kernel_size=3, padding=1
+        )
         self.query_proj = nn.Linear(hidden_dim, hidden_dim, bias=False)
         self.value_proj = nn.Linear(hidden_dim, hidden_dim, bias=False)
         self.score_proj = nn.Linear(hidden_dim, 1, bias=True)
         self.bias = nn.Parameter(torch.rand(hidden_dim).uniform_(-0.1, 0.1))
         self.smoothing = smoothing
 
-    def forward(self, query: Tensor, value: Tensor, last_attn: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self, query: Tensor, value: Tensor, last_attn: Tensor
+    ) -> Tuple[Tensor, Tensor]:
         batch_size, hidden_dim, seq_len = query.size(0), query.size(2), value.size(1)
 
         # Initialize previous attention (alignment) to zeros
         if last_attn is None:
             last_attn = value.new_zeros(batch_size, seq_len)
 
         conv_attn = torch.transpose(self.conv1d(last_attn.unsqueeze(1)), 1, 2)
-        score = self.score_proj(torch.tanh(
-                self.query_proj(query.reshape(-1, hidden_dim)).view(batch_size, -1, hidden_dim)
-                + self.value_proj(value.reshape(-1, hidden_dim)).view(batch_size, -1, hidden_dim)
+        score = self.score_proj(
+            torch.tanh(
+                self.query_proj(query.reshape(-1, hidden_dim)).view(
+                    batch_size, -1, hidden_dim
+                )
+                + self.value_proj(value.reshape(-1, hidden_dim)).view(
+                    batch_size, -1, hidden_dim
+                )
                 + conv_attn
                 + self.bias
-        )).squeeze(dim=-1)
+            )
+        ).squeeze(dim=-1)
 
         if self.smoothing:
             score = torch.sigmoid(score)
             attn = torch.div(score, score.sum(dim=-1).unsqueeze(dim=-1))
         else:
             attn = F.softmax(score, dim=-1)
 
-        context = torch.bmm(attn.unsqueeze(dim=1), value).squeeze(dim=1)  # Bx1xT X BxTxD => Bx1xD => BxD
+        context = torch.bmm(attn.unsqueeze(dim=1), value).squeeze(
+            dim=1
+        )  # Bx1xT X BxTxD => Bx1xD => BxD
 
         return context, attn
 
 
 class MultiHeadLocationAwareAttention(nn.Module):
     """
     Applies a multi-headed location-aware attention mechanism on the output features from the decoder.
@@ -159,47 +183,70 @@
     Returns: output, attn
         - **output** (batch, output_len, dimensions): tensor containing the feature from encoder outputs
         - **attn** (batch * num_heads, v_len): tensor containing the attention (alignment) from the encoder outputs.
     Reference:
         - **Attention Is All You Need**: https://arxiv.org/abs/1706.03762
         - **Attention-Based Models for Speech Recognition**: https://arxiv.org/abs/1506.07503
     """
-    def __init__(self, hidden_dim: int, num_heads: int = 8, conv_out_channel: int = 10) -> None:
+
+    def __init__(
+        self, hidden_dim: int, num_heads: int = 8, conv_out_channel: int = 10
+    ) -> None:
         super(MultiHeadLocationAwareAttention, self).__init__()
         self.hidden_dim = hidden_dim
         self.num_heads = num_heads
         self.dim = int(hidden_dim / num_heads)
         self.conv1d = nn.Conv1d(num_heads, conv_out_channel, kernel_size=3, padding=1)
         self.loc_proj = nn.Linear(conv_out_channel, self.dim, bias=False)
         self.query_proj = nn.Linear(hidden_dim, self.dim * num_heads, bias=False)
         self.value_proj = nn.Linear(hidden_dim, self.dim * num_heads, bias=False)
         self.score_proj = nn.Linear(self.dim, 1, bias=True)
         self.bias = nn.Parameter(torch.rand(self.dim).uniform_(-0.1, 0.1))
 
-    def forward(self, query: Tensor, value: Tensor, last_attn: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self, query: Tensor, value: Tensor, last_attn: Tensor
+    ) -> Tuple[Tensor, Tensor]:
         batch_size, seq_len = value.size(0), value.size(1)
 
         if last_attn is None:
             last_attn = value.new_zeros(batch_size, self.num_heads, seq_len)
 
         loc_energy = torch.tanh(self.loc_proj(self.conv1d(last_attn).transpose(1, 2)))
-        loc_energy = loc_energy.unsqueeze(1).repeat(1, self.num_heads, 1, 1).view(-1, seq_len, self.dim)
-
-        query = self.query_proj(query).view(batch_size, -1, self.num_heads, self.dim).permute(0, 2, 1, 3)
-        value = self.value_proj(value).view(batch_size, -1, self.num_heads, self.dim).permute(0, 2, 1, 3)
+        loc_energy = (
+            loc_energy.unsqueeze(1)
+            .repeat(1, self.num_heads, 1, 1)
+            .view(-1, seq_len, self.dim)
+        )
+
+        query = (
+            self.query_proj(query)
+            .view(batch_size, -1, self.num_heads, self.dim)
+            .permute(0, 2, 1, 3)
+        )
+        value = (
+            self.value_proj(value)
+            .view(batch_size, -1, self.num_heads, self.dim)
+            .permute(0, 2, 1, 3)
+        )
         query = query.contiguous().view(-1, 1, self.dim)
         value = value.contiguous().view(-1, seq_len, self.dim)
 
-        score = self.score_proj(torch.tanh(value + query + loc_energy + self.bias)).squeeze(2)
+        score = self.score_proj(
+            torch.tanh(value + query + loc_energy + self.bias)
+        ).squeeze(2)
         attn = F.softmax(score, dim=1)
 
-        value = value.view(batch_size, seq_len, self.num_heads, self.dim).permute(0, 2, 1, 3)
+        value = value.view(batch_size, seq_len, self.num_heads, self.dim).permute(
+            0, 2, 1, 3
+        )
         value = value.contiguous().view(-1, seq_len, self.dim)
 
-        context = torch.bmm(attn.unsqueeze(1), value).view(batch_size, -1, self.num_heads * self.dim)
+        context = torch.bmm(attn.unsqueeze(1), value).view(
+            batch_size, -1, self.num_heads * self.dim
+        )
         attn = attn.view(batch_size, self.num_heads, -1)
 
         return context, attn
 
 
 class MultiHeadAttention(nn.Module):
     """
@@ -228,50 +275,69 @@
             Case 2: come from the input embeddings
             Case 3: come from the output embedding (masked)
         - **mask** (-): tensor containing indices to be masked
     Returns: output, attn
         - **output** (batch, output_len, dimensions): tensor containing the attended output features.
         - **attn** (batch * num_heads, v_len): tensor containing the attention (alignment) from the encoder outputs.
     """
+
     def __init__(self, d_model: int = 512, num_heads: int = 8):
         super(MultiHeadAttention, self).__init__()
 
         assert d_model % num_heads == 0, "d_model % num_heads should be zero."
 
         self.d_head = int(d_model / num_heads)
         self.num_heads = num_heads
         self.scaled_dot_attn = ScaledDotProductAttention(self.d_head)
         self.query_proj = nn.Linear(d_model, self.d_head * num_heads)
         self.key_proj = nn.Linear(d_model, self.d_head * num_heads)
         self.value_proj = nn.Linear(d_model, self.d_head * num_heads)
 
     def forward(
-            self,
-            query: Tensor,
-            key: Tensor,
-            value: Tensor,
-            mask: Optional[Tensor] = None
+        self, query: Tensor, key: Tensor, value: Tensor, mask: Optional[Tensor] = None
     ) -> Tuple[Tensor, Tensor]:
         batch_size = value.size(0)
 
-        query = self.query_proj(query).view(batch_size, -1, self.num_heads, self.d_head)  # BxQ_LENxNxD
-        key = self.key_proj(key).view(batch_size, -1, self.num_heads, self.d_head)      # BxK_LENxNxD
-        value = self.value_proj(value).view(batch_size, -1, self.num_heads, self.d_head)  # BxV_LENxNxD
-
-        query = query.permute(2, 0, 1, 3).contiguous().view(batch_size * self.num_heads, -1, self.d_head)  # BNxQ_LENxD
-        key = key.permute(2, 0, 1, 3).contiguous().view(batch_size * self.num_heads, -1, self.d_head)      # BNxK_LENxD
-        value = value.permute(2, 0, 1, 3).contiguous().view(batch_size * self.num_heads, -1, self.d_head)  # BNxV_LENxD
+        query = self.query_proj(query).view(
+            batch_size, -1, self.num_heads, self.d_head
+        )  # BxQ_LENxNxD
+        key = self.key_proj(key).view(
+            batch_size, -1, self.num_heads, self.d_head
+        )  # BxK_LENxNxD
+        value = self.value_proj(value).view(
+            batch_size, -1, self.num_heads, self.d_head
+        )  # BxV_LENxNxD
+
+        query = (
+            query.permute(2, 0, 1, 3)
+            .contiguous()
+            .view(batch_size * self.num_heads, -1, self.d_head)
+        )  # BNxQ_LENxD
+        key = (
+            key.permute(2, 0, 1, 3)
+            .contiguous()
+            .view(batch_size * self.num_heads, -1, self.d_head)
+        )  # BNxK_LENxD
+        value = (
+            value.permute(2, 0, 1, 3)
+            .contiguous()
+            .view(batch_size * self.num_heads, -1, self.d_head)
+        )  # BNxV_LENxD
 
         if mask is not None:
             mask = mask.unsqueeze(1).repeat(1, self.num_heads, 1, 1)  # BxNxQ_LENxK_LEN
 
         context, attn = self.scaled_dot_attn(query, key, value, mask)
 
         context = context.view(self.num_heads, batch_size, -1, self.d_head)
-        context = context.permute(1, 2, 0, 3).contiguous().view(batch_size, -1, self.num_heads * self.d_head)  # BxTxND
+        context = (
+            context.permute(1, 2, 0, 3)
+            .contiguous()
+            .view(batch_size, -1, self.num_heads * self.d_head)
+        )  # BxTxND
 
         return context, attn
 
 
 class RelativeMultiHeadAttention(nn.Module):
     """
     Multi-head attention with relative positional encoding.
@@ -285,19 +351,20 @@
         - **key** (batch, time, dim): Tensor containing key vector
         - **value** (batch, time, dim): Tensor containing value vector
         - **pos_embedding** (batch, time, dim): Positional embedding tensor
         - **mask** (batch, 1, time2) or (batch, time1, time2): Tensor containing indices to be masked
     Returns:
         - **outputs**: Tensor produces by relative multi head attention module.
     """
+
     def __init__(
-            self,
-            d_model: int = 512,
-            num_heads: int = 16,
-            dropout_p: float = 0.1,
+        self,
+        d_model: int = 512,
+        num_heads: int = 16,
+        dropout_p: float = 0.1,
     ):
         super(RelativeMultiHeadAttention, self).__init__()
         assert d_model % num_heads == 0, "d_model % num_heads should be zero."
         self.d_model = d_model
         self.d_head = int(d_model / num_heads)
         self.num_heads = num_heads
         self.sqrt_dim = math.sqrt(d_model)
@@ -312,30 +379,44 @@
         self.v_bias = nn.Parameter(torch.Tensor(self.num_heads, self.d_head))
         torch.nn.init.xavier_uniform_(self.u_bias)
         torch.nn.init.xavier_uniform_(self.v_bias)
 
         self.out_proj = nn.Linear(d_model, d_model)
 
     def forward(
-            self,
-            query: Tensor,
-            key: Tensor,
-            value: Tensor,
-            pos_embedding: Tensor,
-            mask: Optional[Tensor] = None,
+        self,
+        query: Tensor,
+        key: Tensor,
+        value: Tensor,
+        pos_embedding: Tensor,
+        mask: Optional[Tensor] = None,
     ) -> Tensor:
         batch_size = value.size(0)
 
         query = self.query_proj(query).view(batch_size, -1, self.num_heads, self.d_head)
-        key = self.key_proj(key).view(batch_size, -1, self.num_heads, self.d_head).permute(0, 2, 1, 3)
-        value = self.value_proj(value).view(batch_size, -1, self.num_heads, self.d_head).permute(0, 2, 1, 3)
-        pos_embedding = self.pos_proj(pos_embedding).view(batch_size, -1, self.num_heads, self.d_head)
-
-        content_score = torch.matmul((query + self.u_bias).transpose(1, 2), key.transpose(2, 3))
-        pos_score = torch.matmul((query + self.v_bias).transpose(1, 2), pos_embedding.permute(0, 2, 3, 1))
+        key = (
+            self.key_proj(key)
+            .view(batch_size, -1, self.num_heads, self.d_head)
+            .permute(0, 2, 1, 3)
+        )
+        value = (
+            self.value_proj(value)
+            .view(batch_size, -1, self.num_heads, self.d_head)
+            .permute(0, 2, 1, 3)
+        )
+        pos_embedding = self.pos_proj(pos_embedding).view(
+            batch_size, -1, self.num_heads, self.d_head
+        )
+
+        content_score = torch.matmul(
+            (query + self.u_bias).transpose(1, 2), key.transpose(2, 3)
+        )
+        pos_score = torch.matmul(
+            (query + self.v_bias).transpose(1, 2), pos_embedding.permute(0, 2, 3, 1)
+        )
         pos_score = self._compute_relative_positional_encoding(pos_score)
 
         score = (content_score + pos_score) / self.sqrt_dim
 
         if mask is not None:
             mask = mask.unsqueeze(1)
             score.masked_fill_(mask, -1e9)
@@ -349,15 +430,17 @@
         return self.out_proj(context)
 
     def _compute_relative_positional_encoding(self, pos_score: Tensor) -> Tensor:
         batch_size, num_heads, seq_length1, seq_length2 = pos_score.size()
         zeros = pos_score.new_zeros(batch_size, num_heads, seq_length1, 1)
         padded_pos_score = torch.cat([zeros, pos_score], dim=-1)
 
-        padded_pos_score = padded_pos_score.view(batch_size, num_heads, seq_length2 + 1, seq_length1)
+        padded_pos_score = padded_pos_score.view(
+            batch_size, num_heads, seq_length2 + 1, seq_length1
+        )
         pos_score = padded_pos_score[:, :, 1:].view_as(pos_score)
 
         return pos_score
 
 
 class CustomizingAttention(nn.Module):
     r"""
@@ -378,51 +461,75 @@
         - **output** (batch, output_len, dimensions): tensor containing the attended output features from the decoder.
         - **attn** (batch * num_heads, v_len): tensor containing the alignment from the encoder outputs.
     Reference:
         - **Attention Is All You Need**: https://arxiv.org/abs/1706.03762
         - **Attention-Based Models for Speech Recognition**: https://arxiv.org/abs/1506.07503
     """
 
-    def __init__(self, hidden_dim: int, num_heads: int = 4, conv_out_channel: int = 10) -> None:
+    def __init__(
+        self, hidden_dim: int, num_heads: int = 4, conv_out_channel: int = 10
+    ) -> None:
         super(CustomizingAttention, self).__init__()
         self.hidden_dim = hidden_dim
         self.num_heads = num_heads
         self.dim = int(hidden_dim / num_heads)
         self.scaled_dot_attn = ScaledDotProductAttention(self.dim)
         self.conv1d = nn.Conv1d(1, conv_out_channel, kernel_size=3, padding=1)
         self.query_proj = nn.Linear(hidden_dim, self.dim * num_heads, bias=True)
         self.value_proj = nn.Linear(hidden_dim, self.dim * num_heads, bias=False)
         self.loc_proj = nn.Linear(conv_out_channel, self.dim, bias=False)
         self.bias = nn.Parameter(torch.rand(self.dim * num_heads).uniform_(-0.1, 0.1))
 
-    def forward(self, query: Tensor, value: Tensor, last_attn: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self, query: Tensor, value: Tensor, last_attn: Tensor
+    ) -> Tuple[Tensor, Tensor]:
         batch_size, q_len, v_len = value.size(0), query.size(1), value.size(1)
 
         if last_attn is None:
             last_attn = value.new_zeros(batch_size * self.num_heads, v_len)
 
-        loc_energy = self.get_loc_energy(last_attn, batch_size, v_len)  # get location energy
-
-        query = self.query_proj(query).view(batch_size, q_len, self.num_heads * self.dim)
-        value = self.value_proj(value).view(batch_size, v_len, self.num_heads * self.dim) + loc_energy + self.bias
-
-        query = query.view(batch_size, q_len, self.num_heads, self.dim).permute(2, 0, 1, 3)
-        value = value.view(batch_size, v_len, self.num_heads, self.dim).permute(2, 0, 1, 3)
+        loc_energy = self.get_loc_energy(
+            last_attn, batch_size, v_len
+        )  # get location energy
+
+        query = self.query_proj(query).view(
+            batch_size, q_len, self.num_heads * self.dim
+        )
+        value = (
+            self.value_proj(value).view(batch_size, v_len, self.num_heads * self.dim)
+            + loc_energy
+            + self.bias
+        )
+
+        query = query.view(batch_size, q_len, self.num_heads, self.dim).permute(
+            2, 0, 1, 3
+        )
+        value = value.view(batch_size, v_len, self.num_heads, self.dim).permute(
+            2, 0, 1, 3
+        )
         query = query.contiguous().view(-1, q_len, self.dim)
         value = value.contiguous().view(-1, v_len, self.dim)
 
         context, attn = self.scaled_dot_attn(query, value)
         attn = attn.squeeze()
 
-        context = context.view(self.num_heads, batch_size, q_len, self.dim).permute(1, 2, 0, 3)
+        context = context.view(self.num_heads, batch_size, q_len, self.dim).permute(
+            1, 2, 0, 3
+        )
         context = context.contiguous().view(batch_size, q_len, -1)
 
         return context, attn
 
     def get_loc_energy(self, last_attn: Tensor, batch_size: int, v_len: int) -> Tensor:
         conv_feat = self.conv1d(last_attn.unsqueeze(1))
-        conv_feat = conv_feat.view(batch_size, self.num_heads, -1, v_len).permute(0, 1, 3, 2)
-
-        loc_energy = self.loc_proj(conv_feat).view(batch_size, self.num_heads, v_len, self.dim)
-        loc_energy = loc_energy.permute(0, 2, 1, 3).reshape(batch_size, v_len, self.num_heads * self.dim)
+        conv_feat = conv_feat.view(batch_size, self.num_heads, -1, v_len).permute(
+            0, 1, 3, 2
+        )
+
+        loc_energy = self.loc_proj(conv_feat).view(
+            batch_size, self.num_heads, v_len, self.dim
+        )
+        loc_energy = loc_energy.permute(0, 2, 1, 3).reshape(
+            batch_size, v_len, self.num_heads * self.dim
+        )
 
-        return loc_energy
+        return loc_energy
```

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/layers.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,36 @@
 import torch.nn as nn
 from torch.nn import Linear
 
 from .FunctionalConvolution import *
 from .FunctionalConvolutionTranspose import *
 from .PolynomialLayers import *
 from .ProductLayer import *
-from .utils import l2_normalization, max_abs_normalization, max_abs_normalization_nd, max_center_normalization
+from .utils import (
+    l2_normalization,
+    max_abs_normalization,
+    max_abs_normalization_nd,
+    max_center_normalization,
+)
 
 
 class MaxAbsNormalization(nn.Module):
     """
     Normalization for the 1D case (MLP)
     """
 
     def __init__(self, eps: float = 1e-6):
         super().__init__()
         self._eps = eps
 
     def forward(self, x):
         return max_abs_normalization(x, eps=self._eps)
 
-class MaxCenterNormalization(nn.Module) :
+
+class MaxCenterNormalization(nn.Module):
     """
     Normalization for the 1D case (MLP) (x-avg)/(max(x)+eps) for each
     sample of the batch.
     """
 
     def __init__(self, eps: float = 1e-6):
         super().__init__()
@@ -88,14 +94,63 @@
         self._layer_list = layer_list
 
     def forward(self, x):
         x_all = [layer(x) for layer in self._layer_list]
         return torch.add(*x_all)
 
 
+class SwitchLayer(Module):
+    """
+    Switch layer just creates 2 (or more) identical input layers
+    and then multiplies the output of all those layers.  In effect
+    one of the layers can turn of features of the other.
+    """
+
+    def __init__(
+        self,
+        layer_type: str,
+        n: str,
+        in_width: int,
+        out_width: int,
+        scale: float = 2.0,
+        segments: int = None,
+        normalization: Callable[[Any], Any] = None,
+        num_input_layers: int = 2,
+    ) -> None:
+        super().__init__()
+
+        self._layers = [
+            high_order_fc_layers(
+                layer_type=layer_type,
+                n=n,
+                in_features=in_width,
+                out_features=out_width,
+                segments=segments,
+                rescale_output=False,
+                scale=scale,
+                periodicity=None,
+            )
+            for _ in range(num_input_layers)
+        ]
+
+        self._normalization = normalization
+
+    def forward(self, x) -> Tensor:
+        outputs = [layer(x) for layer in self._layers]
+
+        final = outputs[0]
+        for i in range(1, len(outputs)):
+            final *= outputs[i]
+
+        if self._normalization is not None:
+            final = self._normalization(final)
+        
+        return final
+
+
 fc_layers = {
     "baseline_relu": LinearReluAdapter,  # Linear layer folowed by relu
     "baseline": LinearAdapter,  # Standard linear layer
     "continuous": PiecewisePolynomial,
     "continuous_prod": PiecewisePolynomialProd,
     "discontinuous": PiecewiseDiscontinuousPolynomial,
     "discontinuous_prod": PiecewiseDiscontinuousPolynomialProd,
@@ -149,15 +204,14 @@
     for i in range(n):
         reg = [0] * n
         reg[i] = 1.0
         combos.append(reg)
 
         for j in range(i + 1, n):
             for r in range(1, rotations):
-
                 # We need to add rotations from each of 2 quadrants
                 temp = [0] * n
 
                 theta = (math.pi / 2) * (r / rotations)
                 rot_x = math.cos(theta)
                 rot_y = math.sin(theta)
                 norm_val = 1 if normalize is False else abs(rot_x) + abs(rot_y)
@@ -182,34 +236,31 @@
     layer = torch.nn.Linear(n, output_width, bias=False)
     weights = torch.tensor(combos)
     layer.weight = torch.nn.Parameter(weights, requires_grad=False)
     return layer, output_width
 
 
 def high_order_fc_layers(layer_type: str, **kwargs):
-
     if layer_type in fc_layers.keys():
         return fc_layers[layer_type](**kwargs)
 
     raise ValueError(
         f"Fully connected layer type {layer_type} not recognized.  Must be one of {list(fc_layers.keys())}"
     )
 
 
 def high_order_convolution_layers(layer_type: str, **kwargs):
-
     if layer_type in convolutional_layers.keys():
         return convolutional_layers[layer_type](**kwargs)
 
     raise ValueError(
         f"Convolutional layer type {layer_type} not recognized.  Must be one of {list(convolutional_layers.keys())}"
     )
 
 
 def high_order_convolution_transpose_layers(layer_type: str, **kwargs):
-
     if layer_type in convolutional_transpose_layers.keys():
         return convolutional_transpose_layers[layer_type](**kwargs)
 
     raise ValueError(
         f"ConvolutionalTranspose layer type {layer_type} not recognized.  Must be one of {list(convolutional_transpose_layers.keys())}"
     )
```

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/modules.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/modules.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/networks.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/networks.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/positional_embeddings.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/positional_embeddings.py`

 * *Files identical despite different names*

### Comparing `high_order_layers_torch-1.3.2/high_order_layers_torch/utils.py` & `high_order_layers_torch-1.3.3/high_order_layers_torch/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return x / (max_abs(x) + eps)
 
 
 def max_center_normalization(x: Tensor, eps: float = 1e-6):
     max_x = torch.max(x, dim=1, keepdim=True)[0]
     min_x = torch.min(x, dim=1, keepdim=True)[0]
 
-    midrange = 0.5*(max_x + min_x)
+    midrange = 0.5 * (max_x + min_x)
     mag = max_x - midrange
 
     centered = x - midrange
     return centered / (mag + eps)
 
 
 def l2_normalization(x: Tensor, eps: float = 1e-6):
```

### Comparing `high_order_layers_torch-1.3.2/pyproject.toml` & `high_order_layers_torch-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "high-order-layers-torch"
-version = "1.3.2"
+version = "1.3.3"
 description = "High order layers in pytorch"
 authors = ["jloverich <john.loverich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `high_order_layers_torch-1.3.2/setup.py` & `high_order_layers_torch-1.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'torch-optimizer>=0.3.0,<0.4.0',
  'torch>=2.0.0,<3.0.0',
  'torchmetrics>=0.10.2,<0.11.0',
  'torchvision>=0.15.1,<0.16.0']
 
 setup_kwargs = {
     'name': 'high-order-layers-torch',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'High order layers in pytorch',
-    'long_description': '![Build Status](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)\n\n# Piecewise Polynomial and Fourier Layers in PyTorch\n\nThis is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.\n\nLagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant.  Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models.  This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.\n\n## Idea\n\nThe idea is extremely simple - instead of a single weight at the synapse, use n-weights.  The n-weights describe a piecewise polynomial (or other complex function) and each of the n-weights can be updated independently.  A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well.  This can be implemented as construction of a polynomial or Fourier kernel followed by a standard pytorch layer where a linear activation is used.\n\nIn the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.\n\n<img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">\n\n## Why\n\nUsing higher order polynomial representations might allow networks with much fewer total weights. In physics, higher order methods\ncan be much more efficient. Spectral and discontinuous galerkin methods are examples of this.  Note that a standard neural network with relu activations is piecewise linear.  Here there are no bias weights and the "non-linearity" is in the synapse.  Also, I\'ve included discontinuous\nlayers, in physics there are many problems that are discontinuous (most non-linear hyperbolic conservation laws form discontinuities) in this case the method becomes a subgradient descent.\n\nIn addition, it\'s well known that the dendrites are also computational units in neurons, for example [Dendritic action potentials and computation in human layer 2/3 cortical neurons](https://science.sciencemag.org/content/367/6473/83) and this is a simple way to add more computational power into the artificial neural network model. In addition it\'s been shown that a single pyramidal has the same computational capacity as a 5 to 8 layer convolutional NN, [Single cortical neurons as deep artificial neural networks](https://www.sciencedirect.com/science/article/abs/pii/S0896627321005018?dgcid=author)\n\n\n\n## Speed\nSolving with relu layers is faster, however, sparsity may mean that there is a speed advantage in using the piecewise polynomial approach\nwhen there are many segments.  There do seem to be situations where the piecewise polynomial approach is significantly better than\nstandard relu layers.  Also, combining these layers with standard relu inputs, or using piecewise polynomial layer as inputs especially for implicit representation type problems (or as "positional embeddings") and in natural language problems seems to be useful.\n\n## Fully Connected Layer Types\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n\nA helper function is provided in selecting and switching between these layers\n\n```python\nfrom high_order_layers_torch.layers import *\nlayer1 = high_order_fc_layers(\n    layer_type=layer_type,\n    n=n,\n    in_features=784,\n    out_features=100,\n    segments=segments,\n    alpha=linear_part\n)\n```\n\nwhere `layer_type` is one of\n| layer_type          | representation\n|--------------------|-------------------------|\n|continuous         |  piecewise polynomial using sum at the neuron |\n|continuous_prod    |  piecewise polynomial using products at the neuron |\n|discontinuous      |  discontinuous piecewise polynomial with sum at the neuron|\n|discontinuous_prod | discontinous piecewise polynomial with product at the neuron|\n|polynomial | single polynomial (non piecewise) with sum at the neuron|\n|polynomial_prod | single polynomial (non piecewise) with product at the neuron|\n|product | Product |\n|fourier | fourier series with sum at the neuron |\n\n\n\n`n` is the number of interpolation points per segment for polynomials or the number of frequencies for fourier series, `segments` is the number of segments for piecewise polynomials, `alpha` is used in product layers and when set to 1 keeps the linear part of the product, when set to 0 it subtracts the linear part from the product.\n\n## Convolutional Layer Types\n\n```python\nconv_layer = high_order_convolution_layers(layer_type=layer_type, n=n, in_channels=3, out_channels=6, kernel_size=5, segments=segments, rescale_output=rescale_output, periodicity=periodicity)\n```\n\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n| layer_type   | representation       |\n|--------------|----------------------|\n|continuous(1d,2d)   | piecewise continuous polynomial\n|discontinuous(1d,2d) | piecewise discontinuous polynomial\n|polynomial(1d,2d) | single polynomial\n|fourier(1d,2d) | fourier series convolution\n\n## h and p refinement\np refinement is taking an existing network and increasing the polynomial order of that network without changing the network output.  This allow the user to train a network at low polynomial order and then use that same network to initialize a network with higher polynomial order.  This is particularly useful since a high order polynomial network will often converge poorly without the right initialization, the lower order network provides a good initial solution.  The function for changing the order of a network is\n```\nfrom high_order_layers_torch.networks import interpolate_high_order_mlp\ninterpolate_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n```\ncurrent implementation only works with high order MLPs, not with convnets.  A similar function exists for h refinement.  h refinement is\nrefining the number of segments in a layer, and is used for similar reasoning.  Layers with lots of segments may be slow to converge\nso the user starts with a small number of segments (1 or 2) and then increases the number of segments (h) using the lower initialization.  The following function currently only works for high order MLPs, not with convnets\n```\nfrom high_order_layers_torch.network import hp_refine_high_order_mlp\nhp_refine_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n)\n```\n# Installing\n\n## Installing locally\n\nThis repo uses poetry, so run\n\n```\npoetry install\n```\n\nand then\n\n```\npoetry shell\n```\n\n## Installing from pypi\n\n```bash\npip install high-order-layers-torch\n```\n\nor\n\n```\npoetry add high-order-layers-torch\n```\n# Examples\n\n## Simple function approximation\n\nApproximating a simple function using a single input and single output (single layer) with no hidden layers\nto approximate a function using continuous and discontinuous piecewise polynomials (with 5 pieces) and simple\npolynomials and fourier series.  The standard approach using ReLU is non competitive.  To see more complex see\nthe implicit representation page [here](https://github.com/jloveric/high-order-implicit-representation).\n\n![piecewise continuous polynomial](plots/piecewise_continuous.png)\n![piecewise discontinuous polynomial](plots/piecewise_discontinuous.png)\n![polynomial](plots/polynomial.png)\n![fourier series](plots/fourier_series.png)\n\n```python\npython examples/function_example.py\n```\n\n## XOR : 0.5 for x*y > 0 else -0.5\nSimple XOR problem using the standard network structure (2 inputs 2 hidden 1 output) this will also work with no hidden layers. The function is discontinuous along the axis and we try and fit that function. Using piecewise discontinuous layers the model can match the function exactly.\n![piecewise discontinuous polynomial](plots/xor_discontinuous.png)\nWith piecewise continuous it doesn\'t work quite as well.\n![piecewise continuous polynomial](plots/xor_continuous.png)\nPolynomial doesn\'t work well at all (expected).\n![polynomial](plots/xor_polynomial.png)\n\n## MNIST (convolutional)\n\n```python\npython examples/mnist.py max_epochs=1 train_fraction=0.1 layer_type=continuous2d n=4 segments=2\n```\n\n## CIFAR100 (convolutional)\n\n```\npython examples/cifar100.py -m max_epochs=20 train_fraction=1.0 layer_type=polynomial segments=2 n=7 nonlinearity=False rescale_output=False periodicity=2.0 lr=0.001 linear_output=False\n```\n\n## Variational Autoencoder\nStill a WIP.  Does work, but needs improvement.\n```\npython examples/variational_autoencoder.py -m max_epochs=300 train_fraction=1.0\n```\nrun with nevergrad for parameter tuning\n```\npython examples/variational_autoencoder.py -m\n```\n## Invariant MNIST (fully connected)\nWithout polynomial refinement\n```python\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 mlp.layer_type=continuous mlp.n=5 mlp.p_refine=False mlp.hidden.layers=4\n```\nwith polynomial refinement (p-refinement)\n```\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 layer_type=mlp.continuous mlp.n=2 mlp.target_n=5 mlp.p_refine=True\n```\nI\'ve also added hp refinement, but it needs a lot of testing.\n## Implicit Representation\n\nAn example of implicit representation for image compression, language generation can be found [here](https://github.com/jloveric/high-order-implicit-representation).  I intend to explore generative models in natural language further [here](https://github.com/jloveric/language-interpolation)\n\n## PDEs in Fluid Dynamics\n\nAn example using implicit representation to solve hyperbolic (nonlinear) wave equations can be found [here](https://github.com/jloveric/neural-network-pdes)\n\n## Natural Language Generation\n\nExamples using these networks for natural language generation can be found\n[here](https://github.com/jloveric/language-interpolation)\n\n## Generative music\n\nWork in progress\n[here](https://github.com/jloveric/high-order-generative-music)\n\n\n## Test and Coverage\nAfter installing and running\n```\npoetry shell\n```\nrun\n```\npytest\n```\nfor coverage, run\n```\ncoverage run -m pytest\n```\nand then\n```\ncoverage report\n```\n## A note on the unit\nThe layers used here do not require additional activation functions and use a simple sum or product in place of the activation.\nI almost always use sum units, but product units are performed in this manner\n\n$$ product=-1+\\prod_{i}(1 + f_{i})+(1-\\alpha)\\sum_{i}f_{i} $$\n\nThe 1 is added to each function output to as each of the sub products is also computed.  The linear part is controlled by\nthe alpha parameter.\n\n## Notes on normalization\nAlthough you can use batchnorm, layernorm etc... I\'ve found that you can actually just use the infinity norm ("max_abs" norm) which has no parameters\nfor this formulation (same approach seems not to work very well for standard relu networks - but need to investigate this further).\nThe max_abs normalization is defined this way\n```\nnormalized_x = x/(max(abs(x))+eps)\n```\nwhere the normalization is done per sample (as opposed to per batch).  The way the layers are formulated, we don\'t want the neuron\nvalues to extend beyond [-1, 1] as the polynomial values grow rapidly beyond that range.  I also use mirror periodicity to keep the\nvalues within from growing rapidly. We want the values to cover the entire range [-1, 1] of the polynomials as the weights\nare packed towards the edges of each segment. Normalizing by the sample L2 norm pushes most of the values towards\nzero, which I don\'t want.\n\n\n## Reference\n```\n@misc{Loverich2020,\n  author = {Loverich, John},\n  title = {High Order Layers Torch},\n  year = {2020},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/jloveric/high-order-layers-torch}},\n}\n```\n',
+    'long_description': '![Build Status](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)\n\n# Piecewise Polynomial and Fourier Layers in PyTorch\n\nThis is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.\n\nLagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant.  Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models.  This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.\n\n## Idea\n\nThe idea is extremely simple - instead of a single weight at the synapse, use n-weights.  The n-weights describe a piecewise polynomial (or other complex function) and each of the n-weights can be updated independently.  A Lagrange polynomial and Gauss Lobatto points are used to minimize oscillations of the polynomial.  The same approach can be applied to any "functional" synapse, and I also have Fourier series synapses in this repo as well.  This can be implemented as construction of a polynomial or Fourier kernel followed by a standard pytorch layer where a linear activation is used.\n\nIn the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.\n\n<img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">\n\n## Why\n\nUsing higher order polynomial representations might allow networks with much fewer total weights.\n\n\n## Fully Connected Layer Types\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n\nA helper function is provided in selecting and switching between these layers\n\n```python\nfrom high_order_layers_torch.layers import *\nlayer1 = high_order_fc_layers(\n    layer_type=layer_type,\n    n=n,\n    in_features=784,\n    out_features=100,\n    segments=segments,\n    alpha=linear_part\n)\n```\n\nwhere `layer_type` is one of\n| layer_type          | representation\n|--------------------|-------------------------|\n|continuous         |  piecewise polynomial using sum at the neuron |\n|continuous_prod    |  piecewise polynomial using products at the neuron |\n|discontinuous      |  discontinuous piecewise polynomial with sum at the neuron|\n|discontinuous_prod | discontinous piecewise polynomial with product at the neuron|\n|polynomial | single polynomial (non piecewise) with sum at the neuron|\n|polynomial_prod | single polynomial (non piecewise) with product at the neuron|\n|product | Product |\n|fourier | fourier series with sum at the neuron |\n\n\n\n`n` is the number of interpolation points per segment for polynomials or the number of frequencies for fourier series, `segments` is the number of segments for piecewise polynomials, `alpha` is used in product layers and when set to 1 keeps the linear part of the product, when set to 0 it subtracts the linear part from the product.\n\n## Convolutional Layer Types\n\n```python\nconv_layer = high_order_convolution_layers(layer_type=layer_type, n=n, in_channels=3, out_channels=6, kernel_size=5, segments=segments, rescale_output=rescale_output, periodicity=periodicity)\n```\n\nAll polynomials are Lagrange polynomials with Chebyshev interpolation points.\n| layer_type   | representation       |\n|--------------|----------------------|\n|continuous(1d,2d)   | piecewise continuous polynomial\n|discontinuous(1d,2d) | piecewise discontinuous polynomial\n|polynomial(1d,2d) | single polynomial\n|fourier(1d,2d) | fourier series convolution\n\n## h and p refinement\np refinement is taking an existing network and increasing the polynomial order of that network without changing the network output.  This allow the user to train a network at low polynomial order and then use that same network to initialize a network with higher polynomial order.  This is particularly useful since a high order polynomial network will often converge poorly without the right initialization, the lower order network provides a good initial solution.  The function for changing the order of a network is\n```\nfrom high_order_layers_torch.networks import interpolate_high_order_mlp\ninterpolate_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n```\ncurrent implementation only works with high order MLPs, not with convnets.  A similar function exists for h refinement.  h refinement is\nrefining the number of segments in a layer, and is used for similar reasoning.  Layers with lots of segments may be slow to converge\nso the user starts with a small number of segments (1 or 2) and then increases the number of segments (h) using the lower initialization.  The following function currently only works for high order MLPs, not with convnets\n```\nfrom high_order_layers_torch.network import hp_refine_high_order_mlp\nhp_refine_high_order_mlp(\n    network_in: HighOrderMLP, network_out: HighOrderMLP\n)\n```\n# Installing\n\n## Installing locally\n\nThis repo uses poetry, so run\n\n```\npoetry install\n```\n\nand then\n\n```\npoetry shell\n```\n\n## Installing from pypi\n\n```bash\npip install high-order-layers-torch\n```\n\nor\n\n```\npoetry add high-order-layers-torch\n```\n# Examples\n\n## Simple function approximation\n\nApproximating a simple function using a single input and single output (single layer) with no hidden layers\nto approximate a function using continuous and discontinuous piecewise polynomials (with 5 pieces) and simple\npolynomials and fourier series.  The standard approach using ReLU is non competitive.  To see more complex see\nthe implicit representation page [here](https://github.com/jloveric/high-order-implicit-representation).\n\n![piecewise continuous polynomial](plots/piecewise_continuous.png)\n![piecewise discontinuous polynomial](plots/piecewise_discontinuous.png)\n![polynomial](plots/polynomial.png)\n![fourier series](plots/fourier_series.png)\n\n```python\npython examples/function_example.py\n```\n\n## XOR : 0.5 for x*y > 0 else -0.5\nSimple XOR problem using the standard network structure (2 inputs 2 hidden 1 output) this will also work with no hidden layers. The function is discontinuous along the axis and we try and fit that function. Using piecewise discontinuous layers the model can match the function exactly.\n![piecewise discontinuous polynomial](plots/xor_discontinuous.png)\nWith piecewise continuous it doesn\'t work quite as well.\n![piecewise continuous polynomial](plots/xor_continuous.png)\nPolynomial doesn\'t work well at all (expected).\n![polynomial](plots/xor_polynomial.png)\n\n## MNIST (convolutional)\n\n```python\npython examples/mnist.py max_epochs=1 train_fraction=0.1 layer_type=continuous2d n=4 segments=2\n```\n\n## CIFAR100 (convolutional)\n\n```\npython examples/cifar100.py -m max_epochs=20 train_fraction=1.0 layer_type=polynomial segments=2 n=7 nonlinearity=False rescale_output=False periodicity=2.0 lr=0.001 linear_output=False\n```\n\n## Variational Autoencoder\nStill a WIP.  Does work, but needs improvement.\n```\npython examples/variational_autoencoder.py -m max_epochs=300 train_fraction=1.0\n```\nrun with nevergrad for parameter tuning\n```\npython examples/variational_autoencoder.py -m\n```\n## Invariant MNIST (fully connected)\nWithout polynomial refinement\n```python\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 mlp.layer_type=continuous mlp.n=5 mlp.p_refine=False mlp.hidden.layers=4\n```\nwith polynomial refinement (p-refinement)\n```\npython examples/invariant_mnist.py max_epochs=100 train_fraction=1 layer_type=mlp.continuous mlp.n=2 mlp.target_n=5 mlp.p_refine=True\n```\nI\'ve also added hp refinement, but it needs a lot of testing.\n## Implicit Representation\n\nAn example of implicit representation for image compression, language generation can be found [here](https://github.com/jloveric/high-order-implicit-representation).  I intend to explore generative models in natural language further [here](https://github.com/jloveric/language-interpolation)\n\n## PDEs in Fluid Dynamics\n\nAn example using implicit representation to solve hyperbolic (nonlinear) wave equations can be found [here](https://github.com/jloveric/neural-network-pdes)\n\n## Natural Language Generation\n\nExamples using these networks for natural language generation can be found\n[here](https://github.com/jloveric/language-interpolation)\n\n## Generative music\n\nWork in progress\n[here](https://github.com/jloveric/high-order-generative-music)\n\n\n## Test and Coverage\nAfter installing and running\n```\npoetry shell\n```\nrun\n```\npytest\n```\nfor coverage, run\n```\ncoverage run -m pytest\n```\nand then\n```\ncoverage report\n```\n## A note on the unit\nThe layers used here do not require additional activation functions and use a simple sum or product in place of the activation.\nI almost always use sum units, but product units are performed in this manner\n\n$$ product=-1+\\prod_{i}(1 + f_{i})+(1-\\alpha)\\sum_{i}f_{i} $$\n\nThe 1 is added to each function output to as each of the sub products is also computed.  The linear part is controlled by\nthe alpha parameter.\n\n## Notes on normalization\nAlthough you can use batchnorm, layernorm etc... I\'ve found that you can actually just use the infinity norm ("max_abs" norm) which has no parameters\nfor this formulation (same approach seems not to work very well for standard relu networks - but need to investigate this further).\nThe max_abs normalization is defined this way\n```\nnormalized_x = x/(max(abs(x))+eps)\n```\nwhere the normalization is done per sample (as opposed to per batch).  The way the layers are formulated, we don\'t want the neuron\nvalues to extend beyond [-1, 1] as the polynomial values grow rapidly beyond that range.  I also use mirror periodicity to keep the\nvalues within from growing rapidly. We want the values to cover the entire range [-1, 1] of the polynomials as the weights\nare packed towards the edges of each segment. Normalizing by the sample L2 norm pushes most of the values towards\nzero, which I don\'t want.\n\n\n## Reference\n```\n@misc{Loverich2020,\n  author = {Loverich, John},\n  title = {High Order Layers Torch},\n  year = {2020},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/jloveric/high-order-layers-torch}},\n}\n```\n',
     'author': 'jloverich',
     'author_email': 'john.loverich@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `high_order_layers_torch-1.3.2/PKG-INFO` & `high_order_layers_torch-1.3.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: high-order-layers-torch
-Version: 1.3.2
-Summary: High order layers in pytorch
-License: MIT
-Author: jloverich
-Author-email: john.loverich@gmail.com
-Requires-Python: >=3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hydra-core (>=1.2.0,<2.0.0)
-Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
-Requires-Dist: torch-optimizer (>=0.3.0,<0.4.0)
-Requires-Dist: torchmetrics (>=0.10.2,<0.11.0)
-Requires-Dist: torchvision (>=0.15.1,<0.16.0)
-Description-Content-Type: text/markdown
-
 ![Build Status](https://github.com/jloveric/high-order-layers-torch/actions/workflows/python-app.yml/badge.svg)
 
 # Piecewise Polynomial and Fourier Layers in PyTorch
 
 This is a PyTorch implementation of my tensorflow [repository](https://github.com/jloveric/high-order-layers) and is more complete due to the flexibility of PyTorch.
 
 Lagrange Polynomial, Piecewise Lagrange Polynomial, Discontinuous Piecewise Lagrange Polynomial, Fourier Series, sum and product layers in PyTorch.  The sparsity of using piecewise polynomial layers means that by adding new segments the representational power of your network increases, but the time to complete a forward step remains constant.  Implementation includes simple fully connected layers, convolution layers and deconvolutional layers using these models.  This is a PyTorch implementation of this [paper](https://www.researchgate.net/publication/276923198_Discontinuous_Piecewise_Polynomial_Neural_Networks) including extension to Fourier Series and convolutional neural networks.
@@ -33,27 +12,17 @@
 
 In the image below each "link" instead of being a single weight, is a function of both x and a set of weights.  These functions can consist of an orthogonal basis functions for efficient approximation.
 
 <img src="plots/NetworkZoom.png" width=50% height=50% style="display: block; margin: 0 auto">
 
 ## Why
 
-Using higher order polynomial representations might allow networks with much fewer total weights. In physics, higher order methods
-can be much more efficient. Spectral and discontinuous galerkin methods are examples of this.  Note that a standard neural network with relu activations is piecewise linear.  Here there are no bias weights and the "non-linearity" is in the synapse.  Also, I've included discontinuous
-layers, in physics there are many problems that are discontinuous (most non-linear hyperbolic conservation laws form discontinuities) in this case the method becomes a subgradient descent.
-
-In addition, it's well known that the dendrites are also computational units in neurons, for example [Dendritic action potentials and computation in human layer 2/3 cortical neurons](https://science.sciencemag.org/content/367/6473/83) and this is a simple way to add more computational power into the artificial neural network model. In addition it's been shown that a single pyramidal has the same computational capacity as a 5 to 8 layer convolutional NN, [Single cortical neurons as deep artificial neural networks](https://www.sciencedirect.com/science/article/abs/pii/S0896627321005018?dgcid=author)
-
+Using higher order polynomial representations might allow networks with much fewer total weights.
 
 
-## Speed
-Solving with relu layers is faster, however, sparsity may mean that there is a speed advantage in using the piecewise polynomial approach
-when there are many segments.  There do seem to be situations where the piecewise polynomial approach is significantly better than
-standard relu layers.  Also, combining these layers with standard relu inputs, or using piecewise polynomial layer as inputs especially for implicit representation type problems (or as "positional embeddings") and in natural language problems seems to be useful.
-
 ## Fully Connected Layer Types
 All polynomials are Lagrange polynomials with Chebyshev interpolation points.
 
 A helper function is provided in selecting and switching between these layers
 
 ```python
 from high_order_layers_torch.layers import *
@@ -263,8 +232,7 @@
   title = {High Order Layers Torch},
   year = {2020},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/jloveric/high-order-layers-torch}},
 }
 ```
-
```

