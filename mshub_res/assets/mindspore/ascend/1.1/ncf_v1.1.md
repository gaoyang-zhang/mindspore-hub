# NCF

---

model-name: ncf

backbone-name: ncf

module-type: recommend

fine-tunable: True

input-shape: [[1, 128], [1, 128], [1, 128]]

model-version: 1.1

train-dataset: ml-1m

author: MindSpore team

update-time: 2021-04-15

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.1/model_zoo/official/recommend/ncf>

user-id: MindSpore

used-for: inference/transfer-learning

train-backend: ascend

infer-backend: ascend

mindspore-version: 1.1

asset:

  -
    file-format: ckpt  
    asset-link: <https://download.mindspore.cn/model_zoo/r1.1/ncf_ascend_v111_movilens_offical_recommend_bs256_hr69/ncf_ascend_v111_movilens_offical_recommend_bs256_hr69.ckpt>
    asset-sha256: addbaf8a7e302231c1ec091140d26692a48b5ff9dc309f9a6d26f3d2c5f4740a

license: Apache2.0

summary: bert_base used to do classification, sequence labeling or squad tasks on various dataset.

---

## Introduction

This MindSpore Hub model uses the implementation of ncf from the MindSpore model zoo on Gitee at model_zoo/official/recommend/ncf.

ncf is a audio network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/recommend/ncf](https://gitee.com/mindspore/mindspore/blob/r1.1/model_zoo/official/recommend/ncf/README.md).

All parameters in the module are trainable.

## Usage

```python
import mindspore_hub as mshub
import mindspore
from mindspore import context, Tensor, nn
from mindspore.train.model import Model
from mindspore.common import dtype as mstype
from mindspore.dataset.transforms import py_transforms

context.set_context(mode=context.GRAPH_MODE,
                    device_target="Ascend",
                    device_id=0)

model = "mindspore/ascend/1.1/ncf_v1.1"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model, num_users=6040, num_items=3706, num_factors=16,
                     model_layers=[64, 32, 16], mf_regularization=0,
                     mlp_reg_layers=[0.0, 0.0, 0.0, 0.0], mf_dim=16)
network.set_train(False)

# Use as the same as MindSpore Model to inference.
# ...
```

## Citation

Paper: Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova. BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding. arXiv preprint arXiv:1810.04805.