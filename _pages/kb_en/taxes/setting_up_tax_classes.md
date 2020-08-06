---
lang: en
layout: article_with_sidebar
updated_at: '2017-08-30 18:35 +0400'
identifier: ref_pAWOdG8N
title: Tax Classes
order: 110
categories:
  - User manual
published: true
---
X-Cart offers a tax class feature that allows assigning special tax rates to groups of products and delivery costs if required. Tax classes differentiate by the rate calculation rules.

{% toc %}

## Product Tax Classes

According to your country's laws, you may need to charge different taxes for different types of products. For instance, you may need to calculate sales tax differently for alcohol and no-alcohol products.

Using the **tax class** feature in X-Cart 5 you can organize your products into groups according to what sales tax rate calculation rules need to be used for them.

For example, if you have a food store selling both alcohol and no-alcohol products, and you need to calculate sales tax differently for those two groups of products, you will need two tax classes - one for alcohol products and one for no-alcohol products. To make it work, you will need to specify how tax rates should be calculated for each of these tax classes. You will also need to assign a tax class to every product in your store. This way all the products will have appropriate tax rates applied to them. 

In X-Cart 5, every product needs to have a tax class assigned to it. By default, new products are created with the **Default tax class** assigned. If you expect all of your store's products to use the same tax rates, you do not need to create any additional tax classes - just use the **Default tax class** for all rates. However, if you are going to have different tax rates for different types of products - like in the example with alcohol and no-alcohol products - then you will need additional tax classes.

## Tax Classes for Shipping

The tax classes feature can be used for shipping as well. Typically you create a tax class, set appropriate tax rates for it and assign the tax class to a shipping method via the **Shipping methods** section. 

## Creating Tax Classes

To create a new tax class:

1.  Open the **Tax classes** tab in the **Taxes** section (**Store setup** > **Taxes**) of your X-Cart Admin area: 
    ![541-tax-classes-page.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-tax-classes-page.png)

2.  Click the **New tax class** button. This adds a new blank field below. 
    ![541-tax-classes-new.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-tax-classes-new.png)
    
    You can click more than once to add multiple fields.

3.  Use the field you have added to enter the name for a new tax class (e.g. "Alcohol" on the sample) and **Save changes**: 
    ![541-tax-classes-new-added.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-tax-classes-new-added.png)

That's all, a tax class has been created:
![541-tax-classes-list.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-tax-classes-list.png)

Now you can configure tax rates for it. 

## Configuring Rates for Tax Classes

To configure a tax rate specifying a tax class:

1. Go to the **Taxes** section (**Store setup** -> **Taxes**) of your X-Cart Admin area and, depending on the tax system you are using, open the appropriate tax configuration tab (Depending on the tax addon you are using, this may be **Sales tax** / **VAT/GST** / **Canadian taxes**).

2. Locate the "General Tax Rates" section of the page and click the **New rate** button. 
   ![541-general-tax-rates-full.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-general-tax-rates-full.png)

3. Configure tax rates by specifying the parameters below. Pay special attention to the "Tax class" selector.
   ![541-general-tax-rates.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-general-tax-rates.png)
   
   * **Zone** : Select the address zone to which the tax rate should apply.
   * **Tax class** : Select the tax class to which the tax rate should apply.
   * **Rate** : Specify the tax rate (in %).
   
   {% note info %}
   **Attention of "Sales Tax" addon users**: To set up a tax rate that will be used exclusively for shipping, use the section "Tax rates on shipping cost". Tax rates configured via the "General Tax Rates" section are not applied to products.
   {% endnote %}
   
4. Click **Save changes**.
   ![tax-class-1.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/tax-class-1.png)

That's it. Now you can assign the created tax rate to a product or to a shipping method by assigning the tax class with this rate to them.

## Assigning Tax Classes to Products

Once a tax class has been created, it can be assigned to products. Any products to which this tax class is assigned will use the tax rates defined for this product class.

To assign a tax class to a product:

1.  In the **Catalog** -> **Products** section of your X-Cart Admin area, choose a product to which you need to assign a tax class and open this product's details page for editing.

2.  In the **Prices & Inventory** section of the product details page, locate the field **Tax class** and select the tax class you want to assign to this product.
    ![541-tax-class-product-details.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-tax-class-product-details.png)

3.  Click **Update product** to save the changes.

The tax class is assigned.

{% note info %}
If you need to assign a tax class to more than one product, you may find it convenient to use the ["Bulk Product Edit"](https://kb.x-cart.com/products/bulk_edit.html#bulk-edit-price-and-membership) feature.
{% endnote %}

## Assigning Tax Classes to Shipping Methods

Once a tax class has been created, it can be assigned to shipping methods.

To assign a tax class to a shipping method:

1. In your store's Admin area, go to the Shipping methods section (**Store setup** > **Shipping**).
   ![541-shippings-page.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-shippings-page.png)

2. In the list of shipping methods, locate the column **Tax class**. 
   ![541-shippings-page-tax-classes.png]({{site.baseurl}}/attachments/ref_pAWOdG8N/541-shippings-page-tax-classes.png)
   
   This column shows the tax classes currently assigned to your store's shipping methods. Shipping methods for which no tax class has been assigned manually will have the default tax class assigned.

3. To change a tax class for a shipping method, click on the name of the tax class currently assigned to it. This opens a drop-down box with a list of available tax classes. Select the tax class you require.

4. Save the changes.


_Related pages:_

*   {% link "Specifying Sales Tax for Your Products" ref_aJPK4DHN %}
