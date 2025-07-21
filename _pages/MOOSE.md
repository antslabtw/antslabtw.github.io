---
layout: archive
title: ""
permalink: /MOOSE/
author_profile: true
---

## 🦌 (MOOSE) Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring 🦌
---------------------------------------


<div align="center">

  
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Po-Kai Chen</span>
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Bo-Wei Tsai</span>
  <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">Kuan-Wei Shao</span>
  <a href="https://homepage.iis.sinica.edu.tw/pages/kinyiu/" style="margin: 10px; width: 120px;text-decoration:none; color:#337ab7;">Chien-Yao Wang</a>
  <a href="https://dlmsl.csie.ncu.edu.tw/faculty" style="margin: 10px;width: 120px; text-decoration:none; color:#337ab7;">Jia-Ching Wang</a>
  <a href="https://antslabtw.github.io/faculty/" style="margin: 10px;width: 120px; text-decoration:none; color:#337ab7;">Yi-Ting Huang</a>

</div>

<div align="center" >
Our paper <strong>Mixture of Ordered Scoring Experts for Cross-prompt Essay Trait Scoring</strong> is accepted to ACL 2025!<br><br>
</div>

<div align="left" >
MOOSE is multi traits cross prompt essay scoring model which imitates how human raters evaluate essays. MOOSE is composed of three experts:<br><br>
1) Scoring Expert: Learn essay inherent scoring cues.<br>
2) Ranking Expert: Compare relative quality across different essays.<br>
3) Adherence Expert: Estimate the degree of prompt adherence.<br><br>
It not only outperforms previos method and stables no matter in prompts and traits.
 <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">The source code of the model is </span>
  <a href="https://github.com/antslabtw/MOOSE-AES" style="margin: 10px; width: 120px;text-decoration:none; color:#337ab7;">here</a>
   <span style="margin: 10px;width: 120px; text-decoration:none;color:#333;">and the online scoring engine is </span>
  <a href="https://github.com/antslabtw/MOOSE-AES" style="margin: 10px; width: 120px;text-decoration:none; color:#337ab7;">here.</a><br><br>
</div>

<div align="center" >
<img src="/images/moose_illustration.png" align="center" width="22%" height="22%"/>





<img src="/images/moose_result.png" align="center"  width="40%" height="40%"/>

</div>

<div align="center" >

<span style="margin: 10px; width: 120px; text-decoration:none; color:#333; font-size: 30px; font-weight: bold;">
  Model overview
</span>

<hr style="border: none; height: 5px; background-color: #ccc; width: 80%;">

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


<!--booktitle = "Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
url = "https://aclanthology.org/2024.acl-long.1/",
oi = "10.18653/v1/2024.acl-long.1",
pages = "1--17",-->

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
    month = "aug",
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    abstract = "utomated Essay Scoring (AES) plays a crucial role in language assessment. In particular, cross-prompt essay trait scoring provides learners with valuable feedback to improve their writing skills. However, due to the scarcity of prompts, most existing methods overlook critical information, such as content from prompts or essays, resulting in incomplete assessment perspectives. In this paper, we propose a robust AES framework, the Mixture of Ordered Scoring Experts (MOOSE), which integrates information from both prompts and essays. MOOSE employs three specialized experts to evaluate (1) the overall quality of an essay, (2) the relative quality across multiple essays, and (3) the relevance between an essay and its prompt. MOOSE introduces the ordered aggregation of assessment results from these experts along with effective feature learning techniques. Experimental results demonstrate that MOOSE achieves exceptionally stable and state-of-the-art performance in both cross-prompt scoring and multi-trait scoring on the ASAP++ dataset. The source code is released at https://github.com/antslabtw/MOOSE-AES"
}
