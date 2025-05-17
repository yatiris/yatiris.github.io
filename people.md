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


* * *

### Past members

**Eugenia Moris** - PhD student (2025) - After finishing: Data Scientist at [Arionkoder](https:www.arionkoder.com/) <br>
**Camila García** - PhD student (2024) - After finishing: Data Scientist at [mediaire](https://www.linkedin.com/company/mediaire/) <br>
**Hernán Külsgaard** - PhD student (2024) <br>
**Tomás Castilla** - Research Intern - After finishing: Data Engineer at [Datalytics](https://www.datalytics.com/) (2022) <br>
**Lautaro Gramuglia** - Research Intern. (2022) <br>
**Rodrigo Cobo** - Undergrad student - After finishing: Data Scientist at [Globant](https://www.globant.com/en) (2021) <br>
**Francisco Iarussi** - Undergrad student and Research Trainee from 2020 to 2021 - After finishing: QA and Test Automation Engineer at [Globant](https://www.globant.com/en) (2021) <br>
**Javier Dottori** - Ph.D. student and Postdoc from 2012 to 2020- After finishing: Senior Software Engineer at [Glofox](https://www.glofox.com/) (2020) <br>
**Hugo Luis Manterola** - Ph.D. student and Postdoc from 2013 to 2019- After finishing: Software Developer at [Lamansys](https://lamansys.com.ar/) (2019) <br>
**Giulia Carbonari** - Ph.D. student from 2019 to 2021- After finishing: Ph.D. student at [ITBA](https://www.itba.edu.ar/) (2020) <br>
**Tomás Pérez Cambet** - Undergrad student from 2018 to 2020- After finishing: Software Development Engineer at [Salesforce](https://www.salesforce.com/mx/?ir=1) (2020) <br>
[**Lucas Lo Vercio**](http://www.pladema.net/llovercio/) - Ph.D. student and Postdoc from 2012 to 2017- After finishing: postdoc at University of Calgari (Canada) (2017) <br>
**Pablo Rubí** - Undergrad and Ph.D. student from 2016 to 2017 - After finishing: Software Developer at Amazon (Seattle, USA) (2017) <br>
**Ezequiel Fernández Vera** - Undergrad student and Research Engineer (2015-2017)- After finishing: Software Developer at [Lamansys](https://lamansys.com.ar/) (2017) <br>