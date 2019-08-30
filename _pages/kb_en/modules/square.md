---
lang: en
layout: article_with_sidebar
updated_at: '2019-08-29 11:17 +0400'
identifier: ref_5kZcVsK7
title: Square
order: 269
published: true
---
The addon [Square Payments](https://market.x-cart.com/addons/square.html "Square") provides an integration with Square, a PCI compliant payment solution. Square is compatible with all types of devices: desktop, tablet and mobile and also supports offline in-person payments. Square payment is integrated with X-Cart via Square API that keeps customers on your site during checkout and credit card data submission.

The integration is available for the US, Canada, Japan, Australia and the UK.

{% toc %}

## Square Account Setup

Prior to configuring the Square Payments addon in the Admin area of your X-Cart based store, you'll need to sign up for Square to get and account that provides access to Square Developer Dashboard where you'll find all the necessary data for the addon configuration in your store admin.

1. To create an account with Square start with a regular [Square sign up](https://squareup.com/t/f_partnerships/d_partnerships/p_xcart/c_general/o_none/u_partnersite?route=signup "Square") link or use the **Start a Square account button** at [https://squareup.com/us/en](https://squareup.com/us/en "Square").
   * You'll need specify your e-mail (will be used as an account ID), set a password and choose your business locale. Also it will be necessary to agree to to Square’s terms, privacy policy, and e-sign consent:
     ![square-sign-up.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/square-sign-up.png)
     Click **Continue** to do further.
   * Then you'll need to fill in the form with your business details (the form and fields to fill in differ depending on a particular country requirements).
     Click **Continue** to create an account with Square. 
     
     {% note info %}
     If you already have an account with Square sign in to access your Square Seller Dashboard.
     {% endnote %}

2. When the account creation is completed or when signed in you'll see your Square Seller Dashboard. Here you need to go to the **Apps** -> **My Apps** section to get access to your Developer Dashboard.
   ![square-client-dashboard.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/square-client-dashboard.png)
   * Click on **My Apps** in the **Apps** section:
     ![apps-my-apps.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/apps-my-apps.png)
     You'll see a new screen with a list of apps connected. 
   * Click the **Go to Developer Dashboard** button to be redirected to your developer dashboard. 
     ![go-to-developer-dash.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/go-to-developer-dash.png)
     Square Developer Dashboard is opened in a new tab. 

4. Click the **Create Your First Application** button (or **New Application**, if you already have some existing apps connected):
   ![create-app.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/create-app.png)
   
   * Name your application and agree to the Square Developer Terms of Service:
     ![new-application.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/new-application.png)
   * Click **Create Application** to complete the step.

5. Now you are inside the application and can get access to the data required to configure Square Payment in your store.
  
   To make the application work with your X-Cart based store switch the application API Version to 2019-02-13 on the **Credentials** page:
   * Scroll down the page to locate the **API Version** section:
     ![change-api-1.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/change-api-1.png)
   * Click on the **Change Version** button and choose v. **2019-02-13** in the drop-down:
     ![change-api-2.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/change-api-2.png)
   * If you want to test the payment integration first, leave the application in **Sanbox Mode**. To accept live payments you'll need to switch it to **Production**:
     <div class="ui stackable two column grid">
       <div class="column" markdown="span"><b>Sandbox Mode ON</b>![sandbox.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/sandbox.png)</div>
       <div class="column" markdown="span"><b>Production Mode On</b>![production.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/production.png)</div>
     </div>
     
6. Do not close the Square Developer Dashboard as you'll need to copy the application details to assign it to your X-Cart store. 

## Square Payments Addon Configuration

{% note warning %}
Make sure the [Square Payments](https://market.x-cart.com/addons/square.html "Square") addon is installed and enabled as described in {% link "Installing Addons from the X-Cart App Store" ref_Vn1mMUw9 %}.
{% endnote %}

To configure Square payments addon in your store Admin area:
1. Open the Square settings page:
   * Via the **Settings** link on the Square addon page in the **My Addons** section of your store Admin area:
     ![settings-link.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/settings-link.png)
   * Via the {% link "**Add payment method**" ref_36BqwVSF %} button in the **Store setup** -> **Payment methods** section of your store Admin area:
     ![add-payment.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/add-payment.png)
2. On the Square payment settings page choose the required application mode and fill in the related fields:
   ![settings-page.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/settings-page.png)
   
   **SANDBOX APPLICATION MODE**
   
    Sandbox application mode is used to test the Square payment configuration. 
     
    * Set the **Application mode** setting value to **Sandbox**.
       {% note info %}
       Make sure your Square Developer Dashboard is set to **Sandbox mode**.
       ![sandbox.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/sandbox.png)
       {% endnote %}
     * Fill in the following fields with the data from your Square Developer Dashboard:
       * **Sandbox Application ID** : Locate the Sandbox Application ID value on the **Square Developer** -> **Credentials** page, copy and paste it here.
         ![sandbox-application-id.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/sandbox-application-id.png)
       * **Sandbox Access Token** : Locate the Sandbox Access Token value on the **Square Developer** -> **Credentials** page, copy and paste it here.
         ![sandbox-access-token.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/sandbox-access-token.png)
       * **Sandbox Location ID** : Locate the Sandbox Location ID value on the **Square Developer** -> **Locations** page, copy and paste it here.
         ![location-id.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/location-id.png)
      * **Submit** the configuration settings.
   
   
   **PRODUCTION APPLICATION MODE**
   
   Production application mode is used to accept real payments in a live store. 
     
     * Set the **Application mode** setting value to **Sandbox**.
       {% note info %}
       Make sure your Square Developer Dashboard is set to the **Production mode**.
       ![production.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/production.png)
       {% endnote %}
     * Fill in the following fields with the data from your Square Developer Dashboard:
       * **Application ID** : Locate the Application ID value on the **Square Developer** -> **Credentials** page, copy and paste it here.
         ![application-id.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/application-id.png)
       * **Application Secret** : Locate the Application Secret value on the **Square Developer** -> **OAuth** page, copy and paste it here.
         ![application-secret.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/application-secret.png)
     * **Submit** the configuration settings.
     * Once the settings have been submitted, 2 (two) new tabs become available on the Square payment settings page of your store Admin area - **OAuth configuration** and **Locations configuration**. You need to configure settings in both of them.
       ![oauth+locations-tabs.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/oauth+locations-tabs.png)
       * **OAuth configuration** 
         * Open the **OAuth configuration** tab of the Square payment settings page:
           ![oauth-tab.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/oauth-tab.png)
         * Copy the URL from the **OAuth configuration** tab of the Square payment settings page using the **Copy** button and paste it to the **Redirect URL** field on the **Square Developer** -> **OAuth** page and **Save** the changes there.
         * Click on the **Get OAuth Token** button in the **OAuth configuration** tab of the Square payment settings page in your store Admin area. You'll be redirected to Square for authorization (you'll need to enter/confirm your login and password) and if passed directed back to the **Locations configuration** tab of the Square payment settings page in your store Admin area.
       * **Locations configuration**
         ![locations-tab.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/locations-tab.png)
         * On the **Locations configuration** tab of the Square payment settings page set the Square Location for Online Payments value from the select drop-down (the location value in the drop-down will be the Square application name you've set during the [Square account setup](https://kb.x-cart.com/modules/square.html#square-account-setup "Square"), that had been passed to X-Cart during the **OAuth configuration** step).
         * Click **Submit** to save the settings.

3. To activate the payment method switch it ON either on the Square settings page (**General configuration** tab) or in the list of online payment methods in the **Store setup** -> **Payment methods** section of your store Admin area.
   
   <div class="ui stackable two column grid">
       <div class="column" markdown="span"><b>Square Settings Page</b>![paymont-on-1.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/paymont-on-1.png)</div>
       <div class="column" markdown="span"><b>Payment Methods Page</b>![payment-on-2.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/payment-on-2.png)</div>
     </div>
  
  Once enabled the Square payment method will become available to customers at checkout. With Square payment customers can specify their credit card info directly on your X-Cart checkout page. This data will be securely transmitted to Square via token.
  ![cus-checkout.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/cus-checkout.png)

## Order Processing Workflow

Square payment integration allows a store admin to choose whether a payment should be captured automatically or should be authorized first. By default all payments are set to pre-authorization by a store admin.

The payment auto capture can be enabled in the **Payment configuration** tab of the Square payment settings page in the store Admin area:
![payment-configuration.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/payment-configuration.png)

Set the **Auto capture** setting value to **Yes** and click **Submit** to save the changes. 

The **Payment configuration** tab of the Square payment settings page also allows to enable logs recording for all Square related operation. Set the **Enable debug** setting to Yes for this ourpose and click **Submit** to save the changes. All logs will be stored to the **System tools** -> **System logs** section of your store Admin area. Square logs will have the square-debug.log.YYYY-MM-DD.php or square-error.log.YYYY-MM-DD.php format.

When an order is paid with Square payment it is registered in the **Orders** -> **Orders list** section of your store Admin area. 

If Square payment is configured to payment authorization the orders will have the 'Authorized' payment status and 'New' fulfilment status by default.

![order-auth.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/order-auth.png)

To process an order it will be necessary to click either the **Capture** button to accept the payment (the order status will be changed to **Paid**) or the **Void** button to reject the payment (the order status will be changed to **Cancelled**).

If Square payment is configured to capture payments automatically the orders will have the 'Paid' payment status and 'New' fulfilment status by default.

![order-paid.png]({{site.baseurl}}/attachments/ref_5kZcVsK7/order-paid.png)

A store admin can refund or partically refund a paid order by specifying the amount for refund in a special field on the order details page and clicking the **Refund**  button. The order will get the **Refunded** status in case of a full refund and **Partially paid** status in case of a partial refund. 

{% note info %}
More info about order payment and fulfilment statuses you can find in {% link "Understanding X-Cart Order Statuses" ref_DkbTi1qJ %}.
{% endnote %}



