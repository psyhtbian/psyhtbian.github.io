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

<ul class="publication-list">
{% for post in site.publications reversed %}
<li>
<p><strong><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></strong><br />
Published in <i>{{ post.venue }}</i>, {{ post.date | default: "1900-01-01" | date: "%Y" }}{% if post.excerpt %}<br />
{{ post.excerpt }}{% endif %}{% if post.citation %}<br />
Recommended citation: {{ post.citation }}{% endif %}{% if post.paperurl %}<br />
<a href="{{ post.paperurl }}">Download Paper</a>{% endif %}</p>
</li>
{% endfor %}
</ul>

Profiles
======

* [Google Scholar](https://scholar.google.com/citations?hl=zh-CN&user=4VP6u6EAAAAJ)
* [ResearchGate](https://www.researchgate.net/profile/Haotian-Bian)
* [ORCID](https://orcid.org/0000-0002-6105-1931)
