# TNT

---

model-name: TNT

backbone-name: TNT

module-type: cv

fine-tunable: True

model-version: 1.3

train-dataset: imagenet2012

evaluation: top1acc81.03 | top5acc95.41

author: MindSpore team

update-time: 2022-04-18

repo-link: <https://gitee.com/mindspore/models/tree/r1.3/research/cv/TNT>

user-id: MindSpore

used-for: inference

mindspore-version: 1.3

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.3/tnt_ascend_v130_imagenet2012_research_cv_top1acc81.03_top5acc95.41.ckpt>
    asset-sha256: 028493c50c666b32c37a036c217c0416a81cc822c591a6662f7136606d66b38d

license: Apache2.0

summary: TNT is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of TNT from the MindSpore model zoo on Gitee at research/cv/TNT.

TNT is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/TNT](https://gitee.com/mindspore/models/blob/r1.3/research/cv/TNT/README_CN.md).

All parameters in the module are trainable.

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
