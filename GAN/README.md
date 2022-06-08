# GAN生成对抗网络

1. **(PGGAN)Progressive Growing of GANs for Improved Quality, Stability, and Variation** [paper](https://arxiv.org/abs/1710.10196) | [code](https://github.com/tkarras/progressive_growing_of_gans) *ICLR2018*

   author: Tero Karras, Timo Aila, Samuli Laine,et al. NVIDIA

   > 采用渐进训练策略，先训练G和D的低分辨率小尺度层，**采用学习残差方式(保持网络稳定性)**来逐步加入大尺度层。

   ![image-20220608162108032](../screenshot/PGGAN1.png)

![image-20220608162152918](../screenshot/PGGAN2.png)