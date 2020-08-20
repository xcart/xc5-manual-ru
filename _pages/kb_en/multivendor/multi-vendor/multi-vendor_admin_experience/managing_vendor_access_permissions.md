---
lang: en
layout: article_with_sidebar
updated_at: '2018-03-15 11:30 +0400'
identifier: ref_0GOeWpB2
title: Managing Vendor Access Permissions
order: 200
published: true
---
A store administrator manages the access permissons for the store users using {% link "Roles" ref_38HKdc1f %} (**Users** > **Roles**). 

The Multi-vendor addon introduces a new user role: "Vendor", that enables access to the dedicated vendor area of the X-Cart store's back end and permissions to operate as a vendor. By default, access permissions for a "Vendor" role are as follows:

*   Manage vendor's catalog;
*   Manage vendor's orders;
*   Manage vendor's shipping settings.
    
If necessary, the store administrator can edit this role changing the role name or the set of access permissions which this role gives to its users. 
    ![541-roles-vendor-page.png]({{site.baseurl}}/attachments/ref_0GOeWpB2/541-roles-vendor-page.png)
    
Alternatively, the store administrator can create other vendor-related roles with some or all of the above-named vendor permissions.

If the administrator chooses to use more than one vendor-related role in their store, they need to set the default vendor role ("Role to assign to new vendor users") via the Multi-vendor addon settings. See the setting **Role to assign to new vendor users** in the **Onboarding** section of the addon settings page.

To change the access permissions of a vendor, the administrator can either change the role assigned to them or give them additional roles according to the functions they need to perform. This can be done via the Access information section of the vendor's user profile (See the **Account details** tab).

More info on the roles management see in {% link "User Roles" ref_38HKdc1f %}.

_Related pages:_
   
   *  {% link "Multi-vendor: Admin Experience" ref_6kbIUy5R %}
   *  {% link "Multi-vendor Getting Started for Admin" ref_5saLJNod %}
