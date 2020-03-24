---
title: Thesis
permalink: /thesis/
---

![](/images/others/celebration.png)

### Thesis

Here you can find some of the PhD thesis and final projects of Software Engineering that were done in our group. Most of them are in Spanish.


### PhD Thesis

These are the PhD thesis that were done in our group.

TBD


### Final Projects (Master Thesis)

These are some of the final projects of Software Engineering that were done in our group.

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains "tesis-grado" %}
    <div class="list-item">
      <p class="list-post-title">
        <a href="{{ post.url | prepend: site.baseurl }}">
            <div class="row">
                <div class="col-sm-4">
                    <img src="/{% if post.header-img %}{{ post.header-img }}{% else %}{{ site.header-img }}{% endif %}">
                </div>
                <div class="col-sm-8">
                    <h5 class="post-title">
                        {{ post.title }}
                    </h5>
                    <p class="list-detail" style="color:#A8A3A0" >
                      {{ post.description }}
                    </p>
                </div>
            </div>
            <hr/>
        </a>
      </p>
    </div>
    {% endif %}
  {% endfor %}
</div>