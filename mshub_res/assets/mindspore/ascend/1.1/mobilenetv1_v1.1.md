# MobileNetV1

---

model-name: mobilenetV1

backbone-name: mobilenetV1

module-type: cv-classification

fine-tunable: True

input-shape: [224, 224, 3]

model-version: 1.1

train-dataset: imagenet2012

author: MindSpore team

update-time: 2021-04-15

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.1/model_zoo/official/cv/mobilenetv1>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: 1.1

mindspore-lite: true

asset:

-
    file-format: ckpt  
    asset-link: <https://download.mindspore.cn/model_zoo/r1.1/mobilenetv1_ascend_v111_imagenet2012_offical_cv_bs256_top172/mobilenetv1_ascend_v111_imagenet2012_offical_cv_bs256_top172.ckpt>
    asset-sha256: 4808018371e8322bccc590657c908ee0e10727a00ba0111095ebdcb802bb0e0e

license: Apache2.0

summary: mobilenetv1 used to classify 600 classes of openimage.

---

## Introduction

This MindSpore Hub model uses the implementation of mobilenetv1 from the MindSpore model zoo on Gitee at model_zoo/official/cv/mobilenetv1.

mobilenetv1 is a audio network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/cv/mobilenetv1](https://gitee.com/mindspore/mindspore/blob/r1.1/model_zoo/official/cv/mobilenetv1/README.md).

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

model = "mindspore/ascend/1.1/mobilenetv1_v1.1"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# Use as the same as MindSpore Model to inference.
# ...
```

## Citation

1. Howard, Andrew, Mark Sandler, Grace Chu, Liang-Chieh Chen, Bo Chen, Mingxing Tan, Weijun Wang et al. "Searching for MobileNetV2." In Proceedings of the IEEE International Conference on Computer Vision, pp. 1314-1324. 2019.