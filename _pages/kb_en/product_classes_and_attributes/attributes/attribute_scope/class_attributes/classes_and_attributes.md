---
lang: en
layout: article_with_sidebar
updated_at: '2019-07-24 11:36 +0400'
identifier: ref_2ydGVBck
title: >-
  Product Classes and Class-Attributes Management via the "Classes & Attributes"
  Section
order: 100
published: true
---
When you open the **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) in the store Admin area for the first time after the software installation, you are most likely to see a screen of the kind:

![attributes-listing.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/attributes-listing.png)

Here you see 1 sample {% link "global attribute" ref_HzMkgc0q %} and 3 sample product classes with attributes configured for them. 

The **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) of the Admin area gives a store admin the tools to create a product class, add attribute(s) or attribute groups to it, configure product class attributes, edit product class and product class attribute names and delete both product classes and product class attributes. 

{% note warning %}
Product classes creation and management via the **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) of the store Admin area is described in the {% link "Product Classes" ref_7bb4uhwg %} section of our Knowledge Base. 
{% endnote %}

{% toc %}

## Adding Product Class Attributes to Product Classes

{% note warning %}
Adding product class attributes via the **Classes & Attributes** section of the Admin area (**Catalog > Classes & attributes**) implies that a related product class has been created beforehand as described in the {% link "Creating Product Classes" ref_6ieZHjOV %} guide of our Knowledge Base.
{% endnote %}

To add attribute(s) to an existing product class via the **Classes & Attributes** section follow the steps below:

1.  In your store's Admin area, go to the **Classes & attributes**section (**Catalog > Classes & attributes**).
2.  In the list of product classes, locate the product class you need to add an attribute to and click on the _Edit attributes (N)_ link opposite it:
    ![pc-attr-add-attribute-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1.png)
    This opens a page where you will be able to manage attributes for this product class:
    ![pc-attr-add-attribute-1-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1-1.png)
3.  On this page, click **New attribute**:
    ![pc-attr-add-attribute-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-2.png)
    A popup titled **New attribute** appears:
    ![new-attribute-popup.png]({{site.baseurl}}/attachments/ref_2ydGVBck/new-attribute-popup.png)
