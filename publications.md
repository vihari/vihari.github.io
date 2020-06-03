---
layout: page
title: Publications
---

Check [Google Scholar](https://scholar.google.co.in/citations?user=DQddccYAAAAJ) for an exhaustive list of publications.  

* Efficient Domain Generalization via Common-Specific Low-Rank Decomposition.  
  ICML 2020 [[pdf](https://arxiv.org/abs/2003.12815)][[code](https://github.com/vihari/CSD/)]  
  When a model is trained on multiple sources, the learned parameters are composed of both shared and domain-specific components. 
  While the domain-specific components improve the performance on the seen train domains, they impede generalization to new domains. 
  We propose a method called CSD, as a replacement for the final linear layer, that identifies and removes the specific components, thereby retaining only the components common across all the domains.   Our method is simple, efficient and yet is competitive.

* Topic Sensitive Attention on Generic Corpora Corrects Sense Bias in Pretrained Embeddings. 
  ACL 2019 [[pdf](https://arxiv.org/abs/1906.02688)][[talk](https://github.com/vihari/focussed_embs)][[slides](https://vimeo.com/384490539">talk</a>][<a href="https://docs.google.com/presentation/d/1cEiov879145R6oOBESjif2PcsNXKljZPORegf6_fEMU/edit?usp=sharing)]  
  We answer three interesting questions about adapting word-embeddings.
  + What is the best way to fintune word-embeddings? Answer: By revisiting the source corpus.
  + Does the pretrained word-embeddings retain information that can enable tuning to any new domain? Answer: No.
  + Are contextual embeddings so rich that they obfuscate the need to adapt embeddings? Answer No. 

* Generalizing across domains via cross-gradient training. 
  ICLR 2018 [[pdf](https://arxiv.org/pdf/1804.10745.pdf)][[code](https://github.com/vihari/crossgrad)]   
  We can avoid overfitting on the train domains by hallucinating new unseen domains. We propose CrossGrad that augments label consistent examples from new domains that helps in domain generalization.