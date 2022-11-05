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

Before pursuing higher degrees at HKPolyU, I served as an IT project manager in LFLogistics China, a world's leading company in supply chain (now under Maersk). Check [here](https://www.hbs.edu/faculty/Pages/item.aspx?num=13533 "Redirecting to the article from Harvord Business School") for its legends from Harvord! I took lead of the system development and implementation of a large intelligent digital project for over 10 key clients, e.g., NIKE, Skechers, Under Armer, Victoria's Secret, Tommy Hilfiger, etc.

After the fascinating experience there, I ask myself two questions: 

(i) What is the real smart DATA? (ii) How could we make the DATA smarter?

In pursuit of what I dreamed of, my current major research interests include but not limit to Data Mining and Graph Learning. At present, I enjoy delving into knowledge graph error detection and commonsense question answering over knowledge graphs. The more I expose to data, the more charm I appreciate. I'm still on my way towards a smart data researcher.

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
