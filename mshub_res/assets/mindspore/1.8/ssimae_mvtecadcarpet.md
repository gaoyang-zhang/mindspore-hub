# ssim-ae

---

model-name: ssim-ae

backbone-name: ssim-ae

module-type: cv

fine-tunable: True

model-version: 1.8

train-dataset: mvtecadcarpet

evaluation: ok98.9 | nok98.9 | avg85.5

author: MindSpore team

update-time: 2022-07-19

repo-link: <https://gitee.com/mindspore/models/tree/r1.8/official/cv/ssim-ae>

user-id: MindSpore

used-for: inference

mindspore-version: 1.8

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.8/ssimae_ascend_v180_mvtecadcarpet_official_cv_ok98.9_nok98.9_avg85.5.ckpt>
    asset-sha256: 5a7c910b586c8f1389d1e1a067694301dae8b3e228d8efe696e469d9f3db0231

license: Apache2.0

summary: ssim-ae is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of ssim-ae from the MindSpore model zoo on Gitee at official/cv/ssim-ae.

ssim-ae is a cv network. More details please refer to the MindSpore model zoo on Gitee at [official/cv/ssim-ae](https://gitee.com/mindspore/models/blob/r1.8/official/cv/ssim-ae/README_CN.md).

All parameters in the module are trainable.

## Citation

Improving Unsupervised Defect Segmentation by Applying Structural Similarity To Autoencoders

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
