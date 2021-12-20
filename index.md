---
layout: default
usemathjax: true
---

I am an AI resident at VinAI Research Vietnam. 
I obtained my B.S. degree in Computer Science from Hanoi University of Science and Technology. 
My research explores mechanisms to understand human languages for computers so that computers can perform cognitive language-related tasks for us. Among others, I am especially interested in distilling structured information and mining useful knowledge from massive human-written text of various domains. I am also interested in other language-related problems with deep learning, including reading comprehension, question answering, machine translation, and natural language generation.
# Biography

{% 
assign biography = "
Nov. 2019 – Present | Research Resident at VinAI Research
---
Jun. 2018 – Oct. 2019 | Software developer at VC Corporation
---
May. 2017 – Oct. 2017 | AI Intern at Cinnamon AI Lab
---
Aug. 2014 – Jun. 2019 | Student at Hanoi University of Science and Technology (HUST). I graduated with an Excellence Degree of Engineer in Computer Science.

" | split: '---' 
%}

{% for milestone in biography %}
{% assign milestone_arr = milestone | strip | split: "|" %}
__<span> {{ milestone_arr[0] | strip }} </span>__ : *{{ milestone_arr[1] | strip}}*
{% endfor %}

# Publications

{% 
assign publications = "

Exploiting Document Structures and Cluster Consistencies for Event Coreference Resolution |
__Hieu Minh Tran*__, Duy Phung, Thien Huu Nguyen |
*Proceedings of ACL-IJCNLP 2021 (oral)* |
pdfs/ACL_2021.pdf
---
The Dots Have Their Values: Exploiting the Node-Edge Connections in Graph-based Neural Models for Document-level Relation Extraction |
__Hieu Minh Tran*__, Minh, Minh Trung Nguyen, Thien Huu Nguyen |
*Proceedings of EMNLP 2020 (Findings)* |
pdfs/EMNLP_2020.pdf
---
Learning Cross-lingual Representations for Event Coreference Resolution
with Multi-view Alignment and Optimal Transport |
Duy Phung, __Hieu Minh Tran*__, Minh Van Nguyen, Thien Huu Nguyen |
*Proceedings of the first Workshop on Multilingual Representation Learning (MRL 2021) at
EMNLP 2021* |
https://ieeexplore.ieee.org/iel7/6287639/8948470/09138369.pdf

" | split: '---' 
%}


{% for pub in publications %}
{% assign pub_arr = pub | strip | split: "|" %}
__<span style='font-size: 20px'> {{ pub_arr[0] | strip }} </span>__ <br> *{{ pub_arr[1] | strip}}* <br> {{ pub_arr[2] | strip}} - [PDF]({{ pub_arr[3] | strip }})<br>
{% endfor %}



# Awards

__Third prize in the national high school students at Information technology subject in 12th grade, 2014__ <br>

# Mentors
- [Thien Huu Nguyen](http://ix.cs.uoregon.edu/~thien)

# Advisors
- [Dat Quoc Nguyen](https://datquocnguyen.github.io)
- [Tin Vo](https://duytinvo.github.io)
