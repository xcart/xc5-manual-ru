---
lang: en
layout: article_with_sidebar
updated_at: '2017-09-11 16:00 +0400'
identifier: ref_ST1QnErC
title: Configuring the Addon 'Mailchimp Integration with E-commerce Support'
order: 300
published: true
---
The settings and preferences for the addon "Mailchimp Integration with Ecommerce support" can be adjusted on the addon settings page in your X-Cart store’s Admin area.

The "Mailchimp Integration with Ecommerce support" addon configuration consists of 2 main steps:
{% toc %}

## Mailchimp Settings Configuration

The basic addon configuration settings are adjusted in the **Mailchimp settings** tab of the settings page:
![settings-tab.png]({{site.baseurl}}/attachments/ref_ST1QnErC/settings-tab.png)
   
   * **Mailchimp API key**: The API key that was used to connect your X-Cart store to your Mailchimp account. If, for some reason, you need to use a different Mailchimp account or a different key, use the "Reset Mailchimp connection" link.
   
   * **Enable E-commerce analytics**: This option enables E-commerce analytics by Mailchimp for your X-Cart store. For details, see the article [Use Mailchimp for E-Commerce](http://kb.mailchimp.com/integrations/e-commerce/use-mailchimp-for-e-commerce "Use Mailchimp for E-Commerce") in Mailchimp Knowledge Base. E-commerce analytics is the core component of the integration functionality; the setting is enabled by default, and we recommend keeping it that way. For E-commerce analytics related features to function properly, you will need to upload your store data (your store catalog and orders) to Mailchimp via the **E-Commerce features setup** section of the addon settings page. (This section appears on the page after you update Mailchimp lists). Be sure to visit the E-Commerce features setup section and specify the lists for which [Ecommerce Stores](https://developer.mailchimp.com/documentation/mailchimp/reference/ecommerce/stores/) need to be created on the Mailchimp end. See the instructions for [E-Commerce features setup](#E-Commerce_features_setup) further below. 
    {% note info %}
    Be sure also to enable [E-Commerce Link Tracking](http://kb.mailchimp.com/integrations/e-commerce/use-mailchimp-for-e-commerce "Use MailChimp for E-Commerce") for your campaigns and automations in your Mailchimp account back end.
    {% endnote %}
   
   * **Enable Abandoned Carts**:  This option enables the Abandoned Carts feature. For more info on this feature, see the [Mailchimp site](https://mailchimp.com/features/abandoned-cart/ "Abandoned Cart")
   
   * **Default list for automatic campaigns**: Specify the default list for automatic campaigns. This is needed for the abandoned carts and order notifications features to function properly for all your customers. (Failure to specify a list in this field will result in that Mailchimp abandoned carts and order notifications will work only for those customers who are already Mailchimp subscribers for this store). 
     
     To adjust this setting: 
     1) Go to the section **E-Commerce features setup** of the addon settings page, select the lists you require and upload store data for the selected lists to Mailchimp. 
     2) Go back to the **Mailchimp settings** section; in the "Default list for automatic campaigns" field, select the list for which abandoned carts and/or order notifications have been configured in Mailchimp. 
   
   * **Enable single opt-in for customers**: This setting defines whether customers who opt in to subscribe to your news lists should be asked to confirm the subscription via email, or not. When this option is disabled, new subscribers get an email with a subscription confirmation link that they need to click to be added to your list (Double opt-in). When this option is enabled, new subscribers are added to your list as soon as they opt in, without having to confirm the subscription by email (Single opt-in). Remember that abusing the single opt-in option may get your account banned by MailChimp.
   
* **Subscription select element type** (_Type:checkbox_ or _Type:select box_): This setting defines the way your customers select a subscription. If the select box option is enabled here, your customers can subscribe to only one mail list; if the checkbox option is enabled, your customers can subscribe to multiple lists.

* **Update Mailchimp lists every** (_Never, 1 minute, 10 minutes, etc._): Select the time interval for the periodical list updates.

* **Type of discount coupons that should be uploaded to Mailchimp**: Adjust this setting to specify the type of coupons that Mailchimp should be able to pull from your store for use in your campaigns via [promo code content blocks](https://mailchimp.com/help/use-promo-code-content-blocks/). 
   {% note info %}
   This setting is available only if the addon [Coupons](https://market.x-cart.com/addons/discount-coupons.html) is installed and active.
   {% endnote %}
   The available options are:
   * _All discount coupons:_ Select this option if you would like to be able to use with Mailchimp any coupons created in your X-Cart store.
   * _Only the discount coupons that match the Mailchimp promo rules:_ Select this option if you need Mailchimp to be able to import only the coupons that have been configured with the following fields defined (all the four of them, or just some of them): 
     - Code;
     - Discount amount;
     - Active from;
     - Active till.
       
       Discount coupons configured using any fields on top of this set (for example, a coupon for which a product category or a product class has been specified) will not be imported into Mailchimp.
  
* **Site connection code**: This is the field where your mc.js connection code snippet needs to be added. Once added via this field, the snippet is installed on your store website so that MailChimp can insert javascript for features. Namely, mc.js is needed so your store website can display this block: https://mailchimp.com/features/custom-forms/. In most cases, you will not have to add the mc.js code snippet via this field manually: the snippet will appear in this field automatically as soon as your store has been fully connected to Mailchimp. The connection process is considered fully completed after your store data has been [uploaded to Mailchimp](#e-commerce-features-setup). After the completion of the connection process, you see your connected store in your Mailchimp account and can access the respective settings:
   ![xc5_mailchimp_store_connected.png]({{site.baseurl}}/attachments/ref_ST1QnErC/xc5_mailchimp_store_connected.png)
   
   By this point, the field "Site connection code" on the Mailchimp addon settings page in your X-Cart store should already contain the mc.js code snippet you require. All you need to do is just to make sure it is there.

   {% note warning %}
   Attention users upgrading from an older Mailchimp integration version _without_ the "Site connection code" field to a newer version _with_ this field: 

   After the upgrade, the Mailchimp addon settings page in your X-Cart store Admin area will have the new field, but the snippet will not be there as you have already completed the store connection process before the upgrade. To get the snippet in place, you will need to update your store data using the button **Update store data** in the **E-Commerce features setup** section; after that the mc.js code snippet should appear in the "Site connection code" field automatically. 
   
   An alternative method will be to add the code snippet in the "Site connection code" manually. The code snippet can be found in your Mailchimp account via your connected store settings:
   ![xc5_mailchimp_code.png]({{site.baseurl}}/attachments/ref_ST1QnErC/xc5_mailchimp_code.png)
   {% endnote %}

When all the settings have beed specified, click the **Submit** button at the bottom of the page to make them active. 

After that you need to update the mailchimp lists by clicking the **Update Mailchimp Lists** button:
![update-lists-button.png]({{site.baseurl}}/attachments/ref_ST1QnErC/update-lists-button.png)

This is required to make the **E-Commerce features setup** tab visible.

## E-Commerce Features Setup

Once the lists have been updated, you need to go to the **E-Commerce features setup** section and upload your store data to Mailchimp. 
![ecommerce-features.png]({{site.baseurl}}/attachments/ref_ST1QnErC/ecommerce-features.png)

Uploading your store data to Mailchimp enables you to take full advantage of Mailchimp Product Recommendations and Abandoned Carts. For the best performance of these features, the products, orders, carts and customers from your ecommerce store need to be uploaded to Mailchimp and organized as a [Store](https://developer.mailchimp.com/documentation/mailchimp/reference/ecommerce/stores/). On the Mailchimp end, a Store is the top-level e-commerce resource. Carts, Customers, Orders, and Products all exist inside of the scope of a Store. 

Each Store in Mailchimp needs to be tied to a Mailchimp list. 

In the **E-Commerce features setup** section of the addon settings page in X-Cart, you specify the lists for which Mailchimp Stores need to be created and initiate the upload/syncing of store data. 

First, you need to select the check boxes for the lists you require and click **Update**. This saves the set of MailChimp lists for which Stores should be created. 

To initiate the upload of store data for the selected lists, click **Upload store data to Mailchimp**. Mailchimp will create the Stores and will connect them to the Mailchimp lists you have specified. Store data from X-Cart will be uploaded to these specific Stores. After the initial synchronization, further synchronization of store data will be done on the go automatically, without the need to click the **Upload store data to Mailchimp** button; for example, when a new cart or a new order are created in your X-Cart store, the respective information will be automatically submitted to Mailchimp. 

The button **Upload store data to Mailchimp** remains in the **E-Commerce features setup** section just in case you need to redo the synchronizion; for example, you may need to use the button again if things get desynchronized between your store and your Mailchimp account after you disable the addon in X-Cart temporarily. 

Another button - **Update store data** - will help you to update your company information on the Mailchimp end (for example, if your company name or address change).

_Related pages:_

*   {% link "Getting started with 'Mailchimp Integration with E-commerce support'" ref_w5MRyybe %}
