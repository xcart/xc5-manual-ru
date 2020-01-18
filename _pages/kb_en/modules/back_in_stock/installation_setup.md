---
lang: en
layout: article_with_sidebar
updated_at: '2018-07-06 15:59 +0400'
identifier: ref_7mZJltoM
title: Addon Installation and Setup
order: 100
published: true
redirect_from:
  - /modules/back_in_stock/module_setup.html
---
To install the addon **Back in Stock Notifications**, follow the instructions from {% link "Installing addons from the X-Cart App Store" ref_Vn1mMUw9 %}.

Once the addon has been installed, proceed to the addon settings page to configure the addon.
![540-settings-link.png]({{site.baseurl}}/attachments/ref_7mZJltoM/540-settings-link.png)

The addon configuration consists of the 2 main parts:
{% toc %}

## Configuring the Addon General Settings

The addon settings page looks as follows:
![540-settings-page.png]({{site.baseurl}}/attachments/ref_7mZJltoM/540-settings-page.png)

Here you can adjust the following settings:

* **Send Back in stock notifications every** : Use this field to set the frequency with which your store should send notifications to customers.
* **Allow customers to subscribe to back in stock notifications** : If this setting is enabled, your customers will be able to subscribe to the back-in-stock notifications for products that have gone out of stock.
* **Allow customer to specify the product quantity they want to buy** : If this setting is enabled, your customers will be able to specify the quantity of product units they wish to buy. They will receive a notification only if the product inventory level is enough to cover their request.
* **Allow customers to subscribe to price drop notifications** : If this setting is enabled, your customers will be able to subscribe to price drop notifications for products.
* **Allow customer to specify the price they want to pay** : If this setting is enabled, your customers will be able to specify the price they are ready to pay for the product. They will receive a notification only if the price changes to meet the request.

After adjusting the settings, be sure to save the changes to make them active.

{% note info %}
Make sure that out-of-stock items are visible in the storefront, otherwise your customers will not be able to sing up to back in stock notification subscriptions for them. To enable the display of out-of-stock items, ensure that the setting **How to show out of stock products** on the **Store setup** -> **Cart & Checkout** page is set to either _Show in all the sections_ or _Show only in categories and search listings_.
{% endnote %}

## Configuring the Related Email Notifications

The addon settings page allows a store admin to proceed to editing the back-in-stock and price drop notifications using the corresponding links at the bottom of the page. 
![540-edit-notifications-buttons.png]({{site.baseurl}}/attachments/ref_7mZJltoM/540-edit-notifications-buttons.png)

{% note info %}
Email notifications can also be {% link "edited" ref_1qTqS245 %} in the **Store setup** -> **Email notifications** section of the admin area. 
{% endnote %}

To edit the notifications a cart admin should click either the _Edit back in stock notification_ or _Edit price drop notification_ link to be redirected to the notifications maintenance page. 

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![540-notification-1.png]({{site.baseurl}}/attachments/ref_7mZJltoM/540-notification-1.png)</div>
  <div class="column" markdown="span">![540-notification-2.png]({{site.baseurl}}/attachments/ref_7mZJltoM/540-notification-2.png)</div>
</div>

Here the admin can enable/disable the notifications using the **State** ON/OFF trigger and change the message that is sent to the customers in the **Text** field if required. When the work is done it will be necessary to **Save changes**.

For more info on editing the email notifications, see {% link "Email Notifications: Setup and Maintenance" ref_5QLrLCu7 %}.
