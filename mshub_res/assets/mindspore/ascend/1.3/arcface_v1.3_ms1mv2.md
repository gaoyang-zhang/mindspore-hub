# arcface

---

model-name: iresnet100

backbone-name: iresnet100

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: 1.3

train-dataset: ms1mv2

accuracy: 95.06

author: MindSpore team

update-time: 2021-09-29

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.3/model_zoo/research/cv/arcface>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.3

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.3/arcface_ascend_v130_ms1mv2_research_cv_bs64_ijbbacc95.06_ijbcacc96.39/arcface_ascend_v130_ms1mv2_research_cv_bs64_ijbbacc95.06_ijbcacc96.39.ckpt>
    asset-sha256: 5897d6d1b98411e170625377871b1daf658f6ba477765ba3c9872a24097a629f

license: Apache2.0

summary: arcface is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of arcface from the MindSpore model zoo on Gitee at model_zoo/research/cv/arcface.

arcface is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/research/cv/arcface](https://gitee.com/mindspore/mindspore/blob/r1.3/model_zoo/research/cv/arcface/README_CN.md).

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

model = "mindspore/ascend/1.3/arcface_v1.3_ms1mv2"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Deng J ,  Guo J ,  Zafeiriou S . ArcFace: Additive Angular Margin Loss for Deep Face Recognition[J].  2018.