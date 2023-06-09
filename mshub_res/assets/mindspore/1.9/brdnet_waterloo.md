# brdnet

---

model-name: brdnet

backbone-name: brdnet

module-type: cv

fine-tunable: True

model-version: 1.9

train-dataset: waterloo

evaluation: PSNR36.14

author: MindSpore team

update-time: 2022-10-11

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/official/cv/brdnet>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/brdnet_ascend_v190_waterloo_official_cv_PSNR36.14.ckpt>
    asset-sha256: ceb72d439465d2b8b1cbe65dbcf63a1f47755412669128289b92d537ec4893c9

license: Apache2.0

summary: brdnet is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of brdnet from the MindSpore model zoo on Gitee at official/cv/brdnet.

brdnet is a cv network. More details please refer to the MindSpore model zoo on Gitee at [official/cv/brdnet](https://gitee.com/mindspore/models/blob/r1.9/official/cv/brdnet/README_CN.md).

All parameters in the module are trainable.

## Citation

[Image denoising using deep CNN with batch renormalization](https://www.sciencedirect.com/science/article/abs/pii/S0893608019302394)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
