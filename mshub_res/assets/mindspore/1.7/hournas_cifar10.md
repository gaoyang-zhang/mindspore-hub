# HourNAS

---

model-name: HourNAS

backbone-name: HourNAS

module-type: cv

fine-tunable: True

model-version: 1.7

train-dataset: cifar10

evaluation: top1acc96.1

author: MindSpore team

update-time: 2022-06-22

repo-link: <https://gitee.com/mindspore/models/tree/r1.7/research/cv/HourNAS>

user-id: MindSpore

used-for: inference

mindspore-version: 1.7

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.7/hournas_ascend_v170_cifar10_research_cv_top1acc96.1.ckpt>
    asset-sha256: 2ce9cb49fd381a3a2d51a7f5b29e2039a00e178e1ec119d4505b0ed671379663

license: Apache2.0

summary: HourNAS is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of HourNAS from the MindSpore model zoo on Gitee at research/cv/HourNAS.

HourNAS is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/HourNAS](https://gitee.com/mindspore/models/blob/r1.7/research/cv/HourNAS/README.md).

All parameters in the module are trainable.

## Citation

Zhaohui Yang, Yunhe Wang, Xinghao Chen, Jianyuan Guo, Wei Zhang, Chao Xu, Chunjing Xu, Dacheng Tao, Chang Xu. HourNAS: Extremely Fast Neural Architecture Search Through an Hourglass Lens. In CVPR 2021.

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
