---
title: People
permalink: /people/
---
{% assign people_sorted = site.people | sort: 'joined' %}
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


| Who are they | When were they here | Where they went |
| :------------- |:-------------| :-----------|
| [Lucas Lo Vercio](http://www.pladema.net/llovercio/) | Ph.D. student and Postdoc (2012-2017) | Postdoc at University of Calgari
