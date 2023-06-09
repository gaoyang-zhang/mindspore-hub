# advanced_east

---

model-name: advanced_east

backbone-name: advanced_east

module-type: cv

fine-tunable: True

model-version: 1.3

train-dataset: icpr2018

evaluation: F1acc61.52

author: MindSpore team

update-time: 2022-03-23

repo-link: <https://gitee.com/mindspore/models/tree/r1.3/research/cv/advanced_east>

user-id: MindSpore

used-for: inference

mindspore-version: 1.3

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.3/advancedeast_ascend_v130_icpr2018_research_cv_F1acc61.52.ckpt>
    asset-sha256: 29da691de69194138d3ab0f74ae62299cff4e3d7432e6e511f70706c238edc9e

license: Apache2.0

summary: advanced_east is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of advanced_east from the MindSpore model zoo on Gitee at research/cv/advanced_east.

advanced_east is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/advanced_east](https://gitee.com/mindspore/models/blob/r1.3/research/cv/advanced_east/README.md).

All parameters in the module are trainable.

## Citation

EAST:An Efficient and Accurate Scene Text Detector.

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
