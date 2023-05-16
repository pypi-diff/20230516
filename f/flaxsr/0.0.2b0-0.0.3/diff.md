# Comparing `tmp/flaxsr-0.0.2b0-py3-none-any.whl.zip` & `tmp/flaxsr-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,29 @@
-Zip file size: 15146 bytes, number of entries: 19
--rw-rw-r--  2.0 unx       42 b- defN 23-Apr-16 13:04 FlaxSR/__init__.py
--rw-rw-r--  2.0 unx      179 b- defN 23-Apr-16 09:21 FlaxSR/layers/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Apr-17 07:28 FlaxSR/layers/stochastic.py
--rw-rw-r--  2.0 unx     1567 b- defN 23-Apr-17 11:53 FlaxSR/layers/upscale.py
--rw-rw-r--  2.0 unx      355 b- defN 23-Apr-17 07:49 FlaxSR/models/__init__.py
--rw-rw-r--  2.0 unx     3658 b- defN 23-Apr-16 13:12 FlaxSR/models/edsr.py
--rw-rw-r--  2.0 unx      858 b- defN 23-Apr-16 12:22 FlaxSR/models/espcn.py
--rw-rw-r--  2.0 unx     1072 b- defN 23-Apr-16 12:04 FlaxSR/models/fsrcnn.py
--rw-rw-r--  2.0 unx     6626 b- defN 23-Apr-17 11:41 FlaxSR/models/nafssr.py
--rw-rw-r--  2.0 unx      930 b- defN 23-Apr-17 06:11 FlaxSR/models/ncnet.py
--rw-rw-r--  2.0 unx     1013 b- defN 23-Apr-16 13:13 FlaxSR/models/srcnn.py
--rw-rw-r--  2.0 unx     2138 b- defN 23-Apr-17 06:39 FlaxSR/models/srgan.py
--rw-rw-r--  2.0 unx      600 b- defN 23-Apr-17 11:53 FlaxSR/models/swinir.py
--rw-rw-r--  2.0 unx      890 b- defN 23-Apr-16 12:47 FlaxSR/models/vdsr.py
--rw-rw-r--  2.0 unx    11313 b- defN 23-Apr-17 11:54 flaxsr-0.0.2b0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1301 b- defN 23-Apr-17 11:54 flaxsr-0.0.2b0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 11:54 flaxsr-0.0.2b0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-17 11:54 flaxsr-0.0.2b0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1499 b- defN 23-Apr-17 11:54 flaxsr-0.0.2b0.dist-info/RECORD
-19 files, 35617 bytes uncompressed, 12716 bytes compressed:  64.3%
+Zip file size: 20481 bytes, number of entries: 27
+-rw-rw-r--  2.0 unx       88 b- defN 23-May-12 09:52 flaxsr/__init__.py
+-rw-rw-r--  2.0 unx      661 b- defN 23-May-12 10:02 flaxsr/_utils.py
+-rw-rw-r--  2.0 unx      179 b- defN 23-May-12 09:22 flaxsr/layers/__init__.py
+-rw-rw-r--  2.0 unx     1651 b- defN 23-May-16 13:28 flaxsr/layers/stochastic.py
+-rw-rw-r--  2.0 unx     1673 b- defN 23-May-16 13:28 flaxsr/layers/upscale.py
+-rw-rw-r--  2.0 unx      365 b- defN 23-May-12 09:22 flaxsr/losses/__init__.py
+-rw-rw-r--  2.0 unx     4049 b- defN 23-May-16 15:56 flaxsr/losses/adversarial_losses.py
+-rw-rw-r--  2.0 unx     2298 b- defN 23-May-16 15:02 flaxsr/losses/perceptual_losses.py
+-rw-rw-r--  2.0 unx     1745 b- defN 23-May-12 13:40 flaxsr/losses/pixel_wise_losses.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-May-16 12:58 flaxsr/losses/utils.py
+-rw-rw-r--  2.0 unx      355 b- defN 23-May-12 09:22 flaxsr/models/__init__.py
+-rw-rw-r--  2.0 unx     3749 b- defN 23-May-12 09:48 flaxsr/models/edsr.py
+-rw-rw-r--  2.0 unx      922 b- defN 23-May-12 09:48 flaxsr/models/espcn.py
+-rw-rw-r--  2.0 unx     1138 b- defN 23-May-12 09:48 flaxsr/models/fsrcnn.py
+-rw-rw-r--  2.0 unx     6677 b- defN 23-May-12 09:48 flaxsr/models/nafssr.py
+-rw-rw-r--  2.0 unx      994 b- defN 23-May-12 09:48 flaxsr/models/ncnet.py
+-rw-rw-r--  2.0 unx     1078 b- defN 23-May-12 09:49 flaxsr/models/srcnn.py
+-rw-rw-r--  2.0 unx     2205 b- defN 23-May-12 09:49 flaxsr/models/srgan.py
+-rw-rw-r--  2.0 unx      954 b- defN 23-May-12 09:50 flaxsr/models/vdsr.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-12 09:22 flaxsr/training/__init__.py
+-rw-rw-r--  2.0 unx      430 b- defN 23-May-12 13:43 flaxsr/training/train_states.py
+-rw-rw-r--  2.0 unx      875 b- defN 23-May-12 13:43 flaxsr/training/train_step.py
+-rw-rw-r--  2.0 unx    11313 b- defN 23-May-16 15:58 flaxsr-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1304 b- defN 23-May-16 15:58 flaxsr-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-16 15:58 flaxsr-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-16 15:58 flaxsr-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2169 b- defN 23-May-16 15:58 flaxsr-0.0.3.dist-info/RECORD
+27 files, 49304 bytes uncompressed, 17003 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,58 +1,82 @@
-Filename: FlaxSR/__init__.py
+Filename: flaxsr/__init__.py
 Comment: 
 
