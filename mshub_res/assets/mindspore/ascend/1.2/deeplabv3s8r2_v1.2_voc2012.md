# deeplabv3

---

model-name: deeplabv3

backbone-name: deeplabv3

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: v1.2

train-dataset: voc2012

accuracy: 79

author: MindSpore team

update-time: 2021-06-29

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.2/model_zoo/official/cv/deeplabv3>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.2

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.2/deeplabv3s8r2_ascend_v120_voc2012_official_cv_bs16_s8acc79/deeplabv3s8r2_ascend_v120_voc2012_official_cv_bs16_s8acc79.ckpt>
    asset-sha256: 5e95788d5c3b96899bf255daf4d5ce322089a1fac1c69a3709e3ee89a7f06edd

license: Apache2.0

summary: deeplabv3 is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of deeplabv3 from the MindSpore model zoo on Gitee at model_zoo/official/cv/deeplabv3.

deeplabv3 is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/cv/deeplabv3](https://gitee.com/mindspore/mindspore/blob/r1.2/model_zoo/official/cv/deeplabv3/README.md).

All parameters in the module are trainable.

## Usage

```python
import mindspore_hub as mshub
from mindspore import context

context.set_context(mode=context.GRAPH_MODE,
                    device_target="Ascend",
                    device_id=0)

model = "mindspore/ascend/1.2/deeplabv3s8r2_v1.2_voc2012"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model, num_classes=21)
network.set_train(False)

# ...
```

## Citation

1. Chen L C, Papandreou G, Schroff F, et al. Rethinking atrous convolution for semantic image segmentation[J]. arXiv preprint arXiv:1706.05587, 2017.