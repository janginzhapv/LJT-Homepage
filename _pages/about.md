---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD candidate at HKUST NLP Group, advised by Professor Junxian He. I graduated from Shanghai Jiao Tong University (SJTU) in June 2024. My research focuses on natural language processing and machine learning, with specific interests in LLM Reasoning and Reinforcement Learning, Hallucination in Vision-Language Models (VLM), and LLM truthfulness and Interpretability.

I have research experience at MINIMAX (February 2025 - Present), Tencent WXG (June 2024 - September 2024), where I was advised by Zifei Shan, and Shanghai AI Lab (June 2023 - December 2023), where I was advised by Prof. Yu Cheng.

Education:
- Ph.D. in Computer Science (2024-Present) at Hong Kong University of Science and Technology
- B.Eng. (2020-2024) at Shanghai Jiao Tong University

Awards:
- Zhiyuan Honor Scholarship at Shanghai Jiao Tong University

## Publications

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2>
        <hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

Contact:
- Email: jliugi@connect.ust.hk
- GitHub: Vicent0205 (https://github.com/Vicent0205)
- Google Scholar: https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate
- X (Twitter): @junteng88716710
