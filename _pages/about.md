---
permalink: /
title: "Haotian Bian"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. student in the Collaborative Innovation Center of Assessment for Basic Education Quality at Beijing Normal University.


Research Interests
======

* Parenting and family dynamics
* Adolescent mental health
* Longitudinal method

Education
======

* Ph.D. Student, Collaborative Innovation Center of Assessment for Basic Education Quality, Beijing Normal University, 2025-2028
* M.A., Collaborative Innovation Center of Assessment for Basic Education Quality, Beijing Normal University, 2021-2024
* B.S., Department of Psychology, Northwest Normal University, 2017-2021

Publications
======

{% if site.author.googlescholar %}
You can also find my articles on [my Google Scholar profile]({{ site.author.googlescholar }}).
{% endif %}

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

Profiles
======

* [Google Scholar](https://scholar.google.com/citations?hl=zh-CN&user=4VP6u6EAAAAJ)
* [ResearchGate](https://www.researchgate.net/profile/Haotian-Bian)
* [ORCID](https://orcid.org/0000-0002-6105-1931)