-Filename: FlaxSR/layers/__init__.py
+Filename: flaxsr/_utils.py
 Comment: 
 
-Filename: FlaxSR/layers/stochastic.py
+Filename: flaxsr/layers/__init__.py
 Comment: 
 
-Filename: FlaxSR/layers/upscale.py
+Filename: flaxsr/layers/stochastic.py
 Comment: 
 
-Filename: FlaxSR/models/__init__.py
+Filename: flaxsr/layers/upscale.py
 Comment: 
 
-Filename: FlaxSR/models/edsr.py
+Filename: flaxsr/losses/__init__.py
 Comment: 
 
-Filename: FlaxSR/models/espcn.py
+Filename: flaxsr/losses/adversarial_losses.py
 Comment: 
 
-Filename: FlaxSR/models/fsrcnn.py
+Filename: flaxsr/losses/perceptual_losses.py
 Comment: 
 
-Filename: FlaxSR/models/nafssr.py
+Filename: flaxsr/losses/pixel_wise_losses.py
 Comment: 
 
-Filename: FlaxSR/models/ncnet.py
+Filename: flaxsr/losses/utils.py
 Comment: 
 
-Filename: FlaxSR/models/srcnn.py
+Filename: flaxsr/models/__init__.py
 Comment: 
 
-Filename: FlaxSR/models/srgan.py
+Filename: flaxsr/models/edsr.py
 Comment: 
 
-Filename: FlaxSR/models/swinir.py
+Filename: flaxsr/models/espcn.py
 Comment: 
 
-Filename: FlaxSR/models/vdsr.py
+Filename: flaxsr/models/fsrcnn.py
 Comment: 
 
-Filename: flaxsr-0.0.2b0.dist-info/LICENSE
+Filename: flaxsr/models/nafssr.py
 Comment: 
 
-Filename: flaxsr-0.0.2b0.dist-info/METADATA
+Filename: flaxsr/models/ncnet.py
 Comment: 
 
-Filename: flaxsr-0.0.2b0.dist-info/WHEEL
+Filename: flaxsr/models/srcnn.py
 Comment: 
 
-Filename: flaxsr-0.0.2b0.dist-info/top_level.txt
+Filename: flaxsr/models/srgan.py
 Comment: 
 
-Filename: flaxsr-0.0.2b0.dist-info/RECORD
+Filename: flaxsr/models/vdsr.py
+Comment: 
+
+Filename: flaxsr/training/__init__.py
+Comment: 
+
+Filename: flaxsr/training/train_states.py
+Comment: 
+
+Filename: flaxsr/training/train_step.py
+Comment: 
+
+Filename: flaxsr-0.0.3.dist-info/LICENSE
+Comment: 
+
+Filename: flaxsr-0.0.3.dist-info/METADATA
+Comment: 
+
+Filename: flaxsr-0.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: flaxsr-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: flaxsr-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `FlaxSR/layers/upscale.py` & `flaxsr/layers/upscale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 
 import flax
 import flax.linen as nn
+from flaxsr._utils import register
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal, Optional
 
@@ -24,22 +25,24 @@
                 jnp.eye(input_c), (out_c * (scale ** 2)) // input_c, axis=0
             ), (1, 1, -1, input_c)
         ), (0, 1, 3, 2)
     )
     return kernel
 
 
+@register('layers', 'pixelshuffle')
 class PixelShuffle(nn.Module):
     scale: int
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
         return _pixel_shuffle(inputs, self.scale)
 
 
+@register('layers', 'nearestconv')
 class NearestConv(nn.Module):
     scale: int
     out_c: Optional[int] = None
     return_upscaled: bool = True
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
```

## Comparing `FlaxSR/models/edsr.py` & `flaxsr/models/edsr.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
-from FlaxSR.layers import PixelShuffle
+from flaxsr.layers import PixelShuffle
+from flaxsr._utils import register
 
 
 class ResBlock(nn.Module):
     n_filters: int
     scale_factor: float = .1
     kernel_size: Sequence[int] = (3, 3)
 
@@ -42,14 +43,15 @@
             inputs = nn.Conv(self.n_filters * 4, (3, 3), padding='SAME')(inputs)
             inputs = PixelShuffle(2)(inputs)
         else:
             raise ValueError(f'Invalid scale: {self.scale}, only support 2, 3, 4')
         return inputs
 
 
