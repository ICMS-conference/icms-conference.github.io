---
layout: default
title: Home
---

# International Congress on Mathematical Software

The “International Congress of Mathematical Software” (ICMS) is a community of researchers
and practioners centered around “mathematical software” as a scientific activity. ... [more](/about/)

### ICMS Publications

ICMS conferences since 2006 have published with Springer: see [Conference proceedings list](https://link.springer.com/conference/icms).

### Upcoming Congress

* ICMS 2022

### Most recent Congress

* [ICMS 2020](/2020/) - Braunschweig, 13-17 July 2020. [local website](http://www.iaa.tu-bs.de/AppliedAlgebra/ICMS2020/ICMS2020.html)

### Past Meetings
* [ICMS 2018 - South Bend (USA)](/2018/) Notre Dame, 24-27 July 2018 
* [ICMS 2016 - Berlin (Germany)](http://icms2016.zib.de/) ([local copy](/2016/))
* [ICMS 2014 - Seoul (Korea)](http://voronoi.hanyang.ac.kr/icms2014/) ([local copy](/2014/))
* [ICMS 2010 - Kobe (Japan)](http://www.math.kobe-u.ac.jp/icms2010/) ([local copy](/2010/))
* [ICMS 2006 - Castro Urdiales (Spain)](http://www.icms2006.unican.es/) ([local copy](/2006/))
* [ICMS 2002 - Chinese Academy of Sciences (China)](http://www.mmrc.iss.ac.cn/icms/) ([local copy](/2002/))

## News ([older news](news/))

{% for post in site.posts %}
    {% if forloop.index < 8 %}
	{% include post_link.html %}
    {% endif %}
{% endfor %}
