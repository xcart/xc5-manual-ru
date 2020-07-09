---
lang: en
layout: article_with_sidebar
updated_at: '2019-07-08 13:17 +0400'
identifier: ref_5eR4FK3h
title: Storefront Setup
order: 110
published: true
---
The way your customers will see products and add them to cart in the storefront will depend on the settings specified in the Customer Zone settings section of the **Store setup > Cart & checkout**  (the tab **General**) page in the Admin area:
![541-customer-zone-settings.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-customer-zone-settings.png)

The settings that you can configure here are as follows:

*   **How to show out of stock products** : This setting allows you to specify whether out-of-stock products should be visible to customers on the storefront. 
    
    The following options are available:
    
    * _Show in all the sections_  
    * _Show only in categories and search listings_ 
    * _Show only in search listings_
    * _Hide and make them available only via a direct link_ (default value)
    
*   **Display check number for eCheck payment method**: This setting is used for stores with the Check payment method set up. It defines whether the payment information form provided to the customer who has chosen to pay by check should include a field for check number, or not.
    ![xc5_check_number_field.png]({{site.baseurl}}/attachments/ref_qAZlJxZm/xc5_check_number_field.png)

*   **Subcategory listings format**: This setting defines how subcategories should be displayed on category pages. 
    Setting the subcategory listings format to "_Icons_" allows you to have icons displayed for your subcategories:
    ![541-subcategories-icons.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-subcategories-icons.png)

    Setting the format to "_List_" produces a simple list of subcategory names, without icons:
    ![541-subcategories-list.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-subcategories-list.png)
    
    {% note info %}
    This setting does not apply to root (top level) categories. The appearance of root categories on the store's Home page can be adjusted with the setting _'Root category listings format'_ on the **Content > Front page** page of your store Admin area.
    {% endnote %}

*   **Default order to sort products within a category**: This setting allows you to control the default display order for products within a category. 
    The following options are available:

    *   _Recommended_ - Product sort order defined by the store owner via the category settings on the category details page in the store Admin area (**Catalog** -> **Categories** -> **<CATEGORY_NAME>** -> **Products**):
        ![541-category-page-reorder.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-category-page-reorder.png)
 
    *   _Newest first_ - Products sorted by arrival date.
    
    *   _By Price - cheapest first_ - The low to high price sort order (Products with the lowest price are displayed first).
     
    *   _By Price - cheapest last_ - The high to low price sort order (Products with the highest price are displayed first).

    *   _By Name - A-Z_ - Products sorted by their names, A to Z direction.
    
    *   _By Name - Z-A_ - Products sorted by their names, Z to A direction.
    
    *   _Sales_ - (Enabled by the addon **Bestsellers**) Products sorted by popularity (Products sold the most often are displayed first).
    
    *   _Rate_ - (Enabled by the addon **Product reviews**) Products sorted by their rating (Products rated highest by the buyers are displayed first).

*   **Default order to sort products within a search result**: This setting specifies the default sort order for products that may be displayed in a list of search results after someone searches for a product in the Customer area. If your store uses the default X-Cart's product search feature, the list of available options here is the same as for the setting 'Default order to sort products within a category' above. If your store's search is powered by {% link "CloudSearch" ref_5IHjr19k %}, you do not need to adjust this option, because CloudSearch automatically sets the default sort order for search results to relevance.

*   **Default display mode for products list**: This setting allows you to set the default display mode for category products listing on a related category page in the storefront (does NOT affect bestsellers, featured products, etc.):
    
    *   _Grid_:
        ![541-product-listing-grid.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-product-listing-grid.png)
    
    *   _List_:
        ![541-product-listing-list.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-product-listing-list.png)

    *   _Table_:
        ![541-product-listing-table.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-product-listing-table.png)


*   **Products per category listing page**: This setting allows you to specify the number of products that should be displayed on a category page by default (Users will be able to change the number of products displayed per page if they wish; here you set the number of products they see initially, before making any changes). 

    For example, if we set this to "3", by default there will be only three products displayed per page. For the rest of the product list pagination will be provided:
    ![541-products-per-category-listing-page.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-products-per-category-listing-page.png)
    
*  **Maximum products per category listing page**: This setting allows you to set a limit on the maximum number of products that can be displayed on a category page. 
   
   For example, if we set this to "5", a user will not be able to change the number of products displayed per page to a number larger than 4 (See the screenshot below: The number of products currently displayed on a category page is 2. A user can switch this to 4, which is less than 5, but they cannot switch it to 5 or more). 
    ![xc5_general_settings_max_prod_number.png]({{site.baseurl}}/attachments/ref_qAZlJxZm/xc5_general_settings_max_prod_number.png)

*   **Minimum allowed order subtotal**: This setting allows you to set the minimum order amount a shopper must reach before being allowed to check out.
    ![541-min-allowed-order-value.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-min-allowed-order-value.png)

*   **Maximum allowed order subtotal**: This setting allows you to set the maximum order amount. A shopper will be allowed to check out only if their order subtotal amount is less than this value.
    ![541-max-allowed-order-value.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-max-allowed-order-value.png)
    
*   **Maximum order quantity (per product)**: This setting allows you to limit the number of product units that a buyer can order at a time. If a buyer attempts to add to cart more product units than specified here, only the allowed quantity will be added. The buyer will NOT be notified of the quantity adjustment.

