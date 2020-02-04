---
lang: en
layout: article_with_sidebar
updated_at: '2020-02-04 15:12 +0400'
identifier: ref_4kjOv7Ne
title: Connecting Your X-Cart Store to X-Payments Cloud
order: 400
published: true
---
Once the X-Payments Cloud connector addon has been {% link "installed and enabled" ref_2BXoj25Y %}, you can connect your store to X-Payments Cloud with it.

To access the connection page, use one of the following methods:

   * Go to the section **My Addons**, find the installed addon X-Payments Cloud connector and click on the **Settings** link pertaining to it.
     ![xp_cloud_connector_settings_link.png]({{site.baseurl}}/attachments/ref_729XUzDQ/xp_cloud_connector_settings_link.png)

   Or:
   
   * Go to the Payment settings page (**Store setup** > **Payment methods**), locate the payment method "X-Payments Cloud" and choose to configure it:
     ![xp_cloud_method_configure_button.png]({{site.baseurl}}/attachments/ref_729XUzDQ/xp_cloud_method_configure_button.png)
     
The connection page is titled "X-Payments Cloud settings" and looks like the following:
     ![xp_cloud_connector_settings1.png]({{site.baseurl}}/attachments/ref_729XUzDQ/xp_cloud_connector_settings1.png)

Once you are ready to proceed with the connection, you will need to either create a new X-Payments Cloud account or to provide the connection details for your {% link "existing X-Payments Cloud account" ref_729XUzDQ#xpc-registered-account %}.

   * **If you do not have an existing X-Payments Cloud account**, choose to create one:

     1. In the field **Your email**, specify the email address that you are going to use for the X-Payments Cloud account administrator. 
     
     2. In the field **Account name**, specify your desired account name.
     
     3. After completing the above fields, click **Create account**.
   
     This will initiate the creation of an X-Payments Cloud account for you and start your trial period. No commitment and no credit card are required during the trial period.
     
     The creation of your X-Payments account is likely to take a few seconds. During this time you will see a screen like the following:
     ![tuned.png]({{site.baseurl}}/attachments/ref_729XUzDQ/tuned.png)

     In the end you will be prompted to set a password for your X-Payments Cloud account: 
     ![set_passwd_4cloud.png]({{site.baseurl}}/attachments/ref_729XUzDQ/set_passwd_4cloud.png)

     Enter your desired password and type it once again for confirmation. Be sure to click Submit. For your convenience, a link to [Strong password generator](https://strongpasswordgenerator.com/) is provided. 
     
     After setting the password, complete 2-step user authentication setup for your account:
     ![2step_user_auth_setup.png]({{site.baseurl}}/attachments/ref_729XUzDQ/2step_user_auth_setup.png)
     
     More info on setting up 2-step user authentication methods in X-Payments Cloud is available in the X-Payments Cloud manual.
     
     Note that after your X-Payments Cloud account has been created, you will receive a confirmation email message at the email address specified during your registration. Please refer to this email message for your getting started instructions.
     
<a id="xpc-registered-account"></a>
   * **If you already have an existing X-Payments Cloud account**:
     
     1. Use the link "If you already have an X-Payments account, please click here" in the lower part of the X-Payments Cloud connection page to access the page for X-Payments Cloud account sign-in:
        ![access_signin_4registered.png]({{site.baseurl}}/attachments/ref_729XUzDQ/access_signin_4registered.png)
   
     2. On the sign-in page, enter your account name and click **Connect**:
        ![connect_registered.png]({{site.baseurl}}/attachments/ref_729XUzDQ/connect_registered.png)

     3. When prompted to specify your connection credentials, provide your X-Payments Cloud account registration email address and password:
        ![connect_registered1.png]({{site.baseurl}}/attachments/ref_729XUzDQ/connect_registered1.png)
     
     This will connect your X-Cart store to your existings X-Payments Cloud account.

Once your X-Cart 5 store has been connected to X-Payments Cloud, you need to go to X-Payments Cloud and configure it as you require. For more information on this, see {% link "Getting Started with X-Payments Cloud" ref_497aaUTF %}

_Related pages:_
* {% link "X-Payments Cloud Connector" ref_729XUzDQ %}