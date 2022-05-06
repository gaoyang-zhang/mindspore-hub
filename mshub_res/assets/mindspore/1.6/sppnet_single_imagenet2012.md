# SPPNet

---

model-name: SPPNet

backbone-name: SPPNet

module-type: cv

fine-tunable: True

model-version: 1.6

train-dataset: imagenet2012

evaluation: top1acc64.82 | top5acc85.62

author: MindSpore team

update-time: 2022-04-18

repo-link: <https://gitee.com/mindspore/models/tree/r1.6/research/cv/SPPNet>

user-id: MindSpore

used-for: inference

mindspore-version: 1.6

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.6/sppnet_single_ascend_v160_imagenet2012_research_cv_top1acc64.82_top5acc85.62.ckpt>
    asset-sha256: 45f0b67fb099a2247e193f4ff4569de225fd670f5b56b82a0fd184eaf8948616

license: Apache2.0

summary: SPPNet is used for cv

---

## Introduction

This MindSpore Hub model uses the implementation of SPPNet from the MindSpore model zoo on Gitee at research/cv/SPPNet.

SPPNet is a cv network. More details please refer to the MindSpore model zoo on Gitee at [research/cv/SPPNet](https://gitee.com/mindspore/models/blob/r1.6/research/cv/SPPNet/README_CN.md).

All parameters in the module are trainable.

## Citation

K. He, X. Zhang, S. Ren and J. Sun, "Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition," in IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 37, no. 9, pp. 1904-1916, 1 Sept. 2015, doi: 10.1109/TPAMI.2015.2389824.

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.