4.  Use the fields of the **New attribute** popup to provide information about the new attribute. Specify the following information:

    *   **Attribute**: Attribute name.
    *   **Attribute group**: Select a group name from the drop-down if this is applicable.
        {% note info%}
        Use the [Adding Groups to Product Class Attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#adding-groups-to-product-class-attributes "Product Class Attributes") part of this guide to learn how to join attributes into groups.
        {% endnote%}
    *   **Type**: Attribute value type (_Plain field_, _Textarea_, _Yes/No_).
        {% note info %}
        To choose a proper attribute value type for your attribute refer to the guides from {% link "Attribute Value Field Types" ref_5qw116xV %}.
        {% endnote %}
    * **Display as** : A display mode for multi-value attributes in the storefront. The property is available for a plain type of attrubute only starting with X-Cart 5.4.1.x.
      ![541-new-attribute-popup.png]({{site.baseurl}}/attachments/ref_2ydGVBck/541-new-attribute-popup.png)
      

5.  Click **Next**. The attribute should be saved. 
    
    Now the popup is expanded so you can add/edit the options for this attribute:
    ![pc-attr-add-attribute-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-4.png)
6.  Click **New value** to configure the attribute options depending on the chosen {% link "attribute value field type" ref_5qw116xV %}. Add as many attribute options as you need.
    
    The screen below demonstrates adding a plain field value: 
    ![pc-attr-add-attribute-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-5.png)
7.  If you want some or all of the attribute option(s) you added for this product class to be applied automatically to all the products this product class will be assigned to in future, click the check-mark icon opposite the names of the related attribute options (the check-mark icon should turn green): 
    ![pc-attr-add-attribute-6.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-6.png)
8.  Once you're done with editing the attribute options, save the changes using the **Save changes** button.
   
    The attribute(s) will be added to the list of attributes of the related product class.
    ![pc-attr-add-attribute-7.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-7.png)

You can add as many attributes to one product class as you need. Once all required attributes have been created you can start [assigning this product class to products](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes/global_tab.html#assigning-product-class-attributes-to-products "Product Class Attributes") in your store.

## Adding Groups to Product Class Attributes

In case a product class should have a considerable amount of attributes it makes sense to devide the attributes into groups to make the attributes representation to a customer structured and easy to persive.

![pc-attr-groups-cus.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-cus.png)

To add a group of attributes to a product class:

1. Locate the product class in quiestion in the Classes & attributes section (**Catalog > Classes & attributes**) in your store dmin area and click on __Edit attributes (N)__ link opposite it:
   ![pc-attr-add-attribute-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1.png)
   This opens a page with the list of attributes for the selected product class:
   ![pc-attr-add-attribute-1-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1-1.png)
2. On this page, click **Manage Groups**:
   ![pc-attr-groups-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-1.png)
   A popup titled **Manage attribute groups** appears.
   
3. Use the **New group** button to add as many attribute groups as you need:
   ![pc-attr-groups-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-2.png)
   
4. Click **Save changes** when you are done:
   ![pc-attr-groups-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-4.png)
   
5. The newly created groups will be added to the product class details page:
   ![pc-attr-groups-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-5.png)

Now you can use these goups when [creating attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes/classes_and_attributes.html#adding-product-class-attributes-to-product-classes "Product Class Attributes") for this product class.

## Managing Product Class Attributes 

A store admin can check the list of attributes added to a product class and manage these attributes on a respective product class details page in the **Classes & attributes** section of the Admin area (**Catalog > Classes & attributes**).

{% note info %}
All changes applied to product class attributes via the **Classes & attributes** section of the Admin area are applied store-wide and will affect all products with the related product class assigned by far.
{% endnote %}

To view the list of attributes a product class has a store admin should locate the respective product class in the **Classes & attributes** section of the Admin area and click on _Edit attributes (N)_ link opposite it (where N stands for the numner of attribues a product class has).

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![pc-attr-management-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-1.png)</div>
  <div class="column" markdown="span">![541-pc-attr-management.png]({{site.baseurl}}/attachments/ref_2ydGVBck/541-pc-attr-management.png)</div>
</div>

On a product class details page a store admin will see a list of all attributes assigned to this product class with the respective attribute types by value.

### Editing Product Class Attribute Configuration and Values
   
To edit a product class attribute:

1. In the list of product class attributes, locate the attribute you need to edit. 
2. If you just need to change the attribute name, click inside the **Attribute name** field and edit the attribute name as you require. 
   ![pc-attr-management.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management.png)
3. If you need to change the attribute values (or both the attribute name and values), click the **Edit** button:
   ![pc-attr-management-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-3.png)
      
   This will open a popup titled **Edit attribute values** where you will be able make the necessary changes.
   ![pc-attr-management-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-4.png)
      *  If you want some or all of the attribute value(s) to be applied automatically to all the products that will have this product class assigned in future, be sure to "enable" the check-mark icon opposite the names of the related attribute values (the check-mark icons should turn green):
         ![pc-attr-management-6.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-6.png)
      *  If you want to change the attribute values sorting use the **Cross** icons to re-arrange the values by grag-n-groping them:
         ![pc-attr-management-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-5.png)
      * If you want to apply the new sorting to all products that has this product class assigned by far, enable the **Apply sorting globally** checkbox:
        ![pc-attr-management-7.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-7.png)
        The **Apply sorting globally** setting affects the "active" attribute values only, i.e. the values that are marked with a green check-box and are automatically assigned to all products within this product class.

4. Once you're done editing, click **Save changes**.

### Editing the Display Mode

Starting with X-Cart 5.4.1 X-Cart allows swithcing the display mode of the plain field attributes from selectbox to blocks in the storefront.
<div class="ui stackable two column grid">
  <div class="column" markdown="span"><b>Display as select box</b>![541-selectbox-representation-cus.png]({{site.baseurl}}/attachments/ref_7b4wR1ex/541-selectbox-representation-cus.png)</div>
  <div class="column" markdown="span"><b>Display as blocks</b>![541-block-representation-cus.png]({{site.baseurl}}/attachments/ref_7b4wR1ex/541-block-representation-cus.png)</div>
</div>

If necessary, a store administrator can change the display mode of an attribute directly on a product class attributes listing page in the **Classes & attributes** section of the store Admin area.

For this purpose a store admin should:
1. Locate the attribute to be edited in the list of product class attributes.
   ![541-edit-display-mode-1.png]({{site.baseurl}}/attachments/ref_2ydGVBck/541-edit-display-mode-1.png)
2. Check the value of the **Display as** column for this attribute.
   ![541-edit-display-mode-2.png]({{site.baseurl}}/attachments/ref_2ydGVBck/541-edit-display-mode-2.png)
3. Click on the value and select an alternative in the drop-down. There are only two options - selectbox and blocks.
   ![541-edit-display-mode-3.png]({{site.baseurl}}/attachments/ref_2ydGVBck/541-edit-display-mode-3.png)
4. Click **Save changes** at the bottom of the listing page.

{% note info %}
For details, see [Configuring Multi-Value Attributes Display Mode](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_values/multivalue.html#configuring-multi-value-attributes-display-mode "Product Classes and Class-Attributes Management via the "Classes & Attributes" Section").
{% endnote %}

### Adding Product Class Attirbute(s) to Filters

{% note info%}
The feature works only with the {% link "Product Filter" ref_6e82A7rL %} addon enabled and configured.
{% endnote %}
   
Use the **Funnel with eye** icon opposite the product class attribute name on the product class details page to make this attribute visible in the product filters in the storefront. 

![pc-attr-funnel-yey.png]({{site.baseurl}}/attachments/ref_2ydGVBck/pc-attr-funnel-yey.png)

By default all available product class attributes are visible in filters. To remove an attribute from filters click on the **Funnel with eye** icon opposite the product class attribute name(s). The icon will turn grey.

**Save changes** when you are done.
   
### Re-Arranging Product Class Attribute(s)
   
Change the attributes order of appearance by drag-n-dropping the attributes with the help of a **Cross** icon on the product class details page.

![pc-attr-drag-n-drop.png]({{site.baseurl}}/attachments/ref_2ydGVBck/pc-attr-drag-n-drop.png)

**Save changes** when you are done.
   
### Deleting Product Class Attribute(s)

Use the **Trash** icon opposite a product class attribute name to mark the respective attribute for deletion on the product class details page.

![pc-attr-trash.png]({{site.baseurl}}/attachments/ref_2ydGVBck/pc-attr-trash.png)

Don't forget to **Save changes** when you are done with the attributes management.
