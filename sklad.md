# Склад ТМЦ

Функционал модуля "Склад" представляет собой набор таблиц, в которые заносятся данные. Каждый пункт меню это таблица, удобная в отображении для определенной цели.   

1. Для начала заполните таблицу "Приходные накладные". Это можно сделать, нажав на "+" справа над таблицей.    
- Дата поставки подставляется автоматически датой, когда создается накладная, но при необходимости эту дату можна изменить.   
- Выберете из списка поставщика. Если список пуст, перейдите на вкладку "Поставщик/Производитель" и создайте поставщиков, нажав на "+" и заполнив обязательное поле. Поле телефона поставщика не обязательное.   
- Филиал подставляется автоматически, но возможно изменить.
- Принимающий поставку подставляется автоматически при сохранении накладной из данных о пользователе, который добавил накладную.
- Следующие поля не обязательны для заполнения.
- После создания самой накладной нужно заполнить ее содержимое.
    - Нажмите на нужную строку с накладной, откроется новая таблица.   
    - Выберете из списка нужный вид материала. Если список пуст, <button class="btn btn-link" onclick='showText()'>заполните</button> таблицу на вкладке "Номенклатура". <div style='display:none' id='myDiv'>Введите название материала, выберите из списка единицу измерения, а так же производителя (заполняется на вкладке "Поставщик/Производитель")</div>
    - Введите количество поставленного материала.
    - Выберете кратную единицу измерения.
    - Остальные поля заполняются необязательно. Сумма считается автоматически из расчета цены за штуку и количества.
    - Нажмите на значок "дискета" над таблицей, чтобы сохранить все созданные строки.


<script>let show = false; let el = document.getElementById('myDiv');  function showText(){show = !show;if(show){el.style.cssText = 'display:block';}else{el.style.cssText = 'display:none'}}</script> 