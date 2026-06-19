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
  <strong>*</strong> denotes equal contribution. Click a title to view the paper. A full list is also available on my <a href="{{ site.author-info.google_scholar.url }}" target="_blank" rel="noopener">Google Scholar profile</a>.
</p>

{% assign publications = "
PRIME: Planning and Retrieval-Integrated Memory for Enhanced Reasoning ;; **Hieu Tran**, Zonghai Yao, Nguyen Luong Tran, Zhichao Yang, Feiyun Ouyang, Shuo Han, Razieh Rahimi, Hong Yu ;; Proceedings of AAAI 2026 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:ufrVoPGSRksC
@@@
Exploiting Tree Structure for Credit Assignment in RL Training of LLMs ;; **Hieu Tran**, Zonghai Yao, Hong Yu ;; Findings of ACL 2026 (arXiv:2509.18314) ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:_FxGoFyzp5QC
@@@
Chatbot To Help Patients Understand Their Health ;; Won Seok Jang*, **Hieu Tran***, Manav Mistry, SaiKiran Gandluri, Yifan Zhang, Sharmin Sultana, Sunjae Kwon, Zonghai Yao, Hong Yu ;; Findings of EMNLP 2025 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:WF5omc3nYNoC
@@@
LEAF: Learning and Evaluation Augmented by Fact-Checking to Improve Factualness in Large Language Models ;; **Hieu Tran**, Junda Wang, Yujan Ting, Hong Yu, Weijing Huang, Terrence Chen ;; Proceedings of EMNLP 2025 (Industry Track) ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:Tyk-4Ss8FVUC
@@@
RARE: Retrieval-Augmented Reasoning Enhancement for Large Language Models ;; **Hieu Tran**, Zonghai Yao, Zhichao Yang, Junda Wang, Yifan Zhang, Shuo Han, Feiyun Ouyang, Hong Yu ;; Proceedings of ACL 2025 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:eQOLeE2rZwMC
@@@
ReadCtrl: Personalizing Text Generation with Readability-Controlled Instruction Learning ;; **Hieu Tran**, Zonghai Yao, Lingxi Li, Hong Yu ;; Fourth Workshop on Intelligent and Interactive Writing Assistance, 2025 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:W7OEmFMy1HYC
@@@
Enhancing LLMs for Identifying and Prioritizing Important Medical Jargons from Electronic Health Record Notes Utilizing Data Augmentation ;; Won Seok Jang, Sharmin Sultana, Zonghai Yao, **Hieu Tran**, Zhichao Yang, Sunjae Kwon, Hong Yu ;; arXiv preprint arXiv:2502.16022, 2025 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:YsMSGLbcyi4C
@@@
ReadMe: Bridging Medical Jargon and Lay Understanding for Patient Education through Data-Centric NLP ;; Zonghai Yao, Nandyala Siddharth Kantu, Guanghao Wei, **Hieu Tran**, Zhangqi Duan, Sunjae Kwon, Zhichao Yang, Hong Yu ;; Findings of EMNLP 2024 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:qjMakFHDy7sC
@@@
SemiHVision: Enhancing Medical Multimodal Models with a Semi-Human Annotated Dataset and Fine-Tuned Instruction Generation ;; Junda Wang, Yujan Ting, Eric Z. Chen, **Hieu Tran**, Hong Yu, Weijing Huang, Terrence Chen ;; arXiv preprint arXiv:2410.14948, 2024 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:zYLM7Y9cAGgC
@@@
BioInstruct: Instruction Tuning of Large Language Models for Biomedical Natural Language Processing ;; **Hieu Tran**, Zhichao Yang, Zonghai Yao, Hong Yu ;; Journal of the American Medical Informatics Association, 31(9), 1821–1832, 2024 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:2osOgNQ5qMEC
@@@
Vietnamese Speech-Based Question Answering over Car Manuals ;; Tin Duy Vo, Manh Tien Luong, Duong Minh Le, **Hieu Tran**, Nhan Tri Do, Duy Nguyen, Thien Hai Nguyen, Hung Hai Bui, Dat Quoc Nguyen, Dinh Phung ;; Companion Proceedings of IUI 2022 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:IjCSPb-OGe4C
@@@
A Vietnamese-English Neural Machine Translation System ;; Thien Hai Nguyen, Tuan-Duy H. Nguyen, Duy Phung, Duy Tran-Cong Nguyen, **Hieu Minh Tran**, Manh Luong, Tin Duy Vo, Hung Hai Bui, Dinh Phung, Dat Quoc Nguyen ;; InterSpeech 2022 — Show & Tell ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:UeHWp8X0CEIC
@@@
Learning Cross-lingual Representations for Event Coreference Resolution with Multi-view Alignment and Optimal Transport ;; Duy Phung, **Hieu Tran**, Minh Van Nguyen, Thien Huu Nguyen ;; MRL Workshop at EMNLP 2021 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:9yKSN-GCB0IC
@@@
Exploiting Document Structures and Cluster Consistencies for Event Coreference Resolution ;; **Hieu Tran***, Duy Phung, Thien Huu Nguyen ;; Proceedings of ACL-IJCNLP 2021 (Oral) ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:d1gkVwhDpl0C
@@@
The Dots Have Their Values: Exploiting the Node-Edge Connections in Graph-based Neural Models for Document-level Relation Extraction ;; **Hieu Tran***, Minh Trung Nguyen, Thien Huu Nguyen ;; Findings of EMNLP 2020 ;; https://scholar.google.com/citations?view_op=view_citation&hl=en&user=tTfxxcAAAAAJ&citation_for_view=tTfxxcAAAAAJ:u-x6o8ySG0sC
" | split: "@@@" %}

<ol class="pub-list">
{% for pub in publications %}
{% assign p = pub | strip | split: ";;" %}
{% assign url = p[3] | strip %}
  <li class="pub">
    <div class="pub-body">
      <a class="pub-title" href="{{ url }}" target="_blank" rel="noopener">{{ p[0] | strip }}</a>
      <div class="pub-authors">{{ p[1] | strip | markdownify | remove: '<p>' | remove: '</p>' }}</div>
      <div class="pub-meta">
        <span class="pub-venue">{{ p[2] | strip }}</span>
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
