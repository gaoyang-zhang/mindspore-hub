# vgg19

---

model-name: vgg19

backbone-name: vgg19

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: 1.2

train-dataset: imagenet2012

accuracy: 74

author: MindSpore team

update-time: 2021-09-14

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.2/model_zoo/research/cv/vgg19>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.2

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.2/vgg19_ascend_v120_imagenet2012_research_cv_bs64_acc74/vgg19_ascend_v120_imagenet2012_research_cv_bs64_acc74.ckpt>
    asset-sha256: 9aa700f673e586aeded8580ab14eb067b2686e8e1677892fb36b83858d7bb86a

license: Apache2.0

summary: vgg19 is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of vgg19 from the MindSpore model zoo on Gitee at model_zoo/research/cv/vgg19.

vgg19 is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/research/cv/vgg19](https://gitee.com/mindspore/mindspore/blob/r1.2/model_zoo/research/cv/vgg19/README_CN.md).

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

model = "mindspore/ascend/1.2/vgg19_v1.2_imagenet2012"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model, num_classes=1000, dataset="imagenet2012")
network.set_train(False)

# ...
```

## Citation

1. Simonyan K, zisserman A. Very Deep Convolutional Networks for Large-Scale Image Recognition[J]. arXiv preprint arXiv:1409.1556, 2014.