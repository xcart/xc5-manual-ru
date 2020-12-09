---
lang: en
layout: article_with_sidebar
updated_at: '2018-04-18 11:33 +0400'
identifier: ref_25POvGjV
title: Configuring and Using CloudFilters
order: 600
published: true
---
## General Information on CloudFilters
The CloudFilters feature is aimed at narrowing down search results and helping your customers to navigate through a large list of products to find items matching certain filtering criteria. Filters will be dynamically adjusted to your customers' needs, automatically updating the count values to reflect the correct number of terms for the current search.

Filters are displayed on a category/subcategory page, search page and brands page (if the addon {% link "Shop by Brand" ref_2LetICls %} is enabled). 

Filters are shown dinamically based on the content of the page on which they are displayed. Accordingly, the filters for one category will not be the same as the filters for another category, and both of them will differ from the filters displayed on the search page, etc. 

<div class="ui stackable three column grid">
  <div class="column" markdown="span">![filters-1.png]({{site.baseurl}}/attachments/ref_25POvGjV/filters-1.png)</div>
  <div class="column" markdown="span">![filter-2.png]({{site.baseurl}}/attachments/ref_25POvGjV/filter-2.png)</div>
  <div class="column" markdown="span">![filters-3.png]({{site.baseurl}}/attachments/ref_25POvGjV/filters-3.png)</div>
</div>

The set of filters to be displayed on a page is automatically narrowed down and is built based on the  {% link "global product attributes" ref_HzMkgc0q %}, {% link "product tags" ref_6nFoxYf1 %} and {% link "vendor" ref_4ahg5FLK %} info. The selected filters are saved in the URL so that one can easily share a link to the filtered list of products. It is not only handy for the users but may also be advantageous for SEO. 

Once a filter has been applied, all the images and prices are updated at once.

## CloudFilters Activation and Setup
To start using CloudFilters, open the **Cloudfilters** tab on the **Catalog** -> **CloudSearch & CloudFilters** page in the Admin area. 
   ![cloud_cloudfilters_tab_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_cloudfilters_tab_en.png)

Enable CloudFilters using the button **Enable CloudFilters**:
   ![cloud_enable_cloudfilters_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_enable_cloudfilters_en.png)

Once CloudFilters service has been activated for your store, you will see a screen with two tab sections, **Set Up Filters** and **Smart Filter Selection For Product Search**.
   ![cloud_cloudfilters_sections_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_cloudfilters_sections_en.png)

The section **Set Up Filters** is where you will do the general setup of your filters to be applied store wide. This section provides a list of filters generated automatically based on all the product attributes, tags and vendors defined in your store. You can enable/disable any filters and change the filter settings:

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![cloud_manage_filters_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_manage_filters_en.png)</div>
  <div class="column" markdown="span">![cloud_size_filter_settings_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_size_filter_settings_en.png)</div>
</div>

If a filter is disabled in the section **Set Up Filters**, it is not displayed on the storefront. 

Besides the filters listed in the section **Set Up Filters**, there are some default filters (category, price and manufacturer) that are always present along with the filters you have enabled. 

The section **Smart Filter Selection For Product Search** is an advanced filtering system that can be used by big stores with a wide range of products (and, as a result, a lot of product attributes) to narrow down the set of filters displayed on the search page on the storefront. Here you can configure special filter categories based on customer search queries. As a result, only relevant filters will be shown.

The section **Smart Filter Selection For Product Search** is where you do the advanced configuration of you store's filtering system. This section will be of use to large stores with a wide range of products (and, accordingly, a large number of product attributes). This section enables you to limit the number of filters that should be displayed on the search page on the storefront in accordance with the search query that has been used. In other words, the essense of the "Smart Filter Selection" feature is that it enables you to configure different sets of filters for different user search queries, linking them to specific keywords. As a result, when this feature is used, the search page does not show all the filters available in the store (as configrued via the **Set Up Filters** section), but only the ones pertaining to the search query that has been used by your customer.

Filter sets that are linked to specific keywords are called filter categories.

To add a filter category:

1. Click **Add Filter Category**.
   ![cloud_add_filter_cat_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_add_filter_cat_en.png)

   A popup titled "Add new filter category" will be displayed.
   ![cloud_add_filter_cat1_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_add_filter_cat1_en.png)

2. Use the popup to configure a filter category: In the field **Keywords**, specify the keyword(s) to which the filter set of this filter category should be linked; then, click within the field **Filters** and select the filters for this category. 

3. Once you are done selecting the filters, click **Add category**.
   ![cloud_add_filter_cat2.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_add_filter_cat2.png)

As a result, the filter category will be created.
   ![cloud_filter_cat_added_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_filter_cat_added_en.png)

Note that the filter categories you use and the keywords you specify in the section **Smart Filter Selection For Product Search** must match the structure of user search queries. For example, if you are selling footballs and sportswear in your store, and you want different filters to appear depending on the type of products that has been found as a result of a search query, you will need to create two filter categories. At the same time, it is important that the specified keywords do not overlap in meaning, because, when your customer does a search on your store site, only one filter category needs to be selected in accordance with the search query.

## Account Management and/or Deactivating CloudFilters 
<a id="cloudfilters-dashboard"></a>You can check the status of your CloudFilters account and, if necessary, disable the use of CloudFilters in your store using the CloudFilters settings panel. 
To access this panel, use the "Settings" button on the **CloudFilters** tab:
   ![cloud_cloudfilters_settings_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_cloudfilters_settings_en.png)

On this panel you can see:
   
   * The status of your CloudFilters subscription and a button that allows you to change your current subscription plan.
   * The status of data synchronization between your store and the CloudFilters service on our servers.
   * A switch that allows you to disable the use of CloudFilters in your store.
   ![cloud_cloudfilters_settings1_en.png]({{site.baseurl}}/attachments/ref_25POvGjV/cloud_cloudfilters_settings1_en.png)
