# hypertext

---

model-name: hypertext

backbone-name: hypertext

module-type: nlp

fine-tunable: True

model-version: 1.9

train-dataset: IFLYTEK

evaluation: acc57.78

author: MindSpore team

update-time: 2022-10-12

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/research/nlp/hypertext>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/hypertext_ascend_v190_iflytek_research_nlp_acc57.78.ckpt>
    asset-sha256: 88c270a0af745744466433dcabd21e1b33c017817428645aa263d460a3830f3c

license: Apache2.0

summary: hypertext is used for nlp

---

## Introduction

This MindSpore Hub model uses the implementation of hypertext from the MindSpore model zoo on Gitee at research/nlp/hypertext.

hypertext is a nlp network. More details please refer to the MindSpore model zoo on Gitee at [research/nlp/hypertext](https://gitee.com/mindspore/models/blob/r1.9/research/nlp/hypertext/README_CN.md).

All parameters in the module are trainable.

## Citation

[HyperText: Endowing FastText with Hyperbolic Geometry](https://arxiv.org/pdf/2010.16143.pdf)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
