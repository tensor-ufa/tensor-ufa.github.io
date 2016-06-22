---
layout: page
title: 23 июня 2016
excerpt: 
comments: true
---

Доклады
-------

<ul class="post-list">
{% for post in site.categories.talks %}
  {% if post.author %}
    {% capture authorslist %}
      {% for a in post.author %}
        {% assign author = site.data.authors[a] %}
        {% if author %} {{ author.name }}{% if author.company %}, {{ author.company }}{% endif %}{% endif %}{% unless forloop.last %};{% endunless %}
      {% endfor %}
    {% endcapture %}
  {% endif %}
  {% if post.announce %}
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}, {{ authorslist }}</a></li>
  {% endif %}
{% endfor %}
</ul>

Когда
-----

Первая встреча пройдет в **четверг**, 23 июня 2016 в 19:00. 

На все доклады отведено приблизительно 2 часа. Между докладами запланирован 10-минутный кофе-брейк, чтобы вы могли перекусить. А после докладов состоится after-party, где можно будет пообщаться на свободные темы — не расходитесь :)

Чтобы мы могли оценить количество участников, пожалуйста, [зарегистрируйтесь][register].

Где
---

Встреча пройдет по адресу: г. Уфа, Верхнеторговая площадь, 2, Отель Holiday Inn Ufa

Центральный вход.
Маршрут от остановки общественного транспорта указан на карте.

Места для парковки автомобилей указаны на карте зеленым цветом. Припарковаться можно: на парковке перед Гостиным двором, перед 8м корпусом УГАТУ или прямо у гостиницы. Парковка *бесплатная*. После проведения мероприятия необходимо сбросить время у пропуска стоянки на ресепшене.


Контактные телефоны: +7 960 800 08 08 Дарья

<script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?sid=07cEbZAuz88f1MHBau5pUv2p-tKHd60J&width=630&height=630&lang=ru_RU&sourceType=constructor&scroll=true"></script>

<!--
<ul class="post-list">
{% for post in site.posts limit:10 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
-->

[register]: /register/
[tensor]: http://tensor.ru/
[speakers]: /speakers/
