---
permalink: /
title: "Haotian Bian (边昊天)"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. student in the Collaborative Innovation Center of Assessment for Basic Education Quality at Beijing Normal University.


Education
======

* Ph.D. Student, Collaborative Innovation Center of Assessment for Basic Education Quality, Beijing Normal University, 2025-2028
* Master of Education, Collaborative Innovation Center of Assessment for Basic Education Quality, Beijing Normal University, 2021-2024
* Bachelor of Science, School of Psychology, Northwest Normal University, 2017-2021

Research Interests
======

* Parenting and family dynamics
* Adolescent mental health
* Longitudinal method

First-author Publications
======

{% include base_path %}

<ul class="publication-list">
{% assign first_author_publications = site.publications | where: "author_position", "first" | sort: "date" | reverse %}
{% for post in first_author_publications %}
<li>
<p>{% if post.paperurl %}<a class="publication-title-link" href="{{ post.paperurl | prepend: base_path }}"><strong>{{ post.title }}</strong></a>{% else %}<strong>{{ post.title }}</strong>{% endif %}<br />
Published in <i>{{ post.venue }}</i>, {{ post.date | default: "1900-01-01" | date: "%Y" }}{% if post.citation %}<br />
Recommended citation: {{ post.citation }}{% endif %}{% if post.citation_chinese %}<br />
Recommended citation in Chinese: {{ post.citation_chinese }}{% endif %}</p>
</li>
{% endfor %}
</ul>

Co-authored Publications
======

<ul class="publication-list">
{% assign coauthored_publications = site.publications | where: "author_position", "coauthored" | sort: "date" | reverse %}
{% for post in coauthored_publications %}
<li>
<p>{% if post.paperurl %}<a class="publication-title-link" href="{{ post.paperurl | prepend: base_path }}"><strong>{{ post.title }}</strong></a>{% else %}<strong>{{ post.title }}</strong>{% endif %}<br />
Published in <i>{{ post.venue }}</i>, {{ post.date | default: "1900-01-01" | date: "%Y" }}{% if post.citation %}<br />
Recommended citation: {{ post.citation }}{% endif %}{% if post.citation_chinese %}<br />
Recommended citation in Chinese: {{ post.citation_chinese }}{% endif %}</p>
</li>
{% endfor %}
</ul>
