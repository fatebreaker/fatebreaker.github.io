---
layout: default
mathjax: true
---

<p>
I am a Computer Science PhD student at the <strong>University of Massachusetts Amherst</strong>,
where my research focuses on <strong>Natural Language Processing</strong>. Previously, I worked
as an AI Resident at <strong>VinAI Research Vietnam</strong> and received my B.S. in Computer
Science from <strong>Hanoi University of Science and Technology</strong>.
</p>

<p>
My primary research interest is enabling large language models to understand, generate, and reason
about human language, so they can perform complex cognitive and language-related tasks more
reliably. Recently I have been working on <em>reinforcement learning</em> and <em>test-time
computing</em>, with a focus on improving the reasoning ability, factual accuracy, and efficiency
of LLMs in both general and domain-specific applications.
</p>

## News

<ul class="news-list">
  <li><span class="news-date">Mar 2026</span><span class="news-text">Paper on <em>tree-structured credit assignment for RL with LLMs</em> accepted to <strong>ACL 2026 (Findings)</strong>.</span></li>
  <li><span class="news-date">Dec 2025</span><span class="news-text"><em>PRIME</em> accepted to <strong>AAAI 2026</strong>.</span></li>
  <li><span class="news-date">Sep 2025</span><span class="news-text"><em>LEAF</em> accepted to <strong>EMNLP 2025 (Industry Track)</strong>.</span></li>
  <li><span class="news-date">May 2025</span><span class="news-text"><em>RARE</em> accepted to <strong>ACL 2025</strong>.</span></li>
  <li><span class="news-date">2025</span><span class="news-text">Awarded the <strong>Optum AI Research Fellowship</strong>.</span></li>
</ul>

## Biography

