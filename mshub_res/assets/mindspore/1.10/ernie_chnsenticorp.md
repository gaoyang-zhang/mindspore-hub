# ernie

---

model-name: ernie

backbone-name: ernie

module-type: nlp

fine-tunable: True

model-version: 1.10

train-dataset: chnsenticorp

evaluation: acc95.83

author: MindSpore team

update-time: 2023-2-17

repo-link: <https://gitee.com/mindspore/models/tree/r1.10/official/nlp/ernie>

user-id: MindSpore

used-for: inference

mindspore-version: 1.10

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.10/ernie_ascend_v1100_chnsenticorp_official_nlp_acc95.83.ckpt>
    asset-sha256: e8301bb372775bd363b1f868af28209e328e4327f15c2d1fcbb56260c31c404b

license: Apache2.0

summary: ernie is used for nlp

---

## Introduction

This MindSpore Hub model uses the implementation of ernie from the MindSpore model zoo on Gitee at official/nlp/ernie.

ernie is a nlp network. More details please refer to the MindSpore model zoo on Gitee at [official/nlp/ernie](https://gitee.com/mindspore/models/blob/r1.10/official/nlp/ernie/README_CN.md).

All parameters in the module are trainable.

## Citation

[ERNIE: Enhanced Representation through Knowledge Integration](https://arxiv.org/pdf/1904.09223.pdf)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
