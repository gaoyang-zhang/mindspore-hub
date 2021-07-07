# xception

---

model-name: xception

backbone-name: xception

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: v1.2

train-dataset: imagenet2012

accuracy: 79

author: MindSpore team

update-time: 2021-06-29

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.2/model_zoo/official/cv/xception>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.2

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.2/xception_ascend_v120_imagenet2012_official_cv_bs128_top1acc79_top5acc94/xception_ascend_v120_imagenet2012_official_cv_bs128_top1acc79_top5acc94.ckpt>
    asset-sha256: 0359d9ffe399d2c359bf7cf488b56f559e665dc5968b61a00809c8a0a53fb26c

license: Apache2.0

summary: xception is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of xception from the MindSpore model zoo on Gitee at model_zoo/official/cv/xception.

xception is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/cv/xception](https://gitee.com/mindspore/mindspore/blob/r1.2/model_zoo/official/cv/xception/README.md).

All parameters in the module are trainable.

## Usage

```python
import mindspore_hub as mshub
from mindspore import context

context.set_context(mode=context.GRAPH_MODE,
                    device_target="Ascend",
                    device_id=0)

model = "mindspore/ascend/1.2/xception_v1.2_imagenet2012"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Franois Chollet. Xception: Deep Learning with Depthwise Separable Convolutions. 2017 IEEE Conference on Computer Vision and Pattern Recognition (CVPR