{% assign biography = "
Aug 2022 – present | PhD student, Computer Science | University of Massachusetts Amherst
---
May 2024 – Aug 2024 | Research Intern | UII America
---
Nov 2019 – Jun 2022 | Research Resident | VinAI Research
---
Jun 2018 – Oct 2019 | Software Developer | VC Corporation
---
May 2017 – Oct 2017 | AI Intern | Cinnamon AI Lab
---
Aug 2014 – Jun 2019 | B.Eng. in Computer Science (Excellence Degree) | Hanoi University of Science and Technology
" | split: "---" %}

{% for milestone in biography %}
{% assign m = milestone | strip | split: "|" %}
<div class="bio-row">
  <div class="bio-date">{{ m[0] | strip }}</div>
  <div class="bio-role">
    <strong>{{ m[1] | strip }}</strong>{% if m[2] %} <span class="bio-sub">· {{ m[2] | strip }}</span>{% endif %}
  </div>
</div>
{% endfor %}

## Publications

<p style="color:#7d8595; font-size:14px; margin-top:-2px;">
  <strong>*</strong> denotes equal contribution. Selected publications, listed in reverse chronological order.
</p>

{% assign publications = "
Exploiting Tree Structure for Credit Assignment in Reinforcement Learning with Large Language Models | **Hieu Tran**, Zonghai Yao, Hong Yu | Proceedings of ACL 2026 (Findings) |
---
PRIME: Planning and Retrieval-Integrated Memory for Enhanced Reasoning | **Hieu Tran**, Zonghai Yao, Nguyen Luong Tran, Zhichao Yang, Feiyun Ouyang, Shuo Han, Razieh Rahimi, Hong Yu | Proceedings of AAAI 2026 | pdfs/prime.pdf
---
LEAF: Learning and Evaluation Augmented by Fact-Checking to Improve Factualness in Large Language Models | **Hieu Tran**, Junda Wang, Yujan Ting, Hong Yu, Weijing Huang, Terrence Chen | Proceedings of EMNLP 2025 (Industry Track) | pdfs/LEAF.pdf
---
RARE: Retrieval-Augmented Reasoning Enhancement for Large Language Models | **Hieu Tran**, Zonghai Yao, Zhichao Yang, Junda Wang, Yifan Zhang, Shuo Han, Feiyun Ouyang, Hong Yu | Proceedings of ACL 2025 | pdfs/RARE.pdf
---
Chatbot To Help Patients Understand Their Health | Won Seok Jang*, **Hieu Tran***, Manav Mistry, SaiKiran Gandluri, Yifan Zhang, Sharmin Sultana, Sunjae Kwon, Zonghai Yao, Hong Yu | Proceedings of EMNLP 2025 (Findings) | pdfs/chatbot.pdf
---
ReadMe: Bridging Medical Jargon and Lay Understanding for Patient Education through Data-Centric NLP | Zonghai Yao, Nandyala Siddharth Kantu, Guanghao Wei, **Hieu Tran**, Zhangqi Duan, Sunjae Kwon, Zhichao Yang, Hong Yu | Proceedings of EMNLP 2024 (Findings) | pdfs/ReadMe.pdf
---
BioInstruct: Instruction Tuning of Large Language Models for Biomedical Natural Language Processing | **Hieu Tran**, Zhichao Yang, Zonghai Yao, Hong Yu | Journal of the American Medical Informatics Association, ocae122 | pdfs/BioInstruct.pdf
---
A Vietnamese-English Neural Machine Translation System | Thien Hai Nguyen, Tuan-Duy H. Nguyen, Duy Phung, Duy Tran-Cong Nguyen, **Hieu Minh Tran**, Manh Luong, Tin Duy Vo, Hung Hai Bui, Dinh Phung, Dat Quoc Nguyen | InterSpeech 2022 — Show & Tell |
---
Learning Cross-lingual Representations for Event Coreference Resolution with Multi-view Alignment and Optimal Transport | Duy Phung, **Hieu Tran**, Minh Van Nguyen, Thien Huu Nguyen | MRL @ EMNLP 2021 | https://ieeexplore.ieee.org/iel7/6287639/8948470/09138369.pdf
---
Exploiting Document Structures and Cluster Consistencies for Event Coreference Resolution | **Hieu Tran***, Duy Phung, Thien Huu Nguyen | Proceedings of ACL-IJCNLP 2021 (Oral) | pdfs/ACL_2021.pdf
---
The Dots Have Their Values: Exploiting the Node-Edge Connections in Graph-based Neural Models for Document-level Relation Extraction | **Hieu Tran***, Minh Trung Nguyen, Thien Huu Nguyen | Proceedings of EMNLP 2020 (Findings) | pdfs/EMNLP_2020.pdf
" | split: "---" %}

<ol class="pub-list">
{% for pub in publications %}
{% assign p = pub | strip | split: "|" %}
{% assign pdf = p[3] | strip %}
  <li class="pub">
    <div class="pub-body">
      <span class="pub-title">{{ p[0] | strip }}</span>
      <div class="pub-authors">{{ p[1] | strip | markdownify | remove: '<p>' | remove: '</p>' }}</div>
      <div class="pub-meta">
        <span class="pub-venue">{{ p[2] | strip }}</span>
        {% if pdf != blank %}
        <a class="pub-pdf" href="{{ pdf }}" target="_blank" rel="noopener">PDF</a>
        {% else %}
        <span class="pub-pdf pub-pdf--pending">PDF coming soon</span>
        {% endif %}
      </div>
    </div>
  </li>
{% endfor %}
</ol>

## Advisor

<ul>
  <li><a href="https://www.cics.umass.edu/faculty/directory/hong_yu" target="_blank" rel="noopener">Prof. Hong Yu</a> — University of Massachusetts Amherst</li>
</ul>

## Awards

<ul>
  <li><strong>Optum AI Research Fellowship</strong> — Optum AI, 2025</li>
  <li><strong>Excellence Scholarship — Level A</strong> — School of Information and Communication Technology, HUST (awarded each semester to the top 5% of students)</li>
  <li><strong>National Excellent Student Award</strong> — Vietnam Ministry of Education and Training, 2014 (third prize, Informatics)</li>
</ul>
