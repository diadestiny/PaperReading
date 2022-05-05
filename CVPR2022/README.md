# CVPR2022



## 去雨Derain

1. **Towards Robust Rain Removal Against Adversarial Attacks: A Comprehensive Benchmark Analysis and Beyond** [paper](https://arxiv.org/abs/2203.16931) | [code](https://github.com/yuyi-sd/Robust_Rain_Removal)

   author: Yi Yu, Wenhang Yang, Yap-Peng Tan, Alex C. Kot Nanyang Technological University

   > This paper makes the first attempt to **conduct a comprehensive study on the robustness of deep learning-based rain removal methods against adversarial attacks**. 
   >
   > Our study shows that, when the image/video is highly degraded, rain removal methods **are more vulnerable to the adversarial attacks as small distortions/perturbations** become less noticeable or detectable.
   >
   > In this paper, we first present a comprehensive empirical evaluation of various methods **at different levels of attacks and with various losses/targets to generate the perturbations** from the perspective of human perception and machine analysis tasks. 
   >
   > A systematic evaluation of key modules in existing methods is performed in terms of their robustness against adversarial attacks. From the insights of our analysis, we construct **a more robust deraining method by integrating these effective modules**. 
   >
   > Finally, we examine various types of adversarial attacks that are specific to deraining problems and their effects on both human and machine vision tasks, including 1) rain region attacks, adding perturbations only in the rain regions to make the perturbations in the attacked rain images less visible; 2) object-sensitive attacks, adding perturbations only in regions near the given objects.

2. **Unpaired Deep Image Deraining Using Dual Contrastive Learning** [paper](https://arxiv.org/abs/2109.02973) | [code](https://cxtalk.github.io/projects/DCD-GAN.html)

   author: Xiang Chen, Jinshan Pan, Kui Jiang et al. Nanjing University of Science and Technology

   > Moreover, simply using existing unpaired learning methods (e.g., unpaired adversarial learning and cycle-consistency constraints) in the SID task is insufficient to learn the underlying relationship from rainy inputs to clean outputs as there exists significant domain gap between the rainy and clean images. 
   >
   > In this paper, we develop **an effective unpaired SID adversarial framework which explores mutual properties of the unpaired exemplars by a dual contrastive learning manner in a deep feature space**, named as DCDGAN. 
   >
   > The proposed method mainly consists of two cooperative branches: Bidirectional Translation Branch (BTB) and Contrastive Guidance Branch (CGB). 
   >
   > Specifically, BTB exploits full advantage of the circulatory architecture of adversarial consistency to generate abundant exemplar pairs and excavates latent feature distributions between two domains by equipping it with bidirectional mapping. 
   >
   > Simultaneously, CGB implicitly constrains the embeddings of different exemplars in the deep feature space by encouraging the similar feature distributions closer while pushing the dissimilar further away, in order to better facilitate rain removal and help image restoration. 

![image-20220505160013287](../screenshot/DCD-GAN.png)

## 图像复原Image Restoration

1. **TransWeather: Transformer-based Restoration of Images Degraded by Adverse Weather Conditions** [paper](https://arxiv.org/abs/2111.14813) | [code](https://github.com/jeya-maria-jose/TransWeather)

   authors: Jeya Maria Jose Valanarasu, Rajeev Yasarla and Vishal M. Patel. Johns Hopkins University

   > Most methods proposed in the literature have been designed to deal with just removing one type of degradation. 
   >
   > In this work, we focus on developing an efficient solution for the all adverse weather removal problem. To this end, we propose TransWeather, **a transformer-based end-to-end model with just a single encoder and a decoder that can restore an image degraded by any weather condition**. 
   >
   > Specifically, we utilize a novel transformer encoder using intra-patch transformer blocks to enhance attention inside the patches to effectively remove smaller weather degradations. 
   >
   > We also introduce a transformer decoder with learnable weather type embeddings to adjust to the weather degradation at hand. 

   ![image-20220505160013287](../screenshot/TransWeather.png)

2. **Deep Generalized Unfolding Networks for Image Restoration**  [paper](https://arxiv.org/abs/2204.13348) | [code](https://github.com/MC-E/Deep-Generalized-Unfolding-Networks-for-Image-Restoration)

   authors: Chong Mou, Qian Wang, Jian Zhang PKUSZ

   >However, most DNN methods are designed as a black box, lacking transparency and interpretability.
   >
   >In this paper, we propose a Deep Generalized Unfolding Network (DGUNet) for image restoration. Concretely, **without loss of interpretability**, we **integrate a gradient estimation strategy into the gradient descent step of the Proximal Gradient Descent (PGD) algorithm**, driving it to deal with complex and real-world image degradation. 
   >
   >In addition, we design inter-stage information pathways across proximal mapping in different PGD iterations to rectify the intrinsic information loss in most deep unfolding networks (DUN) through a multi-scale and spatial-adaptive way. 
   >
   >By integrating the flexible gradient descent and informative proximal mapping, we unfold the iterative PGD algorithm into a trainable DNN. 

![image-20220505155755568](../screenshot/DGUNet.png)

# 增量学习 Incremental Learning

**1. An Efficient Domain-Incremental Learning Approach to Drive in All Weather Conditions**  [paper](https://arxiv.org/abs/2204.08817) 

author: M. Jehanzeb Mirza, Marc Masana, Horst Possegger, Horst Bischof. Institute of Computer Graphics and Vision, Graz University of Technology

> When adapting these models for changed environments, such as different weather conditions, they are prone to **forgetting previously learned information**. 
>
> This catastrophic forgetting is typically addressed via **incremental learning** approaches which usually re-train the model by either keeping a memory bank of training samples or keeping a copy of the entire model or model parameters for each scenario. 
>
> While these approaches show impressive results, they can be prone to scalability issues and their applicability for autonomous driving in all weather conditions has not been shown.
>
> In this paper we propose DISC -- **Domain Incremental through Statistical Correction** -- a simple online zero-forgetting approach which can incrementally learn new tasks (i.e weather conditions) without requiring re-training or expensive memory banks. 
>
> The only information we store for each task are the statistical parameters as we categorize each domain by the change in first and second order statistics. Thus, as each task arrives, we simply 'plug and play' the statistical vectors for the corresponding task into the model and it immediately starts to perform well on that task. 

![image-20220505155755568](../screenshot/DISC.png)