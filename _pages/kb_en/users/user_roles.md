---
lang: en
layout: article_with_sidebar
updated_at: '2017-05-15 13:16 +0400'
identifier: ref_38HKdc1f
title: User Roles
order: 100
published: true
---
A role in X-Cart is a set of permissions providing access to certain features and areas of the store Admin area. X-Cart roles enable a store root admin to configure different levels of access to the store's back end for different administrator users. This feature may be useful if you have staff who you want to delegate some work on the store maintenance but don't want to give this staff full access to the store Admin area. 

Roles are added to the core X-Cart via the addon **User permissions**. This module comes for free with X-Cart Business, Multivendor and Ultimate editions.
    ![module-enabled.png]({{site.baseurl}}/attachments/ref_38HKdc1f/module-enabled.png)
    
{% toc %}


## Roles Listing Page

Typically, if you are using X-Cart Business, Multivendor or Ultimate, the addon **User permissions** is already enabled, and your X-Cart store already has some roles configured - you can view them in the **Roles** section of the Admin area (**Users** > **Roles**).
    ![roles-section.png]({{site.baseurl}}/attachments/ref_38HKdc1f/roles-section.png)

_Administrator_ is the role with the **root access** permissions to the store Admin area, which means that an administrator with this role has full access to all the features (no restrictions at all). This is the only role in X-Cart that can't be edited or deleted.

The rest of the configured roles provide limited access to a store Admin area so that a person could work with just some of the features (sections). 

## Roles Configuration

Roles are totally configurable. Each role consists of a set of access permissions. You can create new roles or edit existing ones and assign as many access permissions to one role as you find necessary. You can also delete the roles you do not need.

### Access Permissions

A full list of access permissions available in a default X-Cart store is as follows:

   * **Root access** : Gives a full access to the store Admin area (with no limitations at all).
   * **Manage catalog** : Gives access to several pages of the **Catalog** section of the strore Admin area, where this user can manage all products including product categories, tags, classes and attributes. Also this user get access to the **Content** -> **Featured products** section of the Admin area to manage featured products. 
   * **Manage reviews** : Gives access to the **Catalog** -> **Reviews** page of the store Admin area where this user can manage existing and create new product reviews.
   * **Manage users** : Gives access to the **Users** -> **User list** page of the Admin area, where this user can manage existing and create new customer accounts. 
   * **Manage administrators** : Extends the **Manage users** access permission with a possibility to manage existing and create new admin and vendor accounts (including root admins). The **Manage administrators** access permission doesn't allow to assign new or change existing roles assigned to different admin accounts.
   * **Manage orders** : Gives access to several pages of the **Orders** section of the store Admin area, where this user can process orders in full, including working with order statuses, payment transactions, order stats and messages. 
   * **Manage import** : Gives access to several pages of the **Catalog** section of the store Admin area, where this user can import data and update products quantity. 
   * **Manage export** : Gives access to the **Catalog** -> **Export** page of the store Admin area, where this user can export all product related info, including categories, classes and attributes and their values and product tabs, as well as product reviews, customers and orders data.
   * **Manage banners** : Gives access to the **Сontent** -> **Front page** -> **Banner rotation** page of the store Admin area, where this user can manage the (sub)categories' banners and the way they are displayed in the storefront.
   * **Allow unfiltered HTML** : Gives a user a possibility to add [unfiltered HTML code](https://devs.x-cart.com/design_changes/adding_custom_javascript_code_to_the_page.html#script-tag-in-content-fields-or-static-pages "User Roles") to any text area (e.g. product description, category description, news, static page content, etc.) in the store Admin area. This access permission can be used only in bundle with other access permissions that give access to different text areas of the store Admin area (e.g. **Manage catalog**, **Manage reviews**, etc.). 
   * **Manage custom pages** :  Gives access to the **Сontent** -> **Pages** page of the Admin area, where this user can create new and manage existing store HTML pages.
   * **Manage menus** :  Gives access to the **Сontent** -> **Menus** page of the Admin area, where this user can create new and manage existing store header and footer menus.
   * **Manage news** : Gives access to the **Сontent** -> **News messages** page of the Admin area, where this user can create new and manage existing news messages.
   * **Manage coupons** : Gives access to the **Discounts** -> **Coupons** page of the Admin area, where this user can create new and manage existing discount coupons.
   * **Manage volume discounts** : Gives access to the **Discounts** -> **Volume discounts** page of the Admin area, where this user can create new and manage existing volume discounts.
   * **Manage conversations** : Gives access to the **Orders** -> **Messages** page of the store Admin area, where this user can work with customers' messages on their orders. 

### Adding New Roles

To add a new role:
1.  Click the **New role** button.
    ![new-role.png]({{site.baseurl}}/attachments/ref_38HKdc1f/new-role.png)

2.  In the form that opens, specify the details of the role you want to create:
    ![role-details.png]({{site.baseurl}}/attachments/ref_38HKdc1f/role-details.png)

     *   **Name** : The name to identify the role.
     *   **Enabled** : Whether the role is active. When a role is inactive (disabled), users with this role can log in to the store's back end, but they cannot access any of the features/areas which their role entitles them to access.
     *   **Permissions** : The set of access permissions the user with this role should have. Simply click in the field and it will show a drop-down list with permissions you will be able to select from.

3.  Click **Create**.

### Managing Roles

To manage roles open the **Roles** page of the store Admin area (**Users** -> **Roles**) and use the tools on the page to apply the necessary changes.

![editing-roles.png]({{site.baseurl}}/attachments/ref_38HKdc1f/editing-roles.png)

1. Role Changes

   To edit a role, click on its name in the Roles table, then edit the role details and click **Update** to save the changes. The changes applied to the role will affect all the admins with this role assigned.

2. Role Deactivation
   
   It is possible to deactivate a role directly on the role listing page to disable the permissions granted by this role to the admins who hold it. To do so, click on the green **On/Off** icon in front of the role name and save the changes.

3. Role Deletion
   
   To delete a role, click on the **Trash** icon opposite the role name at the far right and save the changes.
   
## Assigning Roles to Admin Accounts
    
To assign a role to an admin account:

1. Locate the required admin account on the **Users list** page and click on the email to open the **Account details** page. 
2. On the **Account details** page locate the **Access information** section:
    ![roles-account-setup.png]({{site.baseurl}}/attachments/ref_38HKdc1f/roles-account-setup.png)
3. Click on the **Roles** field and choose the necessary role from the drop-down. You can add more than one role to each user.
4. Click **Update** to save the changes.


