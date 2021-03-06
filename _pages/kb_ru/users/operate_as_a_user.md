---
lang: ru
layout: article_with_sidebar
updated_at: '2018-08-30 15:07 +0300'
identifier: ref_1ZjmNEZf
title: Вход в магазин под учетной записью пользователя
order: 100
published: true
---
Иногда администратору магазина может понадобиться войти в магазин под учетной записью пользователя, например, чтобы разместить заказ от лица пользователя, исследовать проблему или проверить работу интерфейса. 

В X-Cart это возможно с помощью функции **Войти как клиент / Войти как администратор**:

   * [Вход в магазин как покупатель](#вход-в-магазин-как-покупатель)
   * [Вход в магазин как администратор](#вход-в-магазин-как-администратор)

## Вход в магазин как покупатель
Вход в магазин под учетной записью покупателя доступен администратору с полными правами на управление магазином или администратору с набором прав, включающим управление пользователями. 



   1. Откройте учетную запись покупателя.
   2. В меню **Действия с пользователем** нажмите **Войти как клиент**:
     ![1.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/1.png)
      В новой вкладке браузера откроется витрина магазина, в верхней части страницы будет уведомление **Вы вошли на сайт как _email покупателя_**. На странице будет находиться окошко с текстом **Вы вошли на сайт как: Покупатель _email покупателя_** и кнопкой **Завершить работу**:
      ![2.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/2.png)
   3. На открывшейся вкладке администратор действует как покупатель. Так как чаще всего администратор входит в магазин как покупатель, чтобы разместить от его лица заказ, понадобится оффлайн способ оплаты. Поэтому администратору, вошедшему в магазин как покупатель, доступен способ оплаты **Заказ по телефону**, даже если этот способ оплаты отключен в настройках магазина. Покупателям, дествующим в своих учетных записях, способ оплаты **Заказ по телефону** не доступен.
      
   4. Чтобы выйти из режима работы как покупатель, администратор нажимает **Завершить работу**:
      ![3.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/3.png)
Или возвращается на вкладку панели управления магазина и совершает любое действие, вызывающее перезагрузку страницы. Появится уведомление, что работа в учетной записи покупателя прекращена:
      ![4.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/4.png)

## Вход в магазин как администратор
Войти в магазин под учетной записью администратора может только админстратор с полными правами на управление магазином и администратор с правами на управление пользователями и управление администраторами.

Функция **Войти как покупатель / Войти как администратор** не дает доступ к учетной записи главного администратора магазина с полным набором прав управления.


   1. Откройте учетную запись администратора.
   2. В меню **Действия с пользователем** нажмите **Войти как администратор**:
      ![5.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/5.png)
   3. В новой вкладке браузера откроется панель управления магазина в том виде, в каком она доступна администратору, под чьей учетной записью осуществлен вход. 
   4. Чтобы выйти из учетной записи администратора, нажмите **Выход**.
   ![6.png]({{site.baseurl}}/attachments/ref_1ZjmNEZf/6.png)
