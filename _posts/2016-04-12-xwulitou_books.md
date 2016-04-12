---
layout: default
title: zz的书
books: [[['srqc_WPF.jpg', '深入浅出WPF'], ['wcf_gjbc.jpg', 'WCF高级编程'], ['asp.net web api.jpg', 'asp.net web api 2框架揭秘']
        ]]
---

zz的书
--------
{% for line in page.books %}
<div class='line' style="padding-left: 28px; height: 200px">
  {% for book in line %}
  <div class='content' style="float: left; padding-left: 6.9px; padding-right: 16.9px; min-width: 160px">
        <div class='img' style="text-align: center">
            <img src="{{site.baseurl}}/assets/images/{{book[0]}}" alt="{{book[1]}}" width="120" height="160" />
        </div>
        <div class='name' style="text-align: center">{{book[1]}}</div>
  </div>
  {% endfor %}
</div>
{% endfor %}
