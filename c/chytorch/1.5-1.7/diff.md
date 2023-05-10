# Comparing `tmp/chytorch-1.5-py3-none-any.whl.zip` & `tmp/chytorch-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 23569 bytes, number of entries: 20
+Zip file size: 23767 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat     1020 b- defN 22-Mar-14 17:11 chytorch/nn/__init__.py
 -rw-rw-rw-  2.0 fat     1182 b- defN 22-Mar-14 17:11 chytorch/nn/activation.py
 -rw-rw-rw-  2.0 fat     2039 b- defN 22-Mar-14 17:11 chytorch/nn/functional.py
 -rw-rw-rw-  2.0 fat     4000 b- defN 22-Mar-14 17:11 chytorch/nn/molecule.py
--rw-rw-rw-  2.0 fat     4358 b- defN 22-Apr-01 16:10 chytorch/nn/reaction.py
+-rw-rw-rw-  2.0 fat     4358 b- defN 22-Apr-22 13:53 chytorch/nn/reaction.py
 -rw-rw-rw-  2.0 fat     2861 b- defN 22-Apr-01 17:04 chytorch/nn/transformer.py
--rw-rw-rw-  2.0 fat     3963 b- defN 22-Mar-15 09:53 chytorch/nn/voting.py
+-rw-rw-rw-  2.0 fat     4095 b- defN 22-May-20 14:07 chytorch/nn/voting.py
 -rw-rw-rw-  2.0 fat      803 b- defN 22-Mar-14 17:11 chytorch/optim/__init__.py
--rw-rw-rw-  2.0 fat     3074 b- defN 22-Mar-14 17:11 chytorch/optim/lr_scheduler.py
+-rw-rw-rw-  2.0 fat     2697 b- defN 22-Apr-25 14:14 chytorch/optim/lr_scheduler.py
 -rw-rw-rw-  2.0 fat      803 b- defN 22-Mar-14 17:11 chytorch/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3996 b- defN 22-Mar-14 17:11 chytorch/utils/cache.py
--rw-rw-rw-  2.0 fat     1261 b- defN 22-Mar-14 17:11 chytorch/utils/data/__init__.py
--rw-rw-rw-  2.0 fat     4832 b- defN 22-Mar-14 17:11 chytorch/utils/data/molecule.py
--rw-rw-rw-  2.0 fat     4688 b- defN 22-Mar-14 17:11 chytorch/utils/data/reaction.py
+-rw-rw-rw-  2.0 fat     1771 b- defN 22-May-12 08:57 chytorch/utils/data/__init__.py
+-rw-rw-rw-  2.0 fat     5039 b- defN 22-May-11 09:01 chytorch/utils/data/molecule.py
+-rw-rw-rw-  2.0 fat     4854 b- defN 22-May-11 09:01 chytorch/utils/data/reaction.py
 -rw-rw-rw-  2.0 fat       84 b- defN 22-Mar-14 17:11 chytorch/zoo/README.md
--rw-rw-rw-  2.0 fat     7817 b- defN 22-Apr-01 17:14 chytorch-1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4496 b- defN 22-Apr-01 17:14 chytorch-1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Apr-01 17:14 chytorch-1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Apr-01 17:14 chytorch-1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1617 b- defN 22-Apr-01 17:14 chytorch-1.5.dist-info/RECORD
-20 files, 52995 bytes uncompressed, 20947 bytes compressed:  60.5%
+-rw-rw-rw-  2.0 fat     7817 b- defN 22-May-31 09:18 chytorch-1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4496 b- defN 22-May-31 09:18 chytorch-1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-May-31 09:18 chytorch-1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 22-May-31 09:18 chytorch-1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1617 b- defN 22-May-31 09:18 chytorch-1.7.dist-info/RECORD
+20 files, 53633 bytes uncompressed, 21145 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: chytorch/utils/data/reaction.py
 Comment: 
 
 Filename: chytorch/zoo/README.md
 Comment: 
 
-Filename: chytorch-1.5.dist-info/LICENSE
+Filename: chytorch-1.7.dist-info/LICENSE
 Comment: 
 
-Filename: chytorch-1.5.dist-info/METADATA
+Filename: chytorch-1.7.dist-info/METADATA
 Comment: 
 
-Filename: chytorch-1.5.dist-info/WHEEL
+Filename: chytorch-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: chytorch-1.5.dist-info/top_level.txt
+Filename: chytorch-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: chytorch-1.5.dist-info/RECORD
+Filename: chytorch-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chytorch/nn/voting.py

