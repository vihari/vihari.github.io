---
layout: page
title: Publications
---

### Research Theme
I work on making learning systems robust to changing environments (domain).
Some examples of domain shift are when a self-driving car that is trained to drive on clear days deployed on a rainy day, or when an Automatic Speech Recognition engine trained on native-english speech deployed on foreign speakers. 
My research has three broad themes below. 

* **Domain Generaliation (DG)**: When the target domain is unknown, you prepare for the worst when training on the available source domains. [[ICLR18](#crossgrad)][[ICML20](#csd)][[ICML20a](#dg_for_dr)]
* **Domain Transfer**: If a representative target domain is provided, how best to transfer the knowledge for optimal performance on the target? [[ACL19](#srcsel)]
* **Machine Learning as a Service**: Research challenges abound when serving millions of clients through Prediction APIs. [[NeurIPS21](#accsurf)][[EMNLP20](#topicsig)]

Check [Google Scholar](https://scholar.google.co.in/citations?user=DQddccYAAAAJ) for an exhaustive list of publications.  
<a name="accsurf"></a>
* **Active Assessment of Prediction Services as Accuracy Surface Over Attribute Combinations**.  
  NeurIPS 2021 [[pdf](https://arxiv.org/pdf/2108.06514.pdf)]  
  We argue that Prediction Services should report performance on attribute combinations characterizing a client's utility, and go beyond the leaderboards and standard bechmarks. How can we efficiently estimate performance over combinatorially large attribute combinations and address the corresponding label supervision cost? Check out our paper to know more.      
<a name="topicsig"></a>
* **NLP Service APIs and Models for Efficient Registration of New Clients**.   
  **EMNLP Findings 2020** [[pdf](https://arxiv.org/pdf/2010.01526.pdf)].   
  Prediction service APIs are expected to cater millions of client distributions. Adapting to each client is not scalable for computation and storage concerns. 
  We propose an on-the-fly adaptation technique using client side corpus signature.    
<a name="dg_for_dr"></a>
* **Untapped Potential of Data Augmentation: A Domain Generalization Viewpoint**.   
  **ICML UDL Workshop 2020** [[pdf](https://arxiv.org/abs/2007.04662)][[slides](https://docs.google.com/presentation/d/1IZuAc9GKrB2WO00kWOo1FOMs8sGBWe7XZLrhfZNHAJY/edit?usp=sharing)].       
  We argue why plain augmentation leads to shallow parameter sharing between the original and augmented examples. We show how even the SoTA augmentation methods could still overfit on augmentations and the scope for mitigating this overfit by employing domain generalization techniques.  
<a name="csd"></a>
* **Efficient Domain Generalization via Common-Specific Low-Rank Decomposition.**  
  **ICML 2020** [[pdf](https://arxiv.org/abs/2003.12815)][[code](https://github.com/vihari/CSD/)][[talk](https://icml.cc/virtual/2020/poster/6528)][[slides](https://docs.google.com/presentation/d/1x0MXQrutH1XJunhCPPqaHhWnqn49fZcPyMyJEdGDWv4/edit?usp=sharing)]    
  When a model is trained on multiple sources, the learned parameters are composed of both shared and domain-specific components. 
  While the domain-specific components improve the performance on the seen train domains, they impede generalization to new domains. 
  We propose a method called CSD, as a replacement for the final linear layer, that identifies and removes the specific components, thereby retaining only the components common across all the domains.   Our method is simple, efficient and yet competitive.  
<a name="srcsel"></a>
* **Topic Sensitive Attention on Generic Corpora Corrects Sense Bias in Pretrained Embeddings.**  
  **ACL 2019** [[pdf](https://arxiv.org/abs/1906.02688)][[code](https://github.com/vihari/focussed_embs)][[talk](https://vimeo.com/384490539)][[slides](https://docs.google.com/presentation/d/1cEiov879145R6oOBESjif2PcsNXKljZPORegf6_fEMU/edit?usp=sharing)]  
  We answer three interesting questions about adapting word-embeddings.
  + What is the best way to fintune word-embeddings? Answer: By revisiting the source corpus.
  + Does the pretrained word-embeddings retain information that can enable tuning to any new domain? Answer: No.
  + Are contextual embeddings so rich that they obfuscate the need to adapt embeddings? Answer No.   
<a name="crossgrad"></a>
* **Generalizing across domains via cross-gradient training.**   
  **ICLR 2018** [[pdf](https://arxiv.org/pdf/1804.10745.pdf)][[code](https://github.com/vihari/crossgrad)]   
  We can avoid overfitting on the train domains by hallucinating new unseen domains. We propose CrossGrad that augments label consistent examples from new domains that helps in domain generalization.
