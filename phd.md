---
title: Proyectos de Posgrado
permalink: /phd/
---
<br>

### Proyectos de Posgrado

Si querés hacer tu posgrado en Yatiris, te presentamos algunas de las propuestas abiertas. Podés ver algunas [tesis](thesis.md) ya defendidas y las [publicaciones](publications.md) más recientes. 
<br>


#### Propuestas

{% assign reference_type = "propuestas-phd" %}
{% assign state = "open" %}
{% assign sorted_list_of_posts = site.phd | sort: 'date' %}
<div class="content list">
    {% for post in sorted_list_of_posts %}
        {% if post.categories contains reference_type %}
            {% if post.state contains state %}
                <div class="list-item">
                    <p class="list-post-title">
                        <div class="row">
                            <div class="col-sm-4">
                                {% if post.header-img %}
                                    <img src="{{site.baseurl}}/images/phd/{{post.header-img}}">
                                {% else %} 
                                    <img src="http://evansheline.com/wp-content/uploads/2011/02/facebook-Storm-Trooper.jpg">
                                {% endif %}
                            </div>
                            <div class="col-sm-8">
                                <p class="post-title" style="font-weight:600">
                                    {{ post.title }}
                                </p>
                                <p class="list-detail" >
                                    A cargo de: <a href="mailto:{{post.contact}} ">
                                        {{ post.referent }}
                                    </a>
                                </p>
                                <p class="list-detail" style="font-size:.75rem" >
                                    {{ post.description }}
                                </p>
                            </div>
                        </div>
                    </p>
                </div>
                <hr/>
            {% endif %}
        {% endif %}
    {% endfor %}
    </div>




