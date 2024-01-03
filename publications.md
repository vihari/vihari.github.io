---
layout: page
title: Publications
---

### Research Theme
I am interested in building reliable learning systems. Lack of reliability in deployed systems arises (majorly) due to misspecification of the task. I research on non-standard training of machines in order to better define the task. During my PhD, I explored using meta-data, more specifically exploiting per-example annotation identifying the environment or the domain, in a problem setting called domain generalization [[ICLR18](#crossgrad)][[ICML20](#csd)][[ICML20a](#dg_for_dr)][[NeurIPS21](#gi)][[ICLR22](#cgd)] along with its related problems of domain adaptation ([[ACL19](#srcsel)], [[EMNLP20](#topicsig)]) and evaluation  ([[NeurIPS21](#accsurf)]). 

After PhD, again with the intent of building reliable systems, I have been developing algorithms that enable humans to explain (to a machine) what causes a label. So far, we studied supervising using local (i.e. example-level) explanations [[NeurIPS23](#mlx)] and are making progress toward global (i.e. model-level) concept-based explanations [[Preprint](#uace)]. 

<!--
I am interested in studying the performance of Machine Learning systems beyond well-represented training distributions. Towards this objective, I work on generalization, evaluation and adaptation aspects of ML algorithms on unseen distributions.
An example of domain shift in practice is when an entity recognizer trained on news articles is used on emails or when an Automatic Speech Recognition engine trained on native-english speaker is deployed on foreign speakers. 

My research has three broad themes below. 

* **Generaliation**: Algorithms for training domain robust models: domain generalization. Can we exploit the natural variation between train domains and zero-shot generalize to unseen domains? [[ICLR18](#crossgrad)][[ICML20](#csd)][[ICML20a](#dg_for_dr)][[NeurIPS21](#gi)][[ICLR22](#cgd)]
* **Adaptation**: Neither (heavily-subscribed) service models nor (hardware-deficient) clients can afford standard fine-tuning. Can we adapt on the fly without parameter fine-tuning or labeled data? [[ACL19](#srcsel)] [[EMNLP20](#topicsig)]
* **Assessment**: How can we declare or predict test time failures? [[NeurIPS21](#accsurf)]
--> 

Check [Google Scholar](https://scholar.google.co.in/citations?user=DQddccYAAAAJ) for an exhaustive list of publications. 

<a name="uace"></a>
* **Estimation of Concept Explanations Should be Uncertainty Aware**   
  *Under review* [[forum](https://openreview.net/forum?id=WqsYs05Ri7)].  
  with *J Heo, S Singh, A Weller*.    
Uncertainty aware estimation improves reliability of concept explanations
<a name="mlx"></a>
* **Use Perturbations when Learning from Explanations**   
  **NeurIPS 2023** [[pdf](https://arxiv.org/pdf/2303.06419.pdf)].  
  with *J Heo, M Wicker, A Weller*.    
  Explanations are indispensable for avoiding learning of nuisance features or for label efficiency. 
  We studied robustness (such as adversarial or certified-robustness learning) methods for learning from explanation constraints and found them to consistently and drastically out-perform existing methods that regularise using an interpretability tool.
<a name="cgd"></a>
* **Human-in-the-loop Mixup**   
  **UAI 2023** [[pdf](https://arxiv.org/pdf/2211.01202.pdf)]   
  with *K Collins, U Bhatt, W Liu, I Sucholutsky, B Love, A Weller*   
  Synthetic labels used in mixup are not consistently aligned with human perceptual judgments; relabeling examples, with humans-in-the-loop and leveraging human uncertainty information, holds promise to increase downstream model reliability.
* **Robustness, Evaluation and Adaptation of Machine Learning Models in the Wild**    
  PhD Thesis. [[arxiv](https://arxiv.org/abs/2303.02781)]
  
* **Focus on the Common Good: Group Distributional Robustness Follows**.   
  **ICLR 2022** [[pdf](https://arxiv.org/pdf/2110.02619.pdf)] [[code](https://github.com/vihari/CGD/)][[slides](https://docs.google.com/presentation/d/1ZFkwx6QxZgLD6X0ld7FAi6bJUe90Pif0ZGTc9A3pOeM/edit?usp=drive_link)]   
  with *P Netrapalli*, *S Sarawagi*   
  When train group sizes are highly disproportionate, how can we train such that we generalize well to all groups irrespective of their training sizes? We found that by just focussing the training on the groups that improve performance on other groups as well as on the self (common good) yield better group robustness.   
<a name="gi"></a>
* **Training for the Future: A Simple Gradient Interpolation Loss to Generalize Along Time**.  
  **NeurIPS 2021** [[pdf](https://openreview.net/pdf?id=U7SBcmRf65)][[code](https://github.com/anshuln/Training-for-the-Future)]  
  with *A Nasery, S Thakur, A De, S Sarawagi*  
How can we prepare models for future by training on past data? Standard approaches overfit on past and fail to extrapolate to future. We proposed to parameterize the predictor on time and regularized its dependence on time to avoid overfitting on past data.     
<a name="accsurf"></a>
* **Active Assessment of Prediction Services as Accuracy Surface Over Attribute Combinations**.  
  **NeurIPS 2021** [[pdf](https://arxiv.org/pdf/2108.06514.pdf)][[code](https://github.com/vihari/AAA)][[slides](https://docs.google.com/presentation/d/1cKjO5ROhr-PN_rwb0VTqKTye_ZKpW4Yy8XxX_Hz6CME/edit?usp=sharing)]  
  with *S Chakrabarti*, *S Sarawagi*  
  We argue that Prediction Services should report performance for every combination of prespecified and interpretable data shifts, and go beyond leaderboards and standard bechmarks. How can we efficiently estimate performance over combinatorially many shifts without access to equally large labeled data? Check out our paper to know more.      
<a name="topicsig"></a>
* **NLP Service APIs and Models for Efficient Registration of New Clients**.   
  **EMNLP Findings 2020** [[pdf](https://arxiv.org/pdf/2010.01526.pdf)][[code](https://github.com/sahil00199/KYC)]   
  with *S Shah, S Chakrabarti, S Sarawagi*   
  Prediction service APIs are expected to cater millions of client distributions. Adapting to each client is not scalable for computation and storage concerns. 
  We propose an on-the-fly adaptation technique using client side corpus signature.    
<a name="dg_for_dr"></a>
* **Untapped Potential of Data Augmentation: A Domain Generalization Viewpoint**.   
  **ICML UDL Workshop 2020** [[pdf](https://arxiv.org/abs/2007.04662)][[slides](https://docs.google.com/presentation/d/1IZuAc9GKrB2WO00kWOo1FOMs8sGBWe7XZLrhfZNHAJY/edit?usp=sharing)].       
  with *S Shankar*   
  We argue why plain augmentation leads to shallow parameter sharing between the original and augmented examples. We show how even SoTA augmentation methods could still overfit on augmentations and the scope for mitigating this overfit by employing domain generalization techniques.  
<a name="csd"></a>
* **Efficient Domain Generalization via Common-Specific Low-Rank Decomposition.**  
  **ICML 2020** [[pdf](https://arxiv.org/abs/2003.12815)][[code](https://github.com/vihari/CSD/)][[talk](https://icml.cc/virtual/2020/poster/6528)][[slides](https://docs.google.com/presentation/d/1x0MXQrutH1XJunhCPPqaHhWnqn49fZcPyMyJEdGDWv4/edit?usp=sharing)]    
  with *P Netrapalli, S Sarawagi*   
  When a model is trained on multiple sources, learned parameters are composed of both shared and domain-specific components. 
  While domain-specific components improve the performance on seen train domains, they impede generalization to new domains. 
  We propose a method called CSD, as a replacement for the final linear layer, that identifies and removes specific components, thereby retaining only the component common across all domains.   Our method is simple, efficient and yet competitive.  
<a name="srcsel"></a>
* **Topic Sensitive Attention on Generic Corpora Corrects Sense Bias in Pretrained Embeddings.**  
  **ACL 2019** [[pdf](https://arxiv.org/abs/1906.02688)][[code](https://github.com/vihari/focussed_embs)][[talk](https://vimeo.com/384490539)][[slides](https://docs.google.com/presentation/d/1cEiov879145R6oOBESjif2PcsNXKljZPORegf6_fEMU/edit?usp=sharing)]  
  with *S Chakrabarti*, *S Sarawagi*    
  We answer three interesting questions about adapting word-embeddings.
  + What is the best way to fintune word-embeddings? Answer: By revisiting the source corpus.
  + Does pretrained word-embeddings retain information that can enable tuning to any new domain? Answer: No.
  + Are contextual embeddings so rich that they obfuscate the need to adapt embeddings? Answer No.   
<a name="crossgrad"></a>
* **Generalizing across domains via cross-gradient training.**   
  **ICLR 2018** [[pdf](https://arxiv.org/pdf/1804.10745.pdf)][[code](https://github.com/vihari/crossgrad)]   
  with *S Shankar, S. Chaudhuri, P. Jyothi, S Chakrabarti, S Sarawagi*   
  We can avoid overfitting on train domains by hallucinating examples from unseen domains. We propose CrossGrad that augments label consistent examples from new domains that help in domain generalization.
