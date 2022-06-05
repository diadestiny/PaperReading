# Object Detection 目标检测

## Transformer

1. **(DETR)End-to-End Object Detection with Transformers** [paper](https://arxiv.org/abs/2005.12872) | [code](https://github.com/facebookresearch/detr) *ECCV2020*

   author: Nicolas Carion, Francisco Massa, Gabriel Synnaeve et al. Facebook AI

   > 结合CNN+**纯Transformer结构**，利用二分图匹配匈牙利算法计算loss，采用**序列预测**(set prediction)方式，摒弃proposal、anchor、nms等检测设计。

   ![image-20220605172510134](../screenshot/DETR.png)