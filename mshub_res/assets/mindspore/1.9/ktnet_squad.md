# ktnet

---

model-name: ktnet

backbone-name: ktnet

module-type: nlp

fine-tunable: True

model-version: 1.9

train-dataset: SQuAD1.1

evaluation: F1score91.0

author: MindSpore team

update-time: 2022-10-12

repo-link: <https://gitee.com/mindspore/models/tree/r1.9/research/nlp/ktnet>

user-id: MindSpore

used-for: inference

mindspore-version: 1.9

asset:

-
    file-format: ckpt
    asset-link: <https://download.mindspore.cn/models/r1.9/ktnet_ascend_v190_squad_research_nlp_F1score91.0.ckpt>
    asset-sha256: f430fa39810a30be45b5f410358580dd729f7e06b43037c57588dfafc0bcc3ca

license: Apache2.0

summary: ktnet is used for nlp

---

## Introduction

This MindSpore Hub model uses the implementation of ktnet from the MindSpore model zoo on Gitee at research/nlp/ktnet.

ktnet is a nlp network. More details please refer to the MindSpore model zoo on Gitee at [research/nlp/ktnet](https://gitee.com/mindspore/models/blob/r1.9/research/nlp/ktnet/README.md).

All parameters in the module are trainable.

## Citation

[Enhancing Pre-Trained Language Representations with Rich Knowledge for Machine Reading Comprehension](https://aclanthology.org/P19-1226.pdf)

## Disclaimer

MindSpore ("we") do not own any ownership or intellectual property rights of the datasets, and the trained models are provided on an "as is" and "as available" basis. We make no representations or warranties of any kind of the datasets and trained models (collectively, “materials”) and will not be liable for any loss, damage, expense or cost arising from the materials. Please ensure that you have permission to use the dataset under the appropriate license for the dataset and in accordance with the terms of the relevant license agreement. The trained models provided are only for research and education purposes.

To Dataset Owners: If you do not wish to have a dataset included in MindSpore, or wish to update it in any way, we will remove or update the content at your request. Please contact us through GitHub or Gitee. Your understanding and contributions to the community are greatly appreciated.

MindSpore is available under the Apache 2.0 license, please see the LICENSE file.
