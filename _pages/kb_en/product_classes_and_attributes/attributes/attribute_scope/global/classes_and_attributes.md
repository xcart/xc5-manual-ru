---
lang: en
layout: article_with_sidebar
updated_at: '2019-07-26 13:55 +0400'
identifier: ref_4ARLM9v7
title: Global Attributes Management via the "Classes and Attributes" Section
order: 100
published: true
---
Usually global attributes are created and managed via the the **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) of the store Admin area.

To view the list of global attributes configured in the store it's necessary to open the **Classes & Attributes** section and click on the link _Edit attributes (N)_ opposite the Global attributes line (here **N** stands for a number of global attributes configured in the store).

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![ga-listing.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing.png)</div>
  <div class="column" markdown="span">![ga-listing-1.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing-1.png)</div>
</div>

The global attributes listing page allows to add new and manage existing global attributes as well as to group global attributes if required.

{% toc %}

## Adding Global Attributes

To add a new global attribute:

1.  In your store's Admin area, go to the **Classes & attributes** section (**Catalog > Classes & attributes**).
2.  Click on the _Edit attributes (N)_ link opposite the **Global attributes** title:
    ![ga-listing.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing.png)
    This opens a page where you will be able to manage global attributes:
    ![ga-listing-1.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing-1.png)
3.  On this page, click **New attribute**:
    ![ga-add-attribute-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-1.png)
    A popup titled **New attribute** appears:
    ![ga-add-attribute-2.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-2.png)
4.  Use the fields of the **New attribute** popup to provide information about the new attribute. Specify the following information:

    *   **Attribute**: Attribute name.
    *   **Attribute group**: Select a group name from the drop-down if this is applicable.
        {% note info %}
        Use the Adding Groups to Global Attributes part of this guide to learn how to join attributes into groups.
        {% endnote %}
    *   **Type**: Attribute value type (_Plain field_, _Textarea_, _Yes/No_, _Hidden field_).
        {% note info %}
        To choose a proper attribute value type for your attribute refer to the guides from {% link "Attribute Value Field Types" ref_5qw116xV %}.
        {% endnote %}
5.  Click **Next**. The attribute should be saved. Now the popup is expanded so you can edit attribute options:
    ![ga-add-attribute-3.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-3.png)
6.  Configure the attribute options depending on {% link "the chosen attribute value field type" ref_5qw116xV %}. Add as many attribute options as you need.
    ![ga-add-attribute-4.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-4.png)
    
7.  If you want some or all of the option(s) you added for this hidden global attribute to be assigned automatically to all NEW products in your store's catalog, click the check-mark icon opposite the names of the related attribute options (the check-mark icons should turn green):
    ![ga-add-attribute-4-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-4-1.png)
    {% note info %}
    Enabling check-mark for a hidden attribute option will not affect the products that are present in the store by far. All exisiting products will preserve their current global attributes' configuration.
    {% endnote %}
8.  Once you're done editing the attribute options, save the changes using the **Save changes** button.
    
    The attribute options(s) should be saved and added to the global attributes list:
    ![ga-add-attribute-5.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-add-attribute-5.png)
    
All global attributes are assigned automatically to all existing products in the store. However, for them to be displayed properly in the storefront a store admin must configure global attribute options for existing products.


## Adding Groups to Global Attributes

If required it's possible to devide the global attributes into groups to make the attributes representation to a customer structured and easy to persive.

To add a group to global attributes:

1.  In your store's Admin area, go to the **Classes & attributes** section (**Catalog > Classes & attributes**).
2.  Click on the _Edit attributes (N)_ link opposite the **Global attributes** title:
    ![ga-listing.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing.png)
    This opens a page where you will be able to manage global attributes:
    ![ga-listing-1.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing-1.png)
3. On this page, click **Manage Groups**:
   ![ga-groups-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-groups-1.png)
   A popup titled **Manage attribute groups** appears.
   
3. Use the **New group** button to add as many attribute groups as you need:
   ![pc-attr-groups-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-2.png)
   
4. Click **Save changes** when you are done:
   ![pc-attr-groups-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-4.png)
   
5. The newly created groups will be added to the product class details page:
   ![ga-group-2.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-group-2.png)