+@register('models', 'edsr')
 class EDSR(nn.Module):
     n_filters: int
     n_blocks: int
     scale: int  # Upscale ratio
     scale_factor: float = .1  # LayerScale
 
     @nn.compact
@@ -75,14 +77,15 @@
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
         inputs = inputs + ResBlock(self.n_filters, self.scale_factor, (5, 5))(inputs)
         inputs = inputs + ResBlock(self.n_filters, self.scale_factor, (5, 5))(inputs)
         return inputs
 
 
+@register('models', 'mdsr')
 class MDSR(nn.Module):
     n_filters: int
     n_blocks: int
     scale_factor: float = .1
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> Sequence[jnp.ndarray]:
```

## Comparing `FlaxSR/models/espcn.py` & `flaxsr/models/espcn.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
-from FlaxSR.layers import PixelShuffle
+from flaxsr.layers import PixelShuffle
+from flaxsr._utils import register
 
 
+@register('models', 'espcn')
 class ESPCN(nn.Module):
     n_filters: Sequence[int]
     kernel_size: Sequence[int]
     scale: int
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
```

## Comparing `FlaxSR/models/fsrcnn.py` & `flaxsr/models/fsrcnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
+from flaxsr._utils import register
 
+
+@register('models', 'fsrcnn')
 class FSRCNN(nn.Module):
     """
     Original paper only upscale Y channel of YCbCr image.
     """
     d: int
     s: int
     m: int
```

## Comparing `FlaxSR/models/nafssr.py` & `flaxsr/models/nafssr.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal, Optional
 
-from FlaxSR.layers import PixelShuffle, DropPathFast
+from flaxsr.layers import PixelShuffle
+from flaxsr._utils import register
 
 
 def _simple_gate(inputs: jnp.ndarray) -> jnp.ndarray:
     x1, x2 = jnp.split(inputs, inputs.shape[-1] // 2, axis=-1)
     return x1 * x2
 
 
@@ -121,14 +122,15 @@
             if survival_state:
                 feats_new = self.forward(feats, training=training)
                 return [f + ((f_n - f) / self.survival_prob) for f, f_n in zip(feats, feats_new)]
             else:
                 return feats
 
 
+@register('models', 'nafssr')
 class NAFSSR(nn.Module):
     n_filters: int
     n_blocks: int
     train_patch_size: Sequence[int]
     attn_scale: float
     drop_rate: float
     scale: int
```

## Comparing `FlaxSR/models/srcnn.py` & `flaxsr/models/srcnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
+from flaxsr._utils import register
 
+
+@register('models', 'srcnn')
 class SRCNN(nn.Module):
     """
     I fixed n_layers as 3 and kernel_size as 9, 1, 5.
     In paper, there's 4-5 layers versions.
     """
     n_filters: Sequence[int]  # 2 length. Last one is the number of output channels.
     scale: int
```

## Comparing `FlaxSR/models/srgan.py` & `flaxsr/models/srgan.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal, Optional
 
-from FlaxSR.layers import PixelShuffle
+from flaxsr.layers import PixelShuffle
+from flaxsr._utils import register
 
 
 """
 Implemented SRResNet only.
 SRGAN will be implemented later.
 """
 
@@ -29,14 +30,15 @@
         residual = nn.BatchNorm()(residual, use_running_average=not training)
         residual = nn.PReLU(residual)
         residual = nn.Conv(shape[-1], (3, 3), padding='SAME')(residual)
         residual = nn.BatchNorm()(residual, use_running_average=not training)
         return inputs + residual
 
 
+@register('models', 'srresnet')
 class SRResNet(nn.Module):
     n_filters: int
     n_blocks: int
     scale: int
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray, training: bool, **kwargs) -> jnp.ndarray:
```

## Comparing `FlaxSR/models/vdsr.py` & `flaxsr/models/vdsr.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
+from flaxsr._utils import register
 
+
+@register('models', 'vdsr')
 class VDSR(nn.Module):
     n_filters: int
     n_blocks: int
     scale: int
 
     @nn.compact
     def __call__(self, inputs: jnp.ndarray) -> jnp.ndarray:
```

## Comparing `flaxsr-0.0.2b0.dist-info/LICENSE` & `flaxsr-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flaxsr-0.0.2b0.dist-info/METADATA` & `flaxsr-0.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.2b0
+Version: 0.0.3
 Summary: Super Resolution models with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+
+
+
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
 ## HOW TO USE
 
 ### Install
 ```shell
 pip install flaxsr
 ```
 
 ### Usage
+
 ```python
-from FlaxSR.models import VDSR
+from flaxsr.models import VDSR
 import jax
 import jax.numpy as jnp
 
 inputs = jnp.ones((16, 256, 256, 3))
 key = jax.random.PRNGKey(42)
 model = VDSR(n_filters=64, n_blocks=20, scale=4)
 params = model.init(key, inputs)
```

