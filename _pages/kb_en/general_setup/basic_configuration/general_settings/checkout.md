---
lang: en
layout: article_with_sidebar
updated_at: '2019-07-05 13:17 +0400'
identifier: ref_0I0Cpjkh
title: Checkout Setup
order: 100
published: true
---
Checkout is one of the most important processes in any store as business revenues depend directly on whether customers are able to complete the checkout process successfully. The goal of checkout is to gather the information necessary to complete the transaction. Hence your customers will use checkout pages to enter shipping and payment information for their orders. Nothing should distract them or make the information on the page hard to read, so it's best to keep the checkout page design simple. 

X-Cart offers a variety of ways to set up your store's checkout to best suit your business needs and even allows to disable checkout in the store if required. 

{% toc %}

## Checkout Type

A type of checkout that will be used in your store can be configured using the **Checkout type** setting on the **Store setup** -> **Cart&Checkout** -> **General** page of X-Cart Admin area.
![541-cart-and-checkout-page.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/541-cart-and-checkout-page.png)

X-Cart offers 2 possible chechout types by default:
* Fast Lane Checkout
* One Page Checkout 

Choose the checkout type you prefer and click **Submit** to activate it in the storefront.

### Fast Lane Checkout

Fast Lane Checkout (FLC) is a type of checkout when all steps of data submission are divided into pages, i.e. a customer submits the personal data, chooses the preferred delivery and payment methods in series, each next step becoming available only if all the required fields of the previous step are filled in properly. FLC is considered more straightforward for a new custome as it potentially leads to fewer errors during the data submission for the transaction because all necessary info is filled in portions of 2-3 forms of small scape.

This is how the FLC type of checkout will look for an unregistered and not logged in customer:

<div class="ui stackable three column grid">
  <div class="column" markdown="span">![gs-flc-1.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/gs-flc-1.png)</div>
  <div class="column" markdown="span">![gs-flc-2.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/gs-flc-2.png)</div>
  <div class="column" markdown="span">![gs-flc-3.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/gs-flc-3.png)</div>
</div>

For a logged in customer the procees becomes a bit shorter, since all personal data (shipping and billing addresses) will be predefined already based on the customer account info. The preferred delivery and payment methods will also be pre-chosen based on the previous order of this customer. Hence the logged in customer will need only to check the fields and then pay the order.

### One Page Checkout

One Page Checkout (OPC) is a type of checkout when all the infromation required to perform a transaction is displayed on one and the same page being divided into logical blocks of personal data, delivery and payment info.  OPC is considered a more quick and robust option of checkout, but it may lead to errors during the data submission and new customers may be confused by the amount of fields to be filled in at once.

This is how the OPC type of checkout will look for an unregistered customer:

![opc.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/opc.png)

For a logged in customer the personal data (shipping and billing addresses) will be predefined, hence it will be necessary to choose the preferred shipping and payment methods only.

### Catalog Mode (Disabled Checkout)

Sometimes an eCommerce website is needed for demostration purposes only, i.e. a store owner wants to promote products and services online rather than to sell them. 

Such an option in X-Cart can be enabled by installing the {% link "Catalog" ref_3eMIyNpG %} addon.

![catalog.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/catalog.png)

Once the addon has been installed, checkout is disabled, and store visitors are not allowed to buy any products.

## Customer Checkout Options

X-Cart allows both registered and anonymous checkout for customers.

The checkout process for an unregistered customer and for a registered but not logged in customer will start with a page that suggests that they should either sign in with an existing X-Cart account or proceed with an email without an account creation or use their Google and Facebook account for checkout if the {% link "Social Login" ref_IapN8lJ8 %} addon is installed and configured.

![gs-checkout.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/gs-checkout.png) 


### Anonymous Checkout

X-Cart allows anonymous or guest checkout for your customers. This means that if a customer is not registered in your store they don't need to create an account and can proceed to checkout specifying an email only. During checkout unregistered customers will need to specify shipping and billing address, choose the preferred delivery and payment method. X-Cart allows to place an order only when all the fields are filled in properly.

{% note info %}
When the shipping and billing address info is not specified, X-Cart calculates taxes and delivery costs and displays this info to the buyers based on the default customer address predefined in the store.

For more info on the default customer address setup see the {% link "Default Customer Address" ref_3MxAUhHQ %} manual of our Knowledge Base.
{% endnote %}

Unregistered customers can choose to create an account using the data specified during the checkout or they can proceed as guest. The account creation option will look differently depending on [the type of checkout](https://kb.x-cart.com/general_setup/basic_configuration/general_settings/checkout.html#checkout-type "Checkout Setup") enabled in the store:

<div class="ui stackable two column grid">
  <div class="column" markdown="span"><i>Fast Lane Checkout</i>![create-account-flc.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/create-account-flc.png)</div>
  <div class="column" markdown="span"><i>One Page Checkout</i>![create-account-ops.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/create-account-ops.png)</div>
</div>

The fact that a customer doesn't create an account during guest checkout doesn't mean that no account is created for this customer at all. Being it guest checkout or not X-Cart creates a customer account for the e-mail used to place an order and registeres it in the **Users** section on the Admin area. All following orders placed using this email are assigned to the same customer account. If later this customer decides to register an account with the email that was used for placing order(s) previously a store admin has an opportunity to join these 2 customer accounts (one created by X-Cart and one created by the customer) together keeping the info on the previously placed orders safe.

If you wish to disable anonymous checkout, it's necessary to enable the **Ask anonymous users to create an account or sign in before checkout:** option on the **Store setup** -> **Cart&Checkout** -> **General** page of X-Cart Admin area.


### Registered Checkout

Registered customers who are logged into their accounts can complete checkout easier because much of the information is already stored in their accounts. Personal data, like shipping and billing address, are filled in based on the address book data saved for each user account. Shipping and payment method are also predefined. The choice of the selected shipping and/or payment methods will depend on the related data from the previous order of this customer.

Registered customers also have an option to re-order items after a successful checkout, as the data about all orders placed in the store is recorded in the **Orders** section of a customer account in the storefront.
![540-reorder-button.png]({{site.baseurl}}/attachments/ref_0I0Cpjkh/540-reorder-button.png)

Once a customer clicks the **Re-order** button they are redirected to the cart page in the storefront that will contain exactly the same items and in the same amount as in the related order. All they need to do will be to complete the checkout process and pay for the goods.

## Security Settings

Submitting and processing data for transactions require a secure checkout run in the HTTPS mode. Hence for your customers data to be processed safely you must enable HTTPS in the **System tools** -> **HTTPS settings** sections of the Admin area as described in [our security guide.](https://kb.x-cart.com/general_setup/store_security/security_guide.html#step-2-use-ssl-certificates "Checkout Setup")

For more info on how to secure your store please refer to the guides from the {% link "X-Cart Store Security" ref_4ewdbDM8 %} section of our Knowledge Base.