```diff
@@ -18,74 +18,76 @@
 #
 from torch import bmm, no_grad
 from torch.nn import Dropout, GELU, LayerNorm, LazyLinear, Linear, Module
 from torch.nn.functional import cross_entropy, l1_loss, softmax
 
 
 class VotingRegressor(Module):
-    def __init__(self, ensemble: int = 10, hidden: int = 256,
-                 dropout: float = 0.5, activation=GELU, layer_norm_eps: float = 1e-5):
+    def __init__(self, ensemble: int = 10, hidden: int = 256, dropout: float = .5,
+                 activation=GELU, layer_norm_eps: float = 1e-5, loss_function=l1_loss):
         super().__init__()
         self.linear1 = LazyLinear(hidden * ensemble)
         self.layer_norm = LayerNorm(hidden, layer_norm_eps)
         self.activation = activation()
         self.dropout = Dropout(dropout)
         self.linear2 = Linear(hidden, ensemble)
+        self.loss_function = loss_function
 
         self._ensemble = ensemble
         self._hidden = hidden
 
     def forward(self, x):
         # B x E >> B x N*H >> B x N x H >> N x B x H
         x = self.linear1(x).view(-1, self._ensemble, self._hidden).transpose(0, 1)
         x = self.dropout(self.activation(self.layer_norm(x)))
         # N x H >> N x H x 1
         w = self.linear2.weight.unsqueeze(2)
         # N x B x 1 >> N x B >> B x N
         return bmm(x, w).squeeze(-1).transpose(0, 1).contiguous() + self.linear2.bias
 
-    def loss(self, x, y, loss=l1_loss):
+    def loss(self, x, y):
         p = self.forward(x)
-        return loss(p, y.expand(p.size()))
+        return self.loss_function(p, y.expand(p.size()))
 
     @no_grad()
     def predict(self, x, return_std: bool = False):
         p = self.forward(x)
         if return_std:
             return p.mean(1), p.std(1)
         return p.mean(1)
 
 
 class VotingClassifier(Module):
     def __init__(self, ensemble: int = 10, hidden: int = 256, n_classes: int = 2,
-                 dropout: float = 0.5, activation=GELU, layer_norm_eps: float = 1e-5):
+                 dropout: float = .5, activation=GELU, layer_norm_eps: float = 1e-5, loss_function=cross_entropy):
         super().__init__()
         self.linear1 = LazyLinear(hidden * ensemble)
         self.layer_norm = LayerNorm(hidden, layer_norm_eps)
         self.activation = activation()
         self.dropout = Dropout(dropout)
         self.linear2 = Linear(hidden, ensemble * n_classes)
+        self.loss_function = loss_function
 
         self._n_classes = n_classes
         self._ensemble = ensemble
         self._hidden = hidden
 
     def forward(self, x):
         # B x E >> B x N*H >> B x N x H >> N x B x H
         x = self.linear1(x).view(-1, self._ensemble, self._hidden).transpose(0, 1)
         x = self.dropout(self.activation(self.layer_norm(x)))
         # N * C x H >> N x C x H >> N x H x C
         w = self.linear2.weight.view(self._ensemble, -1, self._hidden).transpose(1, 2)
         # N x B x C >> B x N x C
         return bmm(x, w).transpose(0, 1).contiguous() + self.linear2.bias.view(self._ensemble, -1)
 
-    def loss(self, x, y, loss=cross_entropy):
+    def loss(self, x, y):
         p = self.forward(x).view(-1, self._n_classes)  # B x N x C >> B * N x C
         t = y.unsqueeze(-1).expand(-1, self._ensemble).flatten()  # B >> B x 1 >> B x N >> N * B
-        return loss(p, t)
+        return self.loss_function(p, t)
 
     @no_grad()
     def predict(self, x):
         return softmax(self.forward(x), 2).mean(1).argmax(1)
 
     @no_grad()
     def predict_proba(self, x, return_std: bool = False):
```

## chytorch/optim/lr_scheduler.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-#  Copyright 2021 Ramil Nugmanov <nougmanoff@protonmail.com>
+#  Copyright 2021, 2022 Ramil Nugmanov <nougmanoff@protonmail.com>
 #  This file is part of chytorch.
 #
 #  chytorch is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
 #
@@ -13,61 +13,49 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, see <https://www.gnu.org/licenses/>.
 #
 from math import cos, pi
+from torch.optim.lr_scheduler import _LRScheduler
 
 
-class WarmUpCosine:
+class WarmUpCosine(_LRScheduler):
     """
     Warm-Up with non-periodic Cosine.
 
     Note: some code copy-pasted from torch.optim.lr_scheduler.
     """
