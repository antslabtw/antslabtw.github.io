<img width="5156" height="350" alt="image" src="https://github.com/user-attachments/assets/6f8a1540-4824-452d-b859-da3c4b543a95" />---
layout: archive
title: "MOOSE"
permalink: /MOOSE/
author_profile: true
---
---
## 🦌 (MOOSE) Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring 🦌
---------------------------------------
<div align="center">
<div style="display: flex; justify-content: space-around; flex-wrap: wrap;"align="center">

  
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Po-Kai Chen</span>
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Bo-Wei Tsai</span>
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Kuan-Wei Shao</span>
  <a href="https://homepage.iis.sinica.edu.tw/pages/kinyiu/" style="margin: 10px; width: 120px;text-decoration:none; color:#337ab7;">Chien-Yao Wang</a>
  <a href="https://dlmsl.csie.ncu.edu.tw/faculty" style="margin: 10px;width: 120px; text-decoration:none; color:#337ab7;">Jia-Ching Wang</a>
  <a href="https://antslabtw.github.io/faculty/" style="margin: 10px;width: 120px; text-decoration:none; color:#337ab7;">Yi-Ting Huang</a>


</div>

<div align="center" >
Our paper <strong>Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring</strong> is accepted to ACL 2025!
</div>

## Model overview 
---------------------------------------  
  <img src="/images/aes.png"  width="60%" height="60%"/>

</div>

**MOOSE** framework is **the-state-of-the-art** model on **multi-trait cross prompt essay scoring**. It consist of serveral mechanism:

1. **Multi Chunk content feature extractor**: Extract content features of the essay and prompt ,with multi-granularity, via document BERT and multi-chunk BERT models which is follow [(Wang et al., 2022)](https://aclanthology.org/2022.naacl-main.249.pdf). The content features are composed of chuncks at different levels of granularity, enabling the model not only to analyze the essay as a whole, but also to capture the performance of different segments within the essay.

2. **Multi-trait attention**: adopt the architecture of trait attention mechanism proposed in ProTACT [(Do et al.,2023)](https://aclanthology.org/2023.findings-acl.98.pdf) to learn trait-specific representations. Different from the ProTACT, we use the document BERT feature as the query and the multi-chunk BERT features as both key and value in the cross-attention
layer to learn non-prompt specific representation of the essay. 

3. **Mixture of Ordered Scoring Experts**: a mechanism designed to mimic human expert reasoning through a three-stage Ordered Scoring Experts (OSE) framework: a scoring expert learns trait-specific signals from essay features, a ranking expert adaptively selects scoring cues via a Mixture-of-Experts (MoE) mechanism, and an adherence expert assesses the alignment between essay content and prompt. The model employs a dual-layer cross-attention decoder, with stop-gradient applied to queries to simulate scoring cue retrieval. Together, these components enable more accurate and robust essay trait evaluation.
<div align="center">
  <img src="/images/moose.png"  width="60%" height="60%"/>
</div>


## Source Code

* The source code of the model is [here](https://github.com/antslabtw/MOOSE-AES)
* The online scoring engine is [here](https://github.com/tempxdxd)

## Citation
```bibtex
@inproceedings{pokaimooseAES2025,
    title = "Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring",
    author = "Po-Kai Chen an
      Bo-Wei Tsai  and
      Kuan-Wei Shao and
      Chien-Yao Wang and
      Jia-Ching Wang and
     Yi-Ting Huang",
    booktitle = "Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics",
    month = aug,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",

    abstract = "Finetuning large language models (LLMs) has been empirically effective on a variety of downstream tasks. Existing approaches to finetuning an LLM either focus on parameter-efficient finetuning, which only updates a small number of trainable parameters, or attempt to reduce the memory footprint during the training phase of the finetuning. Typically, the memory footprint during finetuning stems from three contributors: model weights, optimizer states, and intermediate activations. However, existing works still require considerable memory, and none can simultaneously mitigate the memory footprint of all three sources. In this paper, we present quantized side tuing (QST), which enables memory-efficient and fast finetuning of LLMs by operating through a dual-stage process. First, QST quantizes an LLM{'}s model weights into 4-bit to reduce the memory footprint of the LLM{'}s original weights. Second, QST introduces a side network separated from the LLM, which utilizes the hidden states of the LLM to make task-specific predictions. Using a separate side network avoids performing back-propagation through the LLM, thus reducing the memory requirement of the intermediate activations. Finally, QST leverages several low-rank adaptors and gradient-free downsample modules to significantly reduce the trainable parameters, so as to save the memory footprint of the optimizer states. Experiments show that QST can reduce the total memory footprint by up to 2.3{\texttimes} and speed up the finetuning process by up to 3$\times$ while achieving competent performance compared with the state-of-the-art. When it comes to full finetuning, QST can reduce the total memory footprint up to 7$\times$."
}
<!--booktitle = "Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
url = "https://aclanthology.org/2024.acl-long.1/",
oi = "10.18653/v1/2024.acl-long.1",
pages = "1--17",-->
