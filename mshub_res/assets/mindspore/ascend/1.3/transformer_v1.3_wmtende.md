# transformer

---

model-name: transformer_large

backbone-name: transformer

module-type: nlp

fine-tunable: True

input-shape: [227, 227, 3]

model-version: 1.3

train-dataset: wmtende

accuracy: 27.21

author: MindSpore team

update-time: 2021-09-27

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.3/model_zoo/official/nlp/transformer>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.3

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.3/transformer_ascend_v130_wmtende_official_nlp_bs96_acc27.21/transformer_ascend_v130_wmtende_official_nlp_bs96_acc27.21.ckpt>
    asset-sha256: b322b9e912295d6f6dae34381488c8fa8676fd4759aae178f77b05acebb3dc0f

license: Apache2.0

summary: transformer is used for nlp

---

## Introduction

This MindSpore Hub model uses the implementation of transformer from the MindSpore model zoo on Gitee at model_zoo/official/nlp/transformer.

transformer is a nlp network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/nlp/transformer](https://gitee.com/mindspore/mindspore/blob/r1.3/model_zoo/official/nlp/transformer/README.md).

All parameters in the module are trainable.

## Usage

```python
import mindspore
import mindspore_hub as mshub
from mindspore import Tensor
from mindspore import nn
from mindspore import context
from mindspore.train.model import Model
from mindspore.common import dtype as mstype
from mindspore.dataset.transforms import py_transforms

context.set_context(mode=context.GRAPH_MODE,
                    device_target="Ascend",
                    device_id=0)

model = "mindspore/ascend/1.3/transformer_v1.3_wmtende"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Ashish Vaswani, Noam Shazeer, Niki Parmar, JakobUszkoreit, Llion Jones, Aidan N Gomez, Ł ukaszKaiser, and Illia Polosukhin. 2017. Attention is all you need. In NIPS 2017, pages 5998–6008.