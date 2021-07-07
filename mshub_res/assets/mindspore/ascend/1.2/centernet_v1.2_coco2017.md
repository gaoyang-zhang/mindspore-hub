# centernet

---

model-name: centernet

backbone-name: centernet

module-type: cv

fine-tunable: True

input-shape: [227, 227, 3]

model-version: v1.2

train-dataset: coco2017

accuracy: 51

author: MindSpore team

update-time: 2021-06-29

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.2/model_zoo/research/cv/centernet>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.2

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.2/centernet_ascend_v120_coco2017_research_cv_bs32_acc51/centernet_ascend_v120_coco2017_research_cv_bs32_acc51.ckpt>
    asset-sha256: f3bb35082b8c70feed99ce252584a5e30c3fa5400db30d04ee1c52dbbab79423

license: Apache2.0

summary: centernet is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of centernet from the MindSpore model zoo on Gitee at model_zoo/research/cv/centernet.

centernet is a cv network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/research/cv/centernet](https://gitee.com/mindspore/mindspore/blob/r1.2/model_zoo/research/cv/centernet/README.md).

All parameters in the module are trainable.

## Usage

```python
import mindspore_hub as mshub
from mindspore import context

context.set_context(mode=context.GRAPH_MODE,
                    device_target="Ascend",
                    device_id=0)

model = "mindspore/ascend/1.2/centernet_v1.2_coco2017"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Xingyi Zhou(UT Austin) and Dequan Wang(UC Berkeley) and Philipp Krahenbuhl(UT Austin). Objects as Points. 2019.