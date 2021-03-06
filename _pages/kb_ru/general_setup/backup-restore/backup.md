---
lang: ru
layout: article_with_sidebar
updated_at: '2018-04-25 11:33 +0400'
identifier: ref_5V7w6uSs
title: Резервная копия файлов и базы данных магазина
order: 170
published: true
---
Администратор магазина X-Cart может создать резервную копию базы данных магазина в панели управления магазина. 

{% note warning %}
В резервную копию базы, созданную стандартными средствами X-Cart, не входят данные сторонних и созданных на заказ модулей, расположенные за пределами базы магазина.
{% endnote %}

Чтобы в дамп вошли все данные, следует делать резервную копию вручную. Воспользуйтесь версиями SSH протокола OpenSSH или PuTTY, Telnet, phpMyAdmin, консолью MySQL, панелью управления хостинга, удалённым рабочим столом и др. 

{% toc %}

## Создание резервной копии базы данных в панели управления магазина

Создание резервной копии базы данных в зоне администратора X-Cart:

 1. Войдите в панель управления магазина.
 2. Откройе раздел **Инструменты / База данных** и перейдите на вкладку **Сохранить базу**.
 ![1.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/1.jpg)
 3. На открывшейся странице выберите подходящую опцию: **Скачать SQL файл** или **Создать SQL файл**. 

{% note info %}
Если у вас нет доступа на сервер/хостинг по SSH или FTP, охраните SQL файл на компьютере.
{% endnote %}

## Создание резервной копии через терминал

1. Войдите в хостинг аккаунт или на сервер по терминальному доступу.

2. Откройте директорию, в которой установлен магазин X-Cart.

3. Запустите shell команду


```
mysqldump -h<db_host> -u<username> -p<password> -r<backup_filename> <db_name>
```

Сокращения в команде:

{:.ui.compact.celled.small.padded.table}
|db_host | DNS имя или IP адрес MySQL сервера|
|username | Имя пользователя в учётной записи MySQL|
|password | Пароль к учётной записи MySQL|
|backup_filename | Название резервной копии и путь к SQL файлу, содержащему дамп базы|
|db_name | Название MySQL базы магазина|


После запуска команды система создаёт SQL файл и сохраняет его в директории, указанной в команде. Если в команде указано только название директории и не указан путь к ней, файл будет сохранён в корневой директории X-Cart.

Рекомендуется расположение внутри корневой директории.

## Создание резервной копии файлов магазина

Резервное копирование файлов означает сохранение всех файлов корневой директории X-Cart в архиве и копирование или перемещение этого архива на удалённый сервер или локальный компьютер.

{% note info %}
Если дамп базы был сохранён в файле в корневой директории, он также будет включён в архив резервной копии файлов.
{% endnote %}

Для создания резервной копии файлов потребуется менеджер архивирования подходящий используемой операционной системе. Наиболее распространённый архиватор, установленный на большинстве UNIX серверов, - TAR. На Windows серверах работают архиваторы WinRAR, WinZIP, PKZip и 7Zip. Запакуйте все файлы корневой папки X-Cart в архив и сохраните этот архив в директории на уровень выше корневой папки магазина.

Если не удаётся создать архив на сервере, где установлен X-Cart, скопируйте корневую папку магазина на компьютер или другой сервер, например, по FTP. Перед копированием убедитесь, что на новом местоположении достаточно свободного места.
Также, хостинг провайдеры позволяют создавать резервные копии аккаунта через панель управления.

### Создание резервной копии файлов X-Cart с помощью архиватора TAR (для UNIX серверов)

В UNIX системах архиватор TAR считается самым надёжным средством создания и управления архивами. Обычно TAR используют с такими служебными программами для сжатия, как GZIP, BZIP2 и LZMA, которые позволяют не только создавать архив, но и сжимать данные внутри него. В результате, получается TAR-архив небольшого объёма, который можно открыть теми же средствами. Чтобы узнать, установлен ли TAR на сервере, запустите команду.

```
tar --version
```

Если архиватор установлен, появится сообщение с версией TAR, если не установлен - сообщение об ошибке. Обратитесь в поддержку хостинга для установки архиватора.

Создание TAR-архива с файлами магазина:

1. Войдите в хостинг аккаунт/на сервер.

2. Откройте корневую директорию магазина.

3. Запустите shell команду

```
tar -czvf ../store_backup.tgz *
```

После запуска команды TAR упакует все файлы корневой папки магазина в файл `store_backup.tgz` и уменьшит размер архива с помощью ZIP.  Архив будет сохранён в директории на уровень выше корневой папки X-Cart. Например, если корневая папка `u/user/public_html/xcart`, файл `store_backup.tgz` будет сохранён в `u/user/public_html`.

## Создание резервной копии с помощью модуля Мастер резервного копирования (Backup Master)

Модуль [Мастер резервного копирования (Backup Master)](https://market.x-cart.com/addons/backup-master.html "Files and Database Backup") упрощает процесс создания резервной копии X-Cart, т.к. создаёт одновременно резервные копии и базы и файлов магазин. 

В _X-Cart Всё включено_ модуль уже установлен и требует только {% link "активации" ref_IEo2gFuZ %} и настройки, а в _X-Cart Базовый, Бизнес_ и _Мультивендор_ модуль требует {% link "установки и активации" ref_gpeZtm28 %}. 

Откройте страницу настройки модуля.

![2.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/2.jpg)

Выберите один из способ создания резервной копии:
* Класс ZipArchive, встроенный в PHP
* Команды консоли Linux
* Команды консоли Linux (без сжатия)

{% note info %}
Команды консоли Linux - самый быстрый способ, поэтому он рекомендован для Linux серверов. ZipArchive может не справиться с объёмными файлами, на это единственный способ на Windows серверах.
{% endnote %}

Способ **Команды консоли Linux** выбран по умолчанию. Если вы выбрали другой метод, сохраните изменения. 

![3.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/3.jpg)

Для создани резервной копии откройте раздел **Инструменты / Backup** и нажмите **Создать резервную копию**.

<div class="ui stackable three column grid">
  <div class="column" markdown="span">![4.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/4.jpg)
</div>
  <div class="column" markdown="span">![5.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/5.jpg)
</div>
</div>

Модуль создаёт полную резервную копию магазина и сохраняет запись о ней в истории резервного копирования. В истории можно найти путь к файлу резервной копии, размер файла и дату создания. Чтобы удалить резервную копию, нажмите на значок корзины рядом с названием файла.
![6.jpg]({{site.baseurl}}/attachments/ref_5V7w6uSs/6.jpg)
