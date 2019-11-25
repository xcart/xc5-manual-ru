---
lang: en
layout: article_with_sidebar
updated_at: '2017-12-01 01:29 +0400'
identifier: ref_uEnDBBA7
title: Activating and Deactivating Addons
categories:
  - User manual
published: true
order: 100
redirect_from:
  - /modules/managing_modules/activating_and_deactivating_modules.html
  - /general_setup/managing_modules/activating_and_deactivating_modules.html
---
In X-Cart 5.3.x and earlier all manipulations with the software addons are performed directly in the store Admin area (**My Addons** section).

Starting from X-Cart 5.4.x the **My Addons** menu section in the store Admin area opens a special **Upgrade System** environment separate from the rest of the store. This was done to ensure that any changes applied to a store via new addons' installation or present addons' upgrade or deletion can be safely and easily rolled back in case of any malfunction.

Basically, since all X-Cart software functionality is added via the separate addons installation, the addons management consists of the addons activation and deactivation, and deletion. 

{% toc %}

## Activating Addons

Sometimes the addon you want to use is installed, but not active. To be able to use such an addon, you need to activate it. 

To activate an installed addon:

1.  In your store's Admin area, click **My addons** to go to the **My Addons** section:
    ![my_addons_link.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/my_addons_link.png)

2.  In this section, find the addon that needs to be activated (for example, **Add to Cart Popup**):
    ![addon2enable.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon2enable.png)

3.  Switch the On/Off trigger below the addon name to the "On" state and click the **Apply changes** button at the bottom of the screen. 
    ![addon_enable.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon_enable.png)

This starts the addon activation process which may take a while to complete. Once your store has been redeployed, you will find the addon active and ready to use:
    ![addon_enabled.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon_enabled.png)
    

## Deactivating Addons

It is possible to temporarily disable (deactivate) an installed addon.

{% note info %}
Deactivation stops the addon from operation, but it does not remove the settings you made to the addon configuration nor clear any data that was generated or collected during the period that the addon was in operation. If you wish to completely remove all the data related to using a certain addon, you need to uninstall it.
{% endnote %}

To deactivate an installed addon:

1.  In the **My Addons** section of your store's Admin area, find the addon that needs to be deactivated.

2.  Switch the On/Off trigger below the addon name to the "Off" state.
    ![addon_deactivate.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon_deactivate.png)

3.  Click **Apply changes**. This starts the addon deactivation process. Once your store has been redeployed, you will find the addon disabled.

## Uninstalling Addons

To uninstall (delete) addon you are not planning to use further:

1.  In the **My Addons** section of your store's Admin area, find the addon that needs to be uninstalled.

2.  Click on the **'Trash'** icon bellow the addon name.
    ![addon_delete.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon_delete.png)

3.  Click **Apply changes**. 
    ![addon_delete1.png]({{site.baseurl}}/attachments/ref_uEnDBBA7/addon_delete1.png)

This starts the addon deinstallation process. Once your store has been redeployed, the addon will be removed from your store.

{% note info %}
It is recommended to uninstall any addons that you do not use to facilitate the overall store performance.
{% endnote %}

_Related pages:_

*   {% link "Managing Addons" ref_gTOegEua %}
