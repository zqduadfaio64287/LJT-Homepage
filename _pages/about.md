---
permalink: /
title: "Junteng Liu"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a first-year Ph.D. candidate in Computer Science at the Hong Kong University of Science and Technology (HKUST), where I work on natural language processing and machine learning in the HKUST NLP Group, advised by Professor Junxian He. Professor Junxian He also advised me during my undergraduate studies at Shanghai Jiao Tong University (SJTU). I graduated from Shanghai Jiao Tong University with a B.Eng. degree in June 2024.

## Education

- Ph.D. in Computer Science, Hong Kong University of Science and Technology, 2024 - Present
- B.Eng., Shanghai Jiao Tong University, 2020 - 2024

## Research Experience

- Research Intern, MINIMAX, February 2025 - Present
- Research Intern, Tencent WXG, June 2024 - September 2024
  - Advisor: Zifei Shan
- Research Intern, Shanghai AI Lab, June 2023 - December 2023
  - Advisor: Prof. Yu Cheng

## Research Interests

- Natural Language Processing and Machine Learning
- LLM Reasoning and Reinforcement Learning
- Hallucination in Vision-Language Models (VLM)
- LLM Truthfulness and Interpretability

## Awards

- Zhiyuan Honor Scholarship, Shanghai Jiao Tong University

## Publications

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
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

## Contact

- Email: [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
- GitHub: [Vicent0205](https://github.com/Vicent0205)
- Google Scholar: [Google Scholar profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
- X (Twitter): [@junteng88716710](https://x.com/junteng88716710)