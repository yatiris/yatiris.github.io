---
title: News
permalink: /news/
---

![](/images/others/yatiris_lab.jpg)

## **News from the lab**

Find here our latest news, both in English and Spanish!


{% assign reference_types = "news-spanish|news-english" | split: "|" %}

{% for type in reference_types %}

{% if type == 'news-english' %}
### **English**
 {% elsif type == 'news-spanish' %}
### **Español**
{% endif %}

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains type %}
    <div class="list-item">
      <p class="list-post-title">
        (<small>{{post.date | date: "%m/%d/%y" }}</small>) <a href="{{ site.baseurl }}{{ post.url }}">- {{ post.title }}</a> 
      </p>
    </div>
    {% endif %}
  {% endfor %}
</div>

<hr>
{% endfor %}