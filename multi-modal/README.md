# multi-modal

## V-L 视觉-语言

1. **(CLIP)Learning Transferable Visual Models From Natural Language Supervision** [paper](https://arxiv.org/abs/2103.00020) | [code](https://github.com/openai/CLIP) *ICML2021*

   author: Alec Radford, Jong Wook Kim, Chris Hallacy, et al.  OpenAI

   > State-of-the-art computer vision systems are trained to predict a fixed set of predetermined object categories. 
   >
   > This restricted form of supervision limits their generality and usability since additional labeled data is needed to specify any other visual concept. 
   >
   > Learning directly from raw text about images is a promising alternative which leverages a much broader source of supervision. 
   >
   > We demonstrate that the simple pre-training task of predicting which caption goes with which image is an efficient and scalable way to learn SOTA image representations from scratch on a dataset of 400 million (image, text) pairs collected from the internet. 
   >
   > After pre-training, natural language is used to reference learned visual concepts (or describe new ones) enabling zero-shot transfer of the model to downstream tasks. 

   ![CLIP](../screenshot/CLIP.png)