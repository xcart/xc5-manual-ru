---
lang: ru
layout: article_with_sidebar
updated_at: '2018-06-13 14:34 +0400'
identifier: ref_1EpoZue8
title: Многовалютность (Multicurrency)
order: 280
published: true
---
Если магазин предлагает товары покупателям за пределами Российской Федерации, модуль [Многовалютность (Multicurrency)](https://market.x-cart.com/addons/multicurrency-for-xcart5.html "Многовалютность (Multicurrency)") необходим: покупатели из других стран быстрее принимают решение о покупке, когда видят цены товаров в валюте своей страны.

{% note info %}
Для работы модуля **Многовалютность (Multicurrency)** требуется модуль [Geolocation](https://market.x-cart.com/addons/geolocation.html "Многовалютность (Multicurrency)"), подключающий бесплатную базу данных геопозиционирования IP-адресов **GeoLite2 Country** от **MaxMind**. Модуль определяет местонахождение посетителя магазина по IP адресу. Администратор может загрузить другую базу в настройках модуля **Geolocation**.

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![1.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/1.jpg)
</div>
  <div class="column" markdown="span">![2.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/2.jpg)
</div>
</div>
{% endnote %}

{% toc %}

## Установка модуля

В _X-Cart Бизнес_, _X-Cart Мультивендор_ и _X-Cart Всё включено_ модуль доступен для установки в Маркетплейсе. В _X-Cart Базовый_ установить модуль нельзя, чтобы настроить несколько валют в магазине, следует приобрести лицензию на _X-Cart Бизнес_, _X-Cart Мультивендор_ или _X-Cart Всё включено_ и {% link "установить модуль из Маркетплейса" ref_gpeZtm28 %}.


## Настройка многовалютности магазина

После установки модуля в разделе **Настройка магазина / Локализация** появляется вкладка **Валюта**.

![3.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/3.jpg)

* **Скрыть нули в дробной части**  - Если опция включена, отображается только целая часть цены; если опция отключена - отображается дробная часть после запятой.
* **Онлайн сервис курса валют** - Выберите онлайн-сервис или значение **Отсутствует**, чтобы устанавливать курс валют вручную.
* **Обновлять курсы валют каждый(е)** - Выберите временной промежуток автоматического обновления курса валют.
* **Добавить валюту** - Выберите из списка дополнительную валюту магазина и нажмите **Добавить валюту**. Добавленная валюта появится в списке ниже.

Для валюты указаны страны, в которых действует эта валюта. Список стран можно изменить - нажать на крестик для удаления страны или нажать внутри поля для добавления страны. Одна страна может быть выбрана только для одной валюты.

![4.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/4.jpg)

Стандартная валюта магазина отмечена в списке. Если вы установили другую валюту в качестве стандартной, сохраните это изменение и нажмите **Обновить курс**.

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![5.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/5.jpg)
</div>
  <div class="column" markdown="span">![6.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/6.jpg)
</div>
</div>

## Выбор валюты в магазине

После установки и настройки модуля валют в магазине появляется поле выбора страны, валюты и языка:

![7.jpg]({{site.baseurl}}/attachments/ref_1EpoZue8/7.jpg)

Страна, валюта и язык предустановлены по IP адресу покупателя. Выбор языка возможен, только если в магазине установлены модули перевода интерфейса. Если для местоположения покупателя не найдены валюта и язык, будут использованы стандартные валюта и язык магазина.

{% note warning %}
Валюта оплаты заказов зависит от настроенного в магазине платёжного сервиса. Одни платёжные системы позволяют оплату заказов только в стандартной валюте магазина, другие - в любой валюте. Уточние эту информацию в поддержке платёжной системы.
{% endnote %}
