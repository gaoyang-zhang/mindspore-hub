# RefineDet

---

model-name: RefineDet

backbone-name: RefineDet

module-type: cv

fine-tunable: True

model-version: 1.9

train-dataset: coco2017

evaluation: acc28.69

author: MindSpore team

update-time: 2022-10-11

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/research/cv/RefineDet>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/refinedet_ascend_v190_coco2017_research_cv_acc28.69.ckpt>
    asset-sha256: 5df4c0602071678957f0039520cde9ebb995f7c2bbadddc817694a02582c4531

license: Apache2.0

summary: RefineDet is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of RefineDet from the MindSpore model zoo on Gitee at research/cv/RefineDet.

RefineDet is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/RefineDet](https://gitee.com/mindspore/models/blob/r1.9/research/cv/RefineDet/README_CN.md).

All parameters in the module are trainable.

## Citation

[Single-Shot Refinement Neural Network for Object Detection](https://arxiv.org/pdf/1711.06897.pdf)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
