# centernet_resnet101

---

model-name: centernet_resnet101

backbone-name: centernet_resnet101

module-type: cv

fine-tunable: True

model-version: 1.9

train-dataset: coco2017

evaluation: mAP34.4 | AP50acc52.4 | AP75acc36.4

author: MindSpore team

update-time: 2022-10-12

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/research/cv/centernet_resnet101>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/centernetresnet101_ascend_v190_coco2017_research_cv_mAP34.4_AP50acc52.4_AP75acc36.4.ckpt>
    asset-sha256: 0c4ea47862785b87e81333c728a268344dd5196b3d7c1d357902136bdd8917be

license: Apache2.0

summary: centernet_resnet101 is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of centernet_resnet101 from the MindSpore model zoo on Gitee at research/cv/centernet_resnet101.

centernet_resnet101 is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/centernet_resnet101](https://gitee.com/mindspore/models/blob/r1.9/research/cv/centernet_resnet101/README.md).

All parameters in the module are trainable.

## Citation

[Objects as Points](https://arxiv.org/pdf/1904.07850.pdf)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
