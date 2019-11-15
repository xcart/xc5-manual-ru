---
lang: en
layout: article_with_sidebar
updated_at: '2018-01-29 16:35 +0400'
identifier: ref_6e82A7rL
title: Product Filter
order: 221
published: true
description: 'product filters, easy search'
---
Let us imagine that you run an online store selling tons of different products. Each product has its own set of attributes like size, color, material, technical characteristics, and many others that make it distinct from other products. A shopper's decision to buy depends on these product attributes, and you as a seller can make a shopper's choice easier by using the addon **[Product Filter](https://market.x-cart.com/addons/product-filter.html)**. 

The addon enables you to add a product filter block that will be displayed on category pages (all of them, or just certain category pages chosen by you); your store visitors will be able to adjust the options in this block to narrow down their search results based on product attributes and find the product they require more easily. Optionally, the filter block can be adjusted to also include product tags, a price range, and in-stock availability. 

![]({{site.baseurl}}/attachments/ref_6e82A7rL/store-front.png)

{% toc %}

## Install Product Filter
If the addon **Product Filter** is not installed in your X-Cart store, you can do it from the X-Cart App Store. Follow the general instructions for {% link "installing and activating addons" ref_0fGEpvrh %}.
![product_filter_addon.png]({{site.baseurl}}/attachments/ref_6e82A7rL/product_filter_addon.png)

## Configure the Product Filter Addon Settings
Before using the addon, you will need to cofigure it. Open the _Settings_ page and configure the addon according to your business needs.

The addon settings are as follows:

![settings.png]({{site.baseurl}}/attachments/ref_6e82A7rL/settings.png)

   * **Enable "In stock only" filter**: If this setting is enabled, the filter block includes an 'In stock' selector allowing shoppers to specify whether they want to find only the products that are in stock or the products that are out of stock as well. If it disabled, no such selector is provided. 

   * **Enable "Price range" filter**: If this setting is enabled, the filter block provides a range slider allowing users to specify the desired price range. If it disabled, no such slider is provided. 
     {% note info %}
     For the attention of users of the {% link "Value Added Tax / Goods and Services Tax " ref_0GjdgNJx %} addon:
     
     In X-Cart 5.3.x and earlier the "Price range" filter works with VAT-exclussive prices only, even if your store is set up to display prices {% link "with VAT included" ref_4tqYojGn %}.
     {% endnote %}

   * **Enable "Attributes" filter**: If this setting is enabled, the filter block allows users to choose product attributes. If it disabled, filtering by attributes is not provided.

     {% note info %}
     For the "Attributes" filter to be displayed, you need to have attributes configured in your store, and those need to be global or class-level attributes of the _Plain field_ and/or _Yes/No_ type. (Attributes of the_Textarea_ type are never used for the product filter.) 
     For information on the configuration of attributes, see {% link "Product classes and attributes" ref_T90ZcEpP %}.
     Note that you can control which attributes should be visible in the product filter, and which ones not. For details, see the sections [Set Classes for Product Filter](#set-classes-for-product-filter) and [Control the Visibility of Specific Attributes for Product Filter](#control-the-visibility-of-specific-attributes-for-product-filter) further below.
     {% endnote %}

   * **Enable "Tags" filter**: If this setting is enabled, the filter block allows users to choose product tags. If it disabled, filtering by product tags is not provided.

     {% note info %}
     For the "Tags" filter to be displayed, you need to have product tags configured in your store. For more info, see {% link "Product Tags" ref_6nFoxYf1 %}.
     {% endnote %}

   * **Show only available attributes and tags for products in category**: If this setting is enabled, X-Cart generates a data cache that is used to display in the filter block only the attribute values and tags that are actually used for the products in the category being viewed. Enabling this option will make a page load faster since only a set of attributes and tags will be counted (as opposed to _all_ the attributes and tags available in the store). Enabling this setting may be especially useful for stores with a high inventory turnover ratio.

   * **Cache reset mode**: This setting can be used to specify whether you want cache to be generated on the fly or to be removed when attribute, tag or product data is changed. The first option will allow working with the actual inventory but will slow down the page loading as it will be necessary to cache the filters each time. If you do not update your inventory too often, using the second option is recommended. 

     {% note info%}
     If the option "Remove cache when ..." is selected, a category page cache will be removed and generated anew the first time this page is opened after you change products, categories or attributes data. The first page loading may last more than usual as time will be spent on cache regeneration.
     {% endnote %}

   * **Sort order for class attributes** (available only if the "Attributes" filter is enabled): Here you can specify whether the attributes should be sorted alphabetically or manually.

     {% note info %}
     This setting affects only the attributes themselves, not their values. The values are sorted alphabetically. 
     {% endnote %}

   * **Generate the URL query string for filter with**: Can be set to _GET params_ or _hash_ depending on how you prefer the search URL to be assembled.

After adjusting the settings, be sure to click **Submit** to save the changes.

## Set Classes for Product Filter
To specify the attributes that should be included into the product filter block on a specific category page in the store front end, you will need to do some configuration on the details page of that category: 

   1. In your store's Admin area, go to **Catalog** > **Categories** > **_Category_Name_**.

      ![category.png]({{site.baseurl}}/attachments/ref_6e82A7rL/category.png)

   2. On the **Category Info** tab, find the setting **Classes for product filter**.

      ![Screen Shot 2018-01-31 at 13.25.42.png]({{site.baseurl}}/attachments/ref_6e82A7rL/Screen Shot 2018-01-31 at 13.25.42.png)

      Use this setting to specify what classes of attributes should be used to filter the products in the current category. The available options are as follows:
      
      * _All classes from this category_ - The filter will include the classes of all the products from this category. Note that the more classes and products a category has, the more time it will take to load the category page.
      
      * _Do not show the filter_ - This type of filter will not be displayed on the category page.
      
      * _Choose classes_ - You will be able to specify the exact class(es) on which the filter will be based. By using this option you can limit the number of classes applied. You can choose any classes available in your store.

      ![]({{site.baseurl}}/attachments/ref_6e82A7rL/Screen%20Shot%202018-01-31%20at%2013.26.33.png)

   3. Save the changes.
   
Note that the product filter block wil not be displayed on the page of a category in the store front end if the category itself does not contain products. If the category has subcategories containing products, but does not have any products outside the subcategories, the **Classes for product filter** setting will need to be configured on the pages of the respective subcategories.

## Control the Visibility of Specific Attributes for Product Filter
You can fine-tune the visibility of specific attributes for the product filter via the Classes & attributes section of the Admin area (**Catalog** > **Classes & attributes**).
      
   ![pf_attr_visibility.png]({{site.baseurl}}/attachments/ref_6e82A7rL/pf_attr_visibility.png)

## Change Product Filter Block Location
You can change the location of the product filter block on the page using Layout Editor in Webmaster mode. For more info on that, see {% link "Layout Editor" ref_1xoeCJwy %}.


_Related pages:_

   * {% link "Product Filter: Usage with Multivendor" ref_5YMhId62 %}
