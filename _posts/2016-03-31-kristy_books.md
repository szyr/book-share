---
layout: default
title: kristy的书
books: [[['dianpeiliuli.jpg', '愿有人陪你颠沛流离'], ['writeforfuture.jpg', '不要让未来的你讨厌现在的自己'],
         ['goutong.jpg', '有一种魔力叫沟通'], ['jianglaiguoqu.jpg', '不畏将来 不念过去']
        ]
       ]
---

kristy的书
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
