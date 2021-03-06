---
lang: ru
layout: article_with_sidebar
updated_at: '2018-06-07 00:28 +0400'
identifier: ref_4js5MsFN
title: Групповое редактирование товаров
order: 140
published: true
---
Модуль **Групповое редактирование товаров (Bulk Editing)** установлен и актвирован в **X-Cart Бизнес**, **X-Cart Всё включено** и **X-Cart Мультивендор**. В **X-Cart Базовый** этот модуль недоступен, чтобы использовать модуль, следует приобрести лицензию  **X-Cart Бизнес**, **X-Cart Всё включено** или **X-Cart Мультивендор**.

Настройка товаров подразумевает одинаковые действия с каждым товаром. Чтобы сэкономить время и избежать монотонной работы, воспользуйтесь функцией группового редактирования товаров в разделе **Каталог / Товары**.

![3.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/3.jpg)

В массовое изменение входит включение и отключение товаров, размещение товаров на распродаже, завершение распродажи, редактирование свойств товаров (категорий, тегов, цен, запаса и т.д.).

{% toc %}

## Включение и отключение товаров

* Отметьте товары, которые собираетесь включить или отключить
* Нажмите **Включить все** или **Отключить все**

  ![4.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/4.jpg)

## Распродажа товаров

 - _Размещение товаров на распродаже_:
* Выберите товары для распродажи
* Нажмите **Поместить на распродажу**
  ![5.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/5.jpg)
* Откроется окно настройки цены товара на распродаже: установите новую сниженную цену или скидку в процентах
  ![6.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/6.jpg)
 
- _Удаление товаров с распродажи_:
* Выберите товары из списка
* Нажмите **Удалить с распродажи** 

## Изменение категорий и тегов

* Выберите товары для редактирования
* Нажмите **Редактировать выбранные / Категории и теги**
  ![7.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/7.jpg)
* На открывшейся странице создайте, выберите, удалите или измените категории и теги товаров.
  * Нажмите на текстовое поле для выбора категории или тега для редактирования. Можно выбрать несколько значений
  ![8.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/8.jpg)

## Изменение размера запаса

* Выберите товары из списка
* Нажмите **Редактировать выбранные / Информация по наличию на складе** 
  ![9.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/9.jpg)
* На открывшейся странице внесите информацию о запасах выбранных товаров:
  ![10.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/10.jpg)
  
  {:.ui.compact.celled.small.padded.table}
  | Контроль остатков | Включите или отключите отслеживание изменения размера запаса |
  | Остаток | Укажите количество товара в наличии |
  | Показывать покупателям предупреждение о низком остатке товара | Включите или отключите уведомление для покупателей |
  | Уведомлять администратора при снижении остатка этого товара на складе до минимального предела | Включите или отключите уведомление для администратора |
  | Минимальный предел остатка | Укажите минимально возможное количество товар, при котором администратор получает напоминание, что запас товара необходимо восполнить |
  | Все покупатели | Укажите минимальное количество товара для покупки для вех покупателей |
  | Оптовые покупатели | Укажите минимальное количество товара для покупки для оптовых покупателей |

* Сохраните изменения 

## Изменение цен и доступности группам пользователей

* Выберите товары для редактирования
* Нажмите **Редактировать выбранные / Цена и доступность для групп**
  ![11.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/11.jpg)
* Настройте выбранные товары на открывшейся странице:
  ![12.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/12.jpg)
  
  {:.ui.compact.celled.small.padded.table}
  | Цена | Укажите цену товаров. Цена будет одинаковой для всех выбранных товаров |
  | Рыночная цена | Средняя стоимость товара в других магазинах. Это поле присутствует, только если в магазине активирован модуль [**Рыночная цена (Market Price)**](https://market.x-cart.com/addons/market-price.html "Групповое редактирование товаров") |
  | Участвует в распродаже | Включите или отключите опцию, чтобы поместить или удалить товары с распродажи |
  | Цена на распродаже | Установите сниженную цену в рублях или скидку в процентах|
  | Доступность только для этих групп пользователей | Добавьте, удалите или измените группу пользователей, представителям которой доступны выбранные товары |
  | Класс налога | Выберите налог, который будет налагаться на выбранные товары |

* Сохраните изменения 

## Изменение информации о доставке

* Выберите товары для редактирования
* Нажмите **Редактировать выбранные / Доставка** 
  ![13.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/13.jpg)
* Настройте доставку для выбранных товаров на открывшейся странице:
  ![14.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/14.jpg)
  
  {:.ui.compact.celled.small.padded.table}
  | Вес | Укажите вес товаров в килограммах |
  | Требуется доставка | Включите или отключите доставку товаров |
  | Бесплатная доставка | Включите или отключите бесплатную доставку товаров |
  | Исключить из расчета стоимости доставки | Никогда не рассчитывать стоимость доставки для выбранных товаров |
  | Фиксированная стоимость доставки | Укажите {% link "стоимость доставки" ref_ELG1SBUJ %} для выбранных товаров |
  | Отправка отдельной посылкой | Укажите, нужна ли отправка отдельной посылкой |
  | Длина / Ширина / Высота | Укажите размеры коробок для отправки выбранных товаров |
  | Макс. кол-во в посылке | Укажите, сколько товаров помещается в одной коробке |

* Сохраните изменения

## Изменение продавцов товаров в X-Cart Мультивендор

* Выберите товары, для которых необходимо установить продавца
* Нажмите **Редактировать выбранные / Продавец** - _этот пункт присутствует в меню **Редактировать выбранные** только в **X-Cart Мультивендор**_
  ![15.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/15.jpg)
* На открывшейся странице выберите продавца из списка и сохраните изменения
  ![16.jpg]({{site.baseurl}}/attachments/ref_4js5MsFN/16.jpg)

