# GENet_Res50

---

model-name: GENet_Res50

backbone-name: GENet_Res50

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: 1.2

train-dataset: imagenet2012

accuracy: 78.4

author: MindSpore team

update-time: 2021-09-14

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.2/model_zoo/research/cv/GENet_Res50>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.2

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.2/genetres50_plus_ascend_v120_imagenet2012_research_cv_bs256_top1acc78.4__top5acc94.14/genetres50_plus_ascend_v120_imagenet2012_research_cv_bs256_top1acc78.4__top5acc94.14.ckpt>
    asset-sha256: 407565a9b390e6daded58219afccc2352ecde06ce4dc4a4b89e3b9ae95030e53

license: Apache2.0

summary: GENet_Res50 is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of GENet_Res50 from the MindSpore model zoo on Gitee at model_zoo/research/cv/GENet_Res50.

GENet_Res50 is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/research/cv/GENet_Res50](https://gitee.com/mindspore/mindspore/blob/r1.2/model_zoo/research/cv/GENet_Res50/README_CN.md).

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

model = "mindspore/ascend/1.2/genetres50_plus_v1.2_imagenet2012"
# initialize the number of classes based on the pre-trained model
# extra: whether to use Depth-wise conv to down sample
mlp = "True"
# mlp: bottleneck whether to use 1*1 conv.
extra = "True"
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Jie Hu, Li Shen, Samuel Albanie, Gang Sun, Andrea Vedaldi. Gather-Excite: Exploiting Feature Context in Convolutional Neural Networks