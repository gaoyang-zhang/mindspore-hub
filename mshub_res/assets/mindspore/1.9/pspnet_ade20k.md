# PSPNet

---

model-name: PSPNet

backbone-name: PSPNet

module-type: cv

fine-tunable: True

model-version: 1.9

train-dataset: ADE20K

evaluation: mIoU41.71 | allAcc79.86

author: MindSpore team

update-time: 2022-10-11

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/research/cv/PSPNet>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/pspnet_ascend_v190_ade20k_research_cv_mIoU41.71_allAcc79.86.ckpt>
    asset-sha256: 91b0a5bfe5d2d2b9d3685177992f20917440e73199616e928a9146f72e16766c

license: Apache2.0

summary: PSPNet is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of PSPNet from the MindSpore model zoo on Gitee at research/cv/PSPNet.

PSPNet is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/PSPNet](https://gitee.com/mindspore/models/blob/r1.9/research/cv/PSPNet/README.md).

All parameters in the module are trainable.

## Citation

Hengshuang Zhao, Jianping Shi, Xiaojuan Qi, Xiaogang Wang, Jiaya Jia. Pyramid Scene Parsing Network 2017.

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.