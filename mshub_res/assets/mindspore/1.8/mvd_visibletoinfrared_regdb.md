# MVD

---

model-name: MVD

backbone-name: MVD

module-type: cv

fine-tunable: True

model-version: 1.8

train-dataset: regdb

evaluation: rank1acc71 | mAP67

author: MindSpore team

update-time: 2022-07-19

repo-link: <https://gitee.com/mindspore/models/tree/r1.8/research/cv/MVD>

user-id: MindSpore

used-for: inference

mindspore-version: 1.8

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.8/mvd_visibletoinfrared_ascend_v180_regdb_research_cv_rank1acc71_mAP67.ckpt>
    asset-sha256: 6540c831b95f05f516ba7a5f13ee4bc2e92a603a1ec0b37e7ba9b37771cd7423

license: Apache2.0

summary: MVD is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of MVD from the MindSpore model zoo on Gitee at research/cv/MVD.

MVD is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/MVD](https://gitee.com/mindspore/models/blob/r1.8/research/cv/MVD/README.md).

All parameters in the module are trainable.

## Citation

Farewell to Mutual Information: Variational Distillation for Cross-Modal Person Re-identification in CVPR 2021

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