*   **Force customer to choose product options before adding a product to cart**: This setting affects the add to cart behavior for products with product options or variants. 
    
    *  _NO_ : With this option selected, a shopper will be able to add a product with options/variants to the shopping cart without selecting any options; the product will be added to the shopping cart with its default option set, which the shopper will be able to adjust later.
    
    * _On Category Listing_ : A shopper who chooses to add to cart a product with options/variants from a category listing will have to specify the options they require before the product is added to the shopping cart.
    
    * _On Category and Product Details Page_ : With this option selected, the add to cart behavior on a category listing will be the same as desribed above (See the _On Category Listing_ option). In addition to that, if a shopper chooses to add a product to the shopping cart from the product details page, they will also have to select product options.    

*   **Redirect customer to the cart page after a product is added to cart**: When this option is enabled, after adding a product to cart a shopper is redirected to the cart page where they can see the item they just added. When the option is disabled, the shopper remains on the same page. 
    {% note info %}
    This setting is not compatible with X-Cart's addon {% link "Add to Cart PopUp" ref_1iGC8Efj %}. When the addon "Add to Cart PopUp" is enabled, adding a product to cart results in a popup being displayed.
    {% endnote %}

*   **Display "Add to cart" buttons for products in grid view**: This setting defines whether "Add to cart" buttons should be displayed for products in grid view, or not. The screenshot below demonstrates products in grid view with the "Add to cart" buttons enabled: 
    ![541-add-to-cart-grid-view.png]({{site.baseurl}}/attachments/ref_5eR4FK3h/541-add-to-cart-grid-view.png)
    
    {% note info %}
    The setting affects only the grid view and has no impact on the list and table modes. For the latter, the "Add to cart" button displays for all products regardless of the value of this setting.
    {% endnote %}

*   **Ask anonymous users to create an account or sign in before checkout**: If this option is enabled, a shopper who is not signed in at the time of clicking the "Checkout" button will be provided with a page where they can sign in to their account or create a new one:
    ![xc5_general_settings_login_b4_checkout.png]({{site.baseurl}}/attachments/ref_qAZlJxZm/xc5_general_settings_login_b4_checkout.png)

    When this option is disabled, such a page is not provided, and the shopper goes straight to the store's checkout page. 
    
    A user who attempts to check out with an email address already existing in the database is recognized by the system based on their email address and prompted to sign in if they wish to:
    ![xc5_general_settings_email_in_use.png]({{site.baseurl}}/attachments/ref_qAZlJxZm/xc5_general_settings_email_in_use.png)

*   **Terms and conditions relative URL**: Relative URL of the static page with your store's Terms and conditions (enabled by the Simple CMS module). If the field is empty (for example, Simple CMS is not installed), a language variable from ?target=terms (Terms and conditions text) will be used (the Terms and conditions text will be displayed in a popup at checkout); this is part of core fuctionality, the module Simple CMS is not necessary.

*   **Next order #**: This field allows you to increase the order number starting from which orders in your store will be numbered. For example, if your store has just went into production and does not yet have many orders, your first customers may be scared off by the order numbers they get. For new customers, a business with order numbers like #1 or #2 may not seem trustworthy enough. To generate more trust, you can set this field, for example, to 103 (In practice, this value can be set to any number - the only requirement is that this number must be greater than the number of the latest order in your database). Your next order will then be #103, and after that you will get the order numbers #104, #105, etc.

*   **Cart TTL (days)**: When a new visitor comes to an X-Cart based store for the first time, a "cart" is created for them in the store's database. Since a lot of visitors will leave the store without creating an account, it's no use storing their carts forever (For visitors who become registered customers, the "cart" is stored for the lifetime of the respective user account). The setting "Cart TTL (days)" allows you to limit the time period for which anonymous shopping carts (carts of visitors who do not have an account) should be stored in the database. Anonymous carts older than the number of days specified here will be considered old (expired) and will be scheduled for deletion by the internal cron service (See the setting below).

*   **Enable internal cron service**: This setting allows you to enable/disable the use of your store's internal cron service. This service schedules the run of certain maintenance tasks required to keep your store running smoothly and problem-free (like removing the expired shopping carts of visitors who do not have an account with your store or performing other tasks implemented via X-Cart modules) at the periodicity of once per 100 user sessions (i.e. every time after your store gets 100 unique visitors). Your store's internal cron service is not related to {% link "console.php" ref_lLqNzAaq %} and does not require any external setup of the crontab on your system. If using the internal cron service causes performance problems for your store, we recommend disabling this option and using an external cron setup to run console.php. 

*   **Allow customers to sign up for membership**: This setting can be enabled to add a membership signup box on the customer profile details page. If a customer wishes to join some membership group, they will be able to use that box to specify the membership group they wish to join. After the customer's profile details with the specified membership are saved, a membership signup request will be submitted to the store administrator in the form of an email notification. The administrator can then choose whether to approve or decline it.

Starting from X-Cart 5.4.0.x the following setting is also available in this section:

*  **Number of days to store the last login data**: This setting defines the lifespan of the “recent_login” cookie that is set by the store on a customer’s computer when they log in. While being stored, the cookie allows the customer to return to the store without having to re-enter their user authentication details (username and password).