-    def __init__(self, optimizer, decrease_coef=.01, warmup=100, period=1000, last_epoch=-1, logger=None):
+    def __init__(self, optimizer, decrease_coef=.01, warmup=100, period=1000, last_epoch=-1):
         """
         :param warmup: number of batches/epochs for linear lr warm up.
         :param period: number of batches/epochs for decreasing from lr to decrease_coef * lr.
         """
         self.optimizer = optimizer
         self.last_epoch = last_epoch
         self.decrease_coef = decrease_coef
         self.warmup = warmup
         self.period = period
-        self.logger = logger
 
         if last_epoch == -1:
             for group in optimizer.param_groups:
                 group.setdefault('initial_lr', group['lr'])
         self._base_lrs = [group['initial_lr'] for group in optimizer.param_groups]
         self._min_lrs = [lr * decrease_coef for lr in self._base_lrs]
         self._delta_lrs = [(x - y) / 2 for x, y in zip(self._base_lrs, self._min_lrs)]
         self._period_warmup = period + warmup
         self.step()
 
-    def state_dict(self):
-        return {key: value for key, value in self.__dict__.items() if key != 'optimizer'}
-
-    def load_state_dict(self, state_dict):
-        self.__dict__.update(state_dict)
-
-    def get_last_lr(self):
-        return self._last_lr
-
     def step(self):
         self.last_epoch += 1
         self._last_lr = values = self.get_lr()
 
         for i, (group, lr) in enumerate(zip(self.optimizer.param_groups, values)):
             group['lr'] = lr
-        if self.logger is not None:
-            for i, v in enumerate(values):
-                self.logger(f'scheduler_param_{i}', v)
 
     def get_lr(self):
         if self.last_epoch == 0:
             return [0.] * len(self._base_lrs)
         elif self.last_epoch <= self.warmup:
             return [lr * self.last_epoch / self.warmup for lr in self._base_lrs]
         elif self.last_epoch >= self._period_warmup:
```

## chytorch/utils/data/__init__.py

```diff
@@ -12,22 +12,43 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program; if not, see <https://www.gnu.org/licenses/>.
 #
+from torch import Size
+from typing import List
 from .molecule import *
 from .reaction import *
 
 
 def chained_collate(*collate_fns):
+    """
+    Collate batch of tuples with different data structures by different collate functions.
+    """
     def w(batch):
         sub_batches = [[] for _ in collate_fns]
         for x in batch:
             for y, s in zip(x, sub_batches):
                 s.append(y)
         return [f(x) for x, f in zip(sub_batches, collate_fns)]
     return w
 
 
-__all__ = ['MoleculeDataset', 'ReactionDataset', 'collate_molecules', 'collate_reactions', 'chained_collate']
+class SizedList(List):
+    """
+    List with tensor-like size method.
+    """
+    def __init__(self, data):
+        super().__init__(data)
+
+    def size(self, dim=None):
+        if dim == 0:
+            return len(self)
+        elif dim is None:
+            return Size((len(self),))
+        raise IndexError
+
+
+__all__ = ['MoleculeDataset', 'ReactionDataset', 'SizedList',
+           'collate_molecules', 'collate_reactions', 'chained_collate']
```

## chytorch/utils/data/molecule.py

```diff
@@ -19,15 +19,15 @@
 from chython import MoleculeContainer
 from numpy import minimum, nan_to_num, ones
 from scipy.sparse.csgraph import shortest_path
 from torch import IntTensor, Size, int32, ones as t_ones, zeros
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
 from torchtyping import TensorType
-from typing import Sequence, Tuple
+from typing import Sequence, Tuple, Union
 
 
 def collate_molecules(batch) -> Tuple[TensorType['batch', 'tokens', int], TensorType['batch', 'tokens', int],
                                       TensorType['batch', 'tokens', 'tokens', int]]:
     """
     Prepares batches of molecules.
 
@@ -51,15 +51,16 @@
         tmp[i, :s, :s] = d
     return pa, pad_sequence(neighbors, True), tmp
 
 
 class MoleculeDataset(Dataset):
     __slots__ = ('molecules', 'distance_cutoff', 'add_cls')
 
-    def __init__(self, molecules: Sequence[MoleculeContainer], *, distance_cutoff: int = 8, add_cls: bool = True):
+    def __init__(self, molecules: Sequence[Union[MoleculeContainer, bytes]], *, distance_cutoff: int = 10,
+                 add_cls: bool = True, unpack: bool = False):
         """
         convert molecules to tuple of:
             atoms vector with atomic numbers + 2,
             neighbors vector with connected neighbored atoms count including implicit hydrogens count shifted by 2,
             distance matrix with the shortest paths between atoms shifted by 2.
 
         Note: atoms shifted to differentiate from padding equal to zero, special cls token equal to 1, and reserved MLM
