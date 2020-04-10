---
layout: page
title: "Участки в продаже" 
permalink: /sales/
order: 0
---
<p>В данном разделе Вы можете ознакомиться с доступными участками и ценами на них. В нашем посёлке "Премиум Парк" действует гибкая ценовая политика и мы уверены что сможем предложить вам лучшие условия на участок в Сергиевом-Посаде!</p>
<div class="alert alert-warning" role="alert">
Последнее обновление 10 апреля 2020 года
</div>
<table class="table table-hover text-center">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Площадь (м²)</th>
      <th scope="col">Кадастр</th>
      <th scope="col">Цена (🇷🇺)</th>
      <!-- <th scope="col">Действия</th> -->
    </tr>
  </thead>
  <script>
</script>
  <tbody>
{% for sector_hash in site.data.output %}
{% assign sector = sector_hash %}
    <tr>
      <th scope="row">{{ sector.num }}</th>
      <td>{{ sector.area }}</td>
      <td>{{ sector.kadastr }}</td>
      <td>{{ sector.price  }} ₽</td>
      <!-- <td><a href="{{ sector.link }}"><button type="button" class="btn btn-sm btn-secondary">Посмотреть на карте</button></a>&nbsp;<button type="button" class="btn btn-primary btn-sm openBtn">Забронировать</button></td>-->
    </tr>
{% endfor %}
  </tbody>
</table>
<div class="modal fade" id="myModal" role="dialog">
    <div class="modal-dialog">
        <!-- Modal content-->
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal">&times;</button>
                <h4 class="modal-title">Modal with Dynamic Content</h4>
            </div>
            <div class="modal-body">

            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
            </div>
        </div>
    </div>
</div>

