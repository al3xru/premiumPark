---
layout: page
title: "Участки в продаже" 
permalink: /sales/
order: 0
---
<p>В данном разделе Вы можете ознакомиться с доступными участками и ценами на них. В нашем посёлке "Премиум Парк" действует гибкая ценовая политика и мы уверены что сможем предложить вам лучшие условия на участок в Сергиевом-Посаде!</p>
<div class="alert alert-warning" role="alert">
Список участков пополняется
</div>
<table class="table table-hover text-center">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Площадь (м²)</th>
      <th scope="col">Цена (🇷🇺)</th>
      <th scope="col">Действия</th>
    </tr>
  </thead>
  <tbody>
{% for sector_hash in site.data.output %}
{% assign sector = sector_hash %}
    <tr>
      <th scope="row">{{ sector.num }}</th>
      <td>{{ sector.area }}</td>
      <td>{{ sector.price }} ₽</td>
      <td><button type="button" class="btn btn-sm btn-secondary">Посмотреть на карте</button>&nbsp;<button type="button" class="btn btn-primary btn-sm">Забронировать</button></td>
    </tr>
{% endfor %}
  </tbody>
</table>
