---
title: People
permalink: /people/
---
{% assign people_sorted = site.people | sort: 'order' %}
{% assign people_array = 'researcher|postdoc|phdstudent|undergrad' | split: '|' %}

{% for item in people_array %}

<div class="pos_header">
{% if item == 'postdoc' %}
<h3>Postdoctoral Fellows</h3>
 {% elsif item == 'researcher' %}
<h3>Permanent Researchers</h3>
 {% elsif item == 'phdstudent' %}
<h3>PhD Students</h3>
 {% elsif item == 'undergrad' %}
<h3>Undergrad Students</h3>
{% endif %}
</div>

<div class="content list people">
  {% for profile in people_sorted %}
    {% if profile.position contains item %}
    <div class="list-item-people">
      <p class="list-post-title">
        {% if profile.avatar %}
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
        {% else %}
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="http://evansheline.com/wp-content/uploads/2011/02/facebook-Storm-Trooper.jpg"></a>
        {% endif %}
        <a class="name" href="{{ site.baseurl }}{{ profile.url }}">{{ profile.name }}</a>
      </p>
    </div>    
    {% endif %}
  {% endfor %}
</div>
<hr>
{% endfor %}


### Other PLADEMA members

**Marcelo Vénere** - Director <br>
**Alejandro Clausse** - Vice-director <br>
**Juan Pablo D'Amato** - CONICET<br>

* * *

### Past members

**Hugo Luis Manterola** - Ph.D. student and Postdoc from 2013 to 2020, now Teaching Assistant at UNICEN and software developer at [Lamansys](https://lamansys.com.ar/).
**Tomás Pérez Cambet** - Undergrad student from 2018 to 2020.
[**Lucas Lo Vercio**](http://www.pladema.net/llovercio/) - Ph.D. student and Postdoc from 2012 to 2017, now postdoc at University of Calgari (Canada) <br>
**Pablo Rubí** - Undergrad and Ph.D. student from 2016 to 2017), now Software Developer at Amazon (Seattle, USA) <br>
**Ezequiel Fernández Vera** - Undergrad student and Research Engineer (2015-2017), now Software Developer at PLADEMA (SINIDE project) <br>