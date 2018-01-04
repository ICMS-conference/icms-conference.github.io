---
layout: default
title: Home
---

# International Congress on Mathematical Software

The “International Congress of Mathematical Software” (ICMS) is a community of researchers
and practioners centered around “mathematical software” as a scientific activity. ... [more](/about/)

### Upcoming Congress

* [ICMS 2018 - South Bend (USA)](http://icms-conference.org/2018) Notre Dame, 24-27 July 2018

### Past Meetings
* [ICMS 2016 - Berlin (Germany)](http://icms2016.zib.de/)
* [ICMS 2014 - Seoul (Korea)](http://voronoi.hanyang.ac.kr/icms2014/)
* [ICMS 2010 - Kobe (Japan)](http://www.math.kobe-u.ac.jp/icms2010/)
* [ICMS 2006 - Castro Urdiales (Spain)](http://www.icms2006.unican.es/)
* [ICMS 2002 - Chinese Academy of Sciences (China)](http://www.mmrc.iss.ac.cn/icms/)

## News ([older news](news/))

{% for post in site.posts %}
    {% if forloop.index < 8 %}
	{% include post_link.html %}
    {% endif %}
{% endfor %}

<p>&copy; {{ site.time | date: '%Y' }}. All rights reserved.</p>
