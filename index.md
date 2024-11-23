---
layout: default
mathjax: true
---

I'm currently a Computer Science PhD student at the University of Massachusetts Amherst, where I research Natural Language Processing. Previously, I worked as an AI resident at VinAI Research Vietnam.  
I obtained my B.S. degree in Computer Science from Hanoi University of Science and Technology.  
My primary research interest is enabling LLMs to understand, generate, and reason about human language to enhance their ability to perform complex cognitive and language-related tasks. Recently, I have expanded my work to advanced topics such as Preference-based Learning, Retrieval-Augmented Generation (RAG), and Test Time Computing, with a particular emphasis on improving the reasoning capabilities, factual accuracy, and efficiency of language models in both general and domain-specific applications.

---

# Biography

{% assign biography = "
May. 2024 – Aug. 2024 | Research Intern at UII America
---
Aug. 2022 – Aug. 2027 | Computer Science PhD student at the University of Massachusetts Amherst
---
Nov. 2019 – Jun. 2022 | Research Resident at VinAI Research
---
Jun. 2018 – Oct. 2019 | Software Developer at VC Corporation
---
May. 2017 – Oct. 2017 | AI Intern at Cinnamon AI Lab
---
Aug. 2014 – Jun. 2019 | Student at Hanoi University of Science and Technology (HUST). I graduated with an Excellence Degree of Engineer in Computer Science.
" | split: "---" %}

{% for milestone in biography %}
{% assign milestone_arr = milestone | strip | split: "|" %}
__<span>{{ milestone_arr[0] | strip }}</span>__ : *{{ milestone_arr[1] | strip }}*  
{% endfor %}

---

# Publications

{% assign publications = "
RARE: Retrieval-Augmented Reasoning Enhancement for Large Language Models |
__Hieu Tran*__, Zonghai Yao, Junda Wang, Yifan Zhang, Zhichao Yang, Hong Yu |
*Under review* |
pdfs/LEAF.pdf
---
SemiHVision: Enhancing Medical Multimodal Models with a Semi-Human Annotated Dataset and Fine-Tuned Instruction Generation |
Junda Wang, Yujan Ting, Eric Z. Chen, __Hieu Tran*__, Hong Yu, Weijing Huang, Terrence Chen |
*Under review* |
pdfs/Semi.pdf
---
LEAF: Learning and Evaluation Augmented by Fact-Checking to Improve Factualness in Large Language Models |
__Hieu Tran*__, Junda Wang, Yujan Ting, Weijing Huang, Terrence Chen |
*Under review* |
pdfs/LEAF.pdf
---
BioInstruct: Instruction Tuning of Large Language Models for Biomedical Natural Language Processing |
__Hieu Tran*__, Zhichao Yang, Zonghai Yao, Hong Yu |
*Journal of the American Medical Informatics Association, ocae122* |
pdfs/BioInstruct.pdf
---
Readme: Bridging medical jargon and lay understanding for patient education through data-centric NLP |
Zonghai Yao, Nandyala Siddharth Kantu, Guanghao Wei, __Hieu Tran*__, Zhangqi Duan, Sunjae Kwon, Zhichao Yang, Hong Yu |
*Proceedings of EMNLP 2024 (Findings)* |
pdfs/ReadMe.pdf
---
Exploiting Document Structures and Cluster Consistencies for Event Coreference Resolution |
__Hieu Tran*__, Duy Phung, Thien Huu Nguyen |
*Proceedings of ACL-IJCNLP 2021 (oral)* |
pdfs/ACL_2021.pdf
---
The Dots Have Their Values: Exploiting the Node-Edge Connections in Graph-based Neural Models for Document-level Relation Extraction |
__Hieu Tran*__, Minh, Minh Trung Nguyen, Thien Huu Nguyen |
*Proceedings of EMNLP 2020 (Findings)* |
pdfs/EMNLP_2020.pdf
---
Learning Cross-lingual Representations for Event Coreference Resolution with Multi-view Alignment and Optimal Transport |
Duy Phung, __Hieu Tran*__, Minh Van Nguyen, Thien Huu Nguyen |
*Proceedings of the first Workshop on Multilingual Representation Learning (MRL 2021) at EMNLP 2021* |
https://ieeexplore.ieee.org/iel7/6287639/8948470/09138369.pdf
" | split: "---" %}

{% for pub in publications %}
{% assign pub_arr = pub | strip | split: "|" %}
__<span style="font-size: 20px">{{ pub_arr[0] | strip }}</span>__  
*{{ pub_arr[1] | strip }}*  
{{ pub_arr[2] | strip }} - [PDF]({{ pub_arr[3] | strip }})  
{% endfor %}

---

# Advisor

- [Hong Yu](https://www.cics.umass.edu/faculty/directory/hong_yu)
