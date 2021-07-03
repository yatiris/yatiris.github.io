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


### Other PLADEMA members who work with us

**Marcelo Vénere** - Director <br>
**Alejandro Clausse** - Vice-director <br>
**Juan Pablo D'Amato** - CONICET<br>

* * *

### Past members

**Rodrigo Cobo** - Undergrad student, now Data Scientist at [Globant](https://www.globant.com/en) <br>
**Francisco Iarussi** - Undergrad student and Research Trainee from 2020 to 2021, now QA and Test Automation Engineer at [Globant](https://www.globant.com/en) <br>
**Javier Dottori** - Ph.D. student and Postdoc from 2012 to 2020, now Senior Software Engineer at [Glofox](https://www.glofox.com/) <br>
**Hugo Luis Manterola** - Ph.D. student and Postdoc from 2013 to 2019, now Software Developer at [Lamansys](https://lamansys.com.ar/) <br>
**Giulia Carbonari** - Ph.D. student from 2019 to 2021, now Ph.D. student at [ITBA](https://www.itba.edu.ar/) <br>
**Tomás Pérez Cambet** - Undergrad student from 2018 to 2020, now Software Development Engineer at [Salesforce](https://www.salesforce.com/mx/?ir=1) <br>
[**Lucas Lo Vercio**](http://www.pladema.net/llovercio/) - Ph.D. student and Postdoc from 2012 to 2017, now postdoc at University of Calgari (Canada) <br>
**Pablo Rubí** - Undergrad and Ph.D. student from 2016 to 2017), now Software Developer at Amazon (Seattle, USA) <br>
**Ezequiel Fernández Vera** - Undergrad student and Research Engineer (2015-2017), now Software Developer at [Lamansys](https://lamansys.com.ar/) <br>