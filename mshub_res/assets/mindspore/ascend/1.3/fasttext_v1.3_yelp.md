# fasttext

---

model-name: fasttext

backbone-name: fasttext

module-type: nlp

fine-tunable: True

input-shape: [227, 227, 3]

model-version: 1.3

train-dataset: yelp

accuracy: 95

author: MindSpore team

update-time: 2021-09-27

repo-link: <https://gitee.com/mindspore/mindspore/tree/r1.3/model_zoo/official/nlp/fasttext>

user-id: MindSpore

used-for: inference

train-backend: ascend

infer-backend: ascend

mindspore-version: v1.3

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/model_zoo/r1.3/fasttext_ascend_v130_yelp_official_nlp_bs2048_acc95/fasttext_ascend_v130_yelp_official_nlp_bs2048_acc95.ckpt>
    asset-sha256: c6156d218c0e9ee484c273558e709c6f733528b0a14fdefdde1117db4dfe35c0

license: Apache2.0

summary: fasttext is used for nlp

---

## Introduction

This MindSpore Hub model uses the implementation of fasttext from the MindSpore model zoo on Gitee at model_zoo/official/nlp/fasttext.

fasttext is a nlp network. More details please refer to the MindSpore model zoo on Gitee at [model_zoo/official/nlp/fasttext](https://gitee.com/mindspore/mindspore/blob/r1.3/model_zoo/official/nlp/fasttext/README.md).

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

model = "mindspore/ascend/1.3/fasttext_v1.3_yelp"
# initialize the number of classes based on the pre-trained model
network = mshub.load(model)
network.set_train(False)

# ...
```

## Citation

1. Bag of Tricks for Efficient Text Classification, 2016, A. Joulin, E. Grave, P. Bojanowski, and T. Mikolov