@@ -67,22 +68,26 @@
               neighbors shifted to differentiate from padding equal to zero and reserved MLM task token equal to 1.
               distances shifted to differentiate from padding equal to zero and from special distance equal to 1
               that code unreachable atoms (e.g. salts).
 
         :param molecules: map-like molecules collection
         :param distance_cutoff: set distances greater than cutoff to cutoff value
         :param add_cls: add special token at first position
+        :param unpack: unpack molecules
         """
         self.molecules = molecules
         self.distance_cutoff = distance_cutoff
         self.add_cls = add_cls
+        self.unpack = unpack
 
     def __getitem__(self, item: int) -> Tuple[TensorType['tokens', int], TensorType['tokens', int],
                                               TensorType['tokens', 'tokens', int]]:
         mol = self.molecules[item]
+        if self.unpack:
+            mol = MoleculeContainer.unpack(mol)
         if self.add_cls:
             atoms = t_ones(len(mol) + 1, dtype=int32)  # cls token = 1
             neighbors = zeros(len(mol) + 1, dtype=int32)  # cls centrality-encoder disabled by padding trick
         else:
             atoms = IntTensor(len(mol))
             neighbors = IntTensor(len(mol))
```

## chytorch/utils/data/reaction.py

```diff
@@ -18,15 +18,15 @@
 #
 from chython import ReactionContainer
 from itertools import chain, repeat
 from torch import IntTensor, cat, zeros, int32, Size
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
 from torchtyping import TensorType
-from typing import Sequence, Tuple
+from typing import Sequence, Tuple, Union
 from .molecule import MoleculeDataset
 
 
 def collate_reactions(batch) -> Tuple[TensorType['batch', 'tokens', int],
                                       TensorType['batch', 'tokens', int],
                                       TensorType['batch', 'tokens', 'tokens', int],
                                       TensorType['batch', 'tokens', int]]:
@@ -51,32 +51,36 @@
         tmp[n, :s, :s] = d
     return pa, pad_sequence(neighbors, True), tmp, pad_sequence(roles, True)
 
 
 class ReactionDataset(Dataset):
     __slots__ = ('reactions', 'distance_cutoff', 'add_cls')
 
-    def __init__(self, reactions: Sequence[ReactionContainer], *, distance_cutoff: int = 8, add_cls: bool = True):
+    def __init__(self, reactions: Sequence[Union[ReactionContainer, bytes]], *, distance_cutoff: int = 10,
+                 add_cls: bool = True, unpack: bool = False):
         """
         convert reactions to tuple of:
             atoms, neighbors and distances tensors similar to molecule dataset.
              distances - merged molecular distances matrices filled by zero for isolating attention.
             roles: 2 reactants, 3 products, 0 padding, 1 cls token.
 
         :param reactions: map-like reactions collection
         :param distance_cutoff: set distances greater than cutoff to cutoff value
         :param add_cls: add special token at first position of each molecule
         """
         self.reactions = reactions
         self.distance_cutoff = distance_cutoff
         self.add_cls = add_cls
+        self.unpack = unpack
 
     def __getitem__(self, item: int) -> Tuple[TensorType['tokens', int], TensorType['tokens', int],
                                               TensorType['tokens', 'tokens', int], TensorType['tokens', int]]:
         rxn = self.reactions[item]
+        if self.unpack:
+            rxn = ReactionContainer.unpack(rxn)
         molecules = MoleculeDataset(rxn.reactants + rxn.products,
                                     distance_cutoff=self.distance_cutoff, add_cls=self.add_cls)
 
         if self.add_cls:
             # disable rxn cls in molecules encoder
             atoms, neighbors, roles = [IntTensor([0])], [IntTensor([0])], [1]
         else:
```

## Comparing `chytorch-1.5.dist-info/LICENSE` & `chytorch-1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `chytorch-1.5.dist-info/METADATA` & `chytorch-1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chytorch
-Version: 1.5
+Version: 1.7
 Summary: UNKNOWN
 Home-page: https://github.com/chython/chytorch
 Author: Dr. Ramil Nugmanov
 Author-email: nougmanoff@protonmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Plugins
```

## Comparing `chytorch-1.5.dist-info/RECORD` & `chytorch-1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 chytorch/nn/__init__.py,sha256=gjDSsvDlLNYwHIEGZiw00Yeht_1tJ-nLtFE_cUmrS4M,1020
 chytorch/nn/activation.py,sha256=-0xNJstrD72otCzhkCRjjtWSBA_qb2b03WjXnXSgmW0,1182
 chytorch/nn/functional.py,sha256=qSYYNxBebokrwnwWCmjBkaylQQVTqp0KxZMShzQw7kQ,2039
 chytorch/nn/molecule.py,sha256=iCy56MiJrqT9nawdT88jjon2meB4iOVj3MvBfv15NU8,4000
 chytorch/nn/reaction.py,sha256=pXdaqUYxJlcOYEb8kOx0c2eGbRVYLOUbP_mt7FMn6T0,4358
 chytorch/nn/transformer.py,sha256=CcZTyKH7wAox8BZE7vuEQNZGQZP-_UOD7sFQJ5UiHAg,2861
-chytorch/nn/voting.py,sha256=jvO2BbU2l9eOAr8KM6THPThIidp1CT0aDyU6lTI7wfs,3963
+chytorch/nn/voting.py,sha256=IA1gbQzO11nKNrrRl0T082d5QlEkxzXDjdhUWgrdNJk,4095
 chytorch/optim/__init__.py,sha256=AxnMY2O1ttHlBTvY_R2WvY1RJHu4UuJOahA1zF0LhT0,803
-chytorch/optim/lr_scheduler.py,sha256=gHfP4GwZcr9P0WLJX7XvS1vjM7kICZzyZ-ZnH4udYmA,3074
+chytorch/optim/lr_scheduler.py,sha256=nl_-HPvHdGOP00PeNJoUGrvUCMrp88VL-kr8sTEGqW8,2697
 chytorch/utils/__init__.py,sha256=AxnMY2O1ttHlBTvY_R2WvY1RJHu4UuJOahA1zF0LhT0,803
 chytorch/utils/cache.py,sha256=feVYZmNuKBikXYpek2z767fo8FD2w_GX-vbUS9bSVvk,3996
-chytorch/utils/data/__init__.py,sha256=XxELEaTHMNPLukygYx2XBY3A29n6E0AhoUsL-1D1YAM,1261
-chytorch/utils/data/molecule.py,sha256=AK-LZ2R1uyHIi_-598HxSkZu5pSd5o8W8dmV1QXgXek,4832
-chytorch/utils/data/reaction.py,sha256=fT0hI_MjNgu8aieyJF6GEXcfPwjzyhcIGh2-4V29ZOY,4688
+chytorch/utils/data/__init__.py,sha256=p2Y4aJk8TkaV7rkyok2SjybpSjUCpaizX6UbhOIdL8A,1771
+chytorch/utils/data/molecule.py,sha256=lV4IRhFo-jmmXaHDZt-2CDf3XidrxG7-gXEn_V89HFE,5039
+chytorch/utils/data/reaction.py,sha256=HHvflUVXurZnR18aWJrGWX-ToUhDy8pgsSK4wtwmszo,4854
 chytorch/zoo/README.md,sha256=-_xHJDX80-Ye9Dkkb-URDNXY4FW5wkiabh382NDx0FY,84
-chytorch-1.5.dist-info/LICENSE,sha256=fTqV5eBpeAZO0_jit8j4Ref9ikBSlHJ8xwj5TLg7gFk,7817
-chytorch-1.5.dist-info/METADATA,sha256=YeVVK6P4rhjrOk7BErQxFnf7z9gjnwEvYu1lD_eIYsc,4496
-chytorch-1.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-chytorch-1.5.dist-info/top_level.txt,sha256=c84VLlDcP6BYx-vXkJo-u3v3pGq0Fy4T_vAF9mACFsc,9
-chytorch-1.5.dist-info/RECORD,,
+chytorch-1.7.dist-info/LICENSE,sha256=fTqV5eBpeAZO0_jit8j4Ref9ikBSlHJ8xwj5TLg7gFk,7817
+chytorch-1.7.dist-info/METADATA,sha256=cFAyMmkHkBzbSd1PCGT9QcxhRy4_YTg9KzqZ9Lsw3ws,4496
+chytorch-1.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+chytorch-1.7.dist-info/top_level.txt,sha256=c84VLlDcP6BYx-vXkJo-u3v3pGq0Fy4T_vAF9mACFsc,9
+chytorch-1.7.dist-info/RECORD,,
```

