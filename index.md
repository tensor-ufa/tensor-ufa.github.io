---
layout: page
title: 13 сентября 2018
excerpt:
comments: true
---

*Сентябрь - месяц айтишных праздников. Приглашаем отметить **День программиста** вместе с нами :)*

Мы расскажем, как уместили в одном решении 20 различных приложений, которыми пользуется каждая 2-я российская компания!  А также, как добиться высокого коэффициента «переиспользования» кода… Ведущие JS разработчики компании «Тензор» поделятся уникальным опытом на UTF 18!

И, конечно, как без подарков! Тебя ждет сюрприз – праздничная лотерея с памятными призами!

[**Регистрируйся**][register] и приходи – мы ждем тебя!


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
  <li><a href="{{ site.url }}{{ post.url }}"><b>{{ post.title }}</b><br/>{{ authorslist }}</a></li>
  {% endif %}
{% endfor %}
</ul>

Когда
-----

Итак, 13 сентября в 18:30 состоится четвертая встреча программистов в рамках UTF – 2018.  На все доклады отведено 3 часа. Между выступлениями запланирован 10-минутный кофе-брейк, чтобы вы могли перекусить. А после, приходи на after-party, где можно будет пообщаться на свободные темы — не расходитесь :)

Дата: 13/09/2018, четверг.

Время: с 18.30 до 21.30.


Где
---

Встреча пройдет в отеле Holiday Inn – конференц-зал «Шаляпин», Центральный вход, 1 этаж. По адресу: Россия, Республика Башкортостан, Уфа, Верхнеторговая площадь, 2. 

Маршрут от остановки общественного транспорта указан на карте.

Места для парковки автомобилей указаны на карте зеленым цветом.

Контактные телефоны: +7 909 249 11 00, Мария


<script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?sid=07cEbZAuz88f1MHBau5pUv2p-tKHd60J&width=834&height=834&lang=ru_RU&sourceType=constructor&scroll=true"></script>

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
