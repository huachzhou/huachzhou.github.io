---
permalink: /
title: "Towards a Data Researcher"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am now a first-year research student in DEEP Lab at The Hong Kong Polytechnic University, Department of Computing, supervised by [Dr. Xiao Huang](https://www4.comp.polyu.edu.hk/~xiaohuang/index.html "Redirecting to Dr.Huang's homepage"). I obtained my Master's degree at HKPolyU in 2021, majored in Information Technology.

Before pursuing higher degrees at HKPolyU, I served as an IT project manager in LFLogistics China under Fung's Group (now under Maersk), a world's leading company in supply chain. Check [here](https://www.hbs.edu/faculty/Pages/item.aspx?num=13533 "Redirecting to the article from Harvord Business School") for its legends from Harvord Business School! I took lead of the implementation and project management of a large intelligent digital project, improving over 10 key clients' warehouse operation performance, including NIKE, Skechers, Under Armer, Victoria's Secret, Tommy Hilfiger, etc.

After the fascinating experience there, I ask myself two questions: 

(i) What is the real smart DATA? (ii) How could we make the DATA smarter?

In pursuit of what I'm dreaming for, my current major research interests include but not limit to data mining and graph learning. At present, I enjoy delving into knowledge graph error detection and commonsense question answering over knowledge graphs. The more I expose to data, the more charm I appreciate. I'm still on my way towards a smart data researcher.

<h1> Publications </h1>

{% include base_path %}

{% assign cur_year = "9999" %}
{% for post in site.publications reversed %}
  {% assign dates = post.date | split: "-" %}
  {% assign year = dates.first %}
  {% if year != cur_year %}
    {% assign cur_year = year %}
<h2> {{ year }} </h2>
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
