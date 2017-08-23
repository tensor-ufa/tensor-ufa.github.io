---
layout: page
title: 14 сентября 2017
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

Вот так, незаметно, подобралась и третья встреча программистов в Уфе, которая пройдет в **четверг**, 14 сентября 2017 с 19.00 до 22.00

На все доклады отведено приблизительно 3 часа. Между докладами запланирован 10-минутный кофе-брейк, чтобы вы могли перекусить. А после докладов состоится after-party, где можно будет пообщаться на свободные темы — не расходитесь :)

Чтобы мы могли оценить количество участников, пожалуйста, [зарегистрируйтесь][register].

Где
---

Встреча пройдет по адресу: г.Уфа, ул.Менделеева 134/7,  [БЦ Территория 3000][place]

Центральный вход, 3 этаж

Маршрут от остановки общественного транспорта указан на карте.

Места для парковки автомобилей указаны на карте зеленым цветом.


Контактные телефоны: +7 960 800 08 08 Дарья

<script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?um=constructor%3A9d2543421718b1f17a67800b32bcf55128119cb491f29743f021b6a978dbe0cc&amp;width=834&amp;height=720&amp;lang=ru_RU&amp;scroll=true"></script>

<!--
<ul class="post-list">
{% for post in site.posts limit:10 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
-->

[register]: /register/
[place]: http://territory3000.ru/
[tensor]: http://tensor.ru/
[speakers]: /speakers/
