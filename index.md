---
layout: default
title: Home
---

# International Congress on Mathematical Software

The “International Congress of Mathematical Software” (ICMS) is a community of researchers
and practitioners centered around “mathematical software” as a scientific activity. ... [more](/about/)

### ICMS Publications

ICMS conferences since 2006 have published with Springer: see [Conference proceedings list](https://link.springer.com/conference/icms).

### Upcoming Congress
* tbd


### Past Meetings
* [ICMS 2024](/2024/) - Durham (United Kingdom), 22-25 July 2024. [local website](https://maths.dur.ac.uk/icms2024)
* [ICMS 2020](/2020/) - Braunschweig (Germany), 13-17 July 2020. [local website](http://www.iaa.tu-bs.de/AppliedAlgebra/ICMS2020/ICMS2020.html)
* [ICMS 2018](/2018/) - South Bend (USA), Notre Dame, 24-27 July 2018
* [ICMS 2016](/2016/) - Berlin (Germany)], 11-14 July 2016 [local website](http://icms2016.zib.de/)
* [ICMS 2014](/2014/) - Seoul (Korea), 05-09 Aug 2014 [local website](http://voronoi.hanyang.ac.kr/icms2014/)
* [ICMS 2010](/2010/) - Kobe (Japan) [local website](http://www.math.kobe-u.ac.jp/icms2010/)
* [ICMS 2006](/2006/) - Castro Urdiales (Spain)] [local website](http://www.icms2006.unican.es/)
* [ICMS 2002](/2002/) - Beijing (China), Chinese Academy of Sciences [local website](http://www.mmrc.iss.ac.cn/icms/)

## News ([older news](news/))

{% for post in site.posts %}
    {% if forloop.index < 2 %}
	{% include post_link.html %}
    {% endif %}
{% endfor %}
