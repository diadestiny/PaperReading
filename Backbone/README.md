# Backbone Design 架构设计

1. **EfficientFormer: Vision Transformers at MobileNet** [paper](https://arxiv.org/abs/2206.01191) | [code](https://github.com/snap-research/efficientformer)  *arxiv 2022*

   author: Yanyu Li, Geng Yuan, Yang Wen et al. Snap Inc, Northeastern University

   > 1. propose a new **dimension-consistent design paradigm for vision transformers** which splits the network into a 4D partition where operators are implemented in CONV-net style (MB4*D*), and a 3D partition where linear projections and attentions are performed over 3D tensor to enjoy the global modeling power of MHSA without sacrificing efficiency (MB3*D*)
   >
   > 2. Observation:
   >
   >    (1) *Patch embedding with large kernel and stride is a speed bottleneck on mobile devices*
   >
   >    (2) *Consistent feature dimension is important for the choice of token mixer. MHSA is not necessarily a speed bottleneck* **(摒弃Reshape operations)**

   ![image-20220605202855056](../screenshot/EfficientFormer.png)