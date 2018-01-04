---
layout: default2018
title: ICMS 2018 - Notre Dame
---

# International Congress on Mathematical Software - ICMS 2018
## Notre Dame, 24-27 July 2018

**General Chair**: [James H. Davenport](http://people.bath.ac.uk/masjhd/)

**Program Chairs**: 
[Manual Kauers](http://www.kauers.de/), 
[George Labahn](https://cs.uwaterloo.ca/~glabahn/), and
[Josef Urban](https://www.ciirc.cvut.cz/~urbanjo3/).

**Local Chairs**: [Jonathan Hauenstein](https://www3.nd.edu/~jhauenst/), [Andrew Sommese](https://www3.nd.edu/~sommese/) 

## News ([older news](/news/))

{% for post in site.posts %}
    {% if forloop.index < 8 %}
        {% include post_link.html %}
    {% endif %}
{% endfor %}


<p>&copy; {{ site.time | date: '%Y' }}. All rights reserved.</p>