Now you can use these goups when [creating global attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes/classes_and_attributes.html#adding-product-class-attributes-to-product-classes "Product Class Attributes").

## Managing Global Attributes 

A store admin can check the list of global attributes and manage them on a global attributes listing page in the **Classes & attributes** section of the Admin area (**Catalog > Classes & attributes**).

{% note info %}
All changes applied to global attributes via the **Classes & attributes** section of the Admin area are applied store-wide and will affect all products with the related global attribute enabled.
{% endnote %}

To view the list of global attributes configured in the store it's necessary to open the **Classes & Attributes** section and click on the link _Edit attributes (N)_ opposite the Global attributes line (here **N** stands for a number of global attributes configured in the store).

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![ga-listing.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing.png)</div>
  <div class="column" markdown="span">![ga-listing-1.png]({{site.baseurl}}/attachments/ref_HzMkgc0q/ga-listing-1.png)</div>
</div>

On the global attributes listing page gives a store admin the tools to edit global attribute name and configuration, add global attributes to filters in the storefront, re-arrange and delete global attributes. 

### Editing Global Attributes

Sometimes you may need to change the name and/or values of a global attribute. 

1.  On the global attributes listing page, locate the attribute you need to edit and hover your cursor over its name. 
2.  If you just need to change the attribute name, click inside the **Attribute name** field and edit the attribute name as you require. 
    ![ga-edit-2.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-2.png)
3. If you need to change the attribute values (or both the attribute name and values), click the **Edit** button:
   ![ga-edit-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-1.png)
   This will open a popup titled **Edit attribute values** where you will be able make the necessary changes:
   ![ga-edit-3.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-3.png)
   * If you want some or all of the attribute options(s) to be applied automatically to all the products in your store, be sure to "enable" the check-mark icon opposite the names of the related attribute options (the check-mark icons should turn green):
     ![ga-edit-4.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-4.png)
   * If you want to change the attribute options sorting use the **Cross** icons to re-arrange the values by grag-n-groping them:
      ![ga-edit-5.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-5.png)
   * If you want to apply the new sorting to all products that has this global attribute assigned, enable the **Apply sorting globally** checkbox:
     ![ga-edit-6.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-edit-6.png)
     The **Apply sorting globally** setting affects the "active" attribute options only, i.e. the options that are marked with a green check-box and are automatically assigned to all products.
4.  Once you're done editing, click **Save changes**.

### Editing the Display Mode

Starting with X-Cart 5.4.1 X-Cart allows swithcing the display mode of the plain field attributes from selectbox to blocks in the storefront.
<div class="ui stackable two column grid">
  <div class="column" markdown="span"><b>Display as select box</b>![541-selectbox-representation-cus.png]({{site.baseurl}}/attachments/ref_7b4wR1ex/541-selectbox-representation-cus.png)</div>
  <div class="column" markdown="span"><b>Display as blocks</b>![541-block-representation-cus.png]({{site.baseurl}}/attachments/ref_7b4wR1ex/541-block-representation-cus.png)</div>
</div>

If necessary, a store administrator can change the display mode of an attribute directly on a global attributes listing page in the **Classes & attributes** section of the store Admin area.

For this purpose a store admin should:
1. Locate the attribute to be edited in the list of product class attributes.
   ![541-ga-display-mode.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/541-ga-display-mode.png)
2. Check the value of the **Display as** column for this attribute.
3. Click on the value and select an alternative in the drop-down. There are only two options - selectbox and blocks.
   ![541-ga-display-mode-dropdown.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/541-ga-display-mode-dropdown.png)
4. Click **Save changes** at the bottom of the listing page.

{% note info %}
For details, see [Configuring Multi-Value Attributes Display Mode](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_values/multivalue.html#configuring-multi-value-attributes-display-mode "Product Classes and Class-Attributes Management via the "Classes & Attributes" Section").
{% endnote %}

### Adding Global Attirbute(s) to Filters

{% note info%}
The feature works only with the {% link "Product Filter" ref_6e82A7rL %} addon enabled and configured.
{% endnote %}
   
Use the **Funnel with eye** icon opposite the global attribute name on the global attributes listing page to make this attribute visible in the product filters in the storefront. 

![ga-filters-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-filters-1.png)

By default all available global attributes are visible in filters. To remove an attribute from filters click on the **Funnel with eye** icon opposite the global attribute name(s). The icon will turn grey.

**Save changes** when you are done.
   
### Re-Arranging Global Attribute(s)
   
Change the attributes order of appearance by drag-n-dropping the attributes with the help of a **Cross** icon on the global attributes listing page.

![ga-rearrange-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-rearrange-1.png)

**Save changes** when you are done.

### Deleting Global Attributes

Use the **Trash** icon opposite a global attribute name to mark the respective attribute for deletion on the global attributes listing page.

![ga-delete-1.png]({{site.baseurl}}/attachments/ref_4ARLM9v7/ga-delete-1.png)

Don't forget to **Save changes** when you are done with the attributes management.

The attribute will be deleted from the list of your store's global attributes and will be removed from the details of all products.
