---
title: Thesis
permalink: /thesis/
---

![](/images/others/celebration.png)

### Thesis

Here you can find some of the PhD thesis and final projects of Software Engineering that were done in our group. Most of them are in Spanish.


### PhD Thesis

Since we established ourselves as Yatiris in 2014, several PhD students made there thesis in our lab. We are always looking for talented, enthusiastic students with a strong mathematical and software development backgroud to join Yatiris to pursue a doctorate degree. If you want to know more about our open positions, you can check the Career tab in this website, or send us an email to [yatirisarg@gmail.com](mailto:yatirisarg@gmail.com).


<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains "tesis-doctorado" %}
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

<hr>


### Final Projects - Software Engineering

Our researchers are also actively supervising Software Engineering students in their final projects. We believe that undergrad thesis are an excellent opportunity to learn very specific topics, while also practicing some of the activities we make in the lab.

These are just a few of the final project that were made in the lab. If you want to do yours also at Yatiris, you can contact us at [yatirisarg@gmail.com](mailto:yatirisarg@gmail.com). We always have open topics to work on!

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