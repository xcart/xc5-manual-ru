---
lang: en
layout: article_with_sidebar
updated_at: '2019-06-27 13:10 +0400'
identifier: ref_00nAL9h3
title: Admin Area Login and Password Recovery
order: 100
published: true
---
Once the X-Cart software installation process has been [completed](https://kb.x-cart.com/general_setup/installation/installation_guide.html#step-7-installation-completed "Admin Area Login and Password Recovery"), you can get to managing products, orders, customers, and most other features of your store. But first you need to log in to your X-Cart store Admin area. If you forget the admin password, you can recover it at any time using the email address that is associated with the account.

{% toc %}

## Admin Area Login

1. In the address bar of your browser, enter the URL that was specified during the X-Cart software installation, followed by the base URL of your store’s Admin area. 
   
   The default Admin URL looks like this: `http://<your-domain>/<x-cart-5-directory>/admin.php?target=login`
   
   You should see a page like this:
   ![login-page.png]({{site.baseurl}}/attachments/ref_00nAL9h3/login-page.png)
   
   {% note info %}
   You can bookmark the Admin Login page for easy access.
   {% endnote %}
   
2. Enter your email and password for the Admin area.

   {% note info %}
   The initial Admin area login credentials were set up during [Step 2 of the X-Cart software installation](https://kb.x-cart.com/general_setup/installation/installation_guide.html#step-2-creating-administrator-account "Admin Area Login and Password Recovery").
   {% endnote %}
   
3. Click the **Log in** button.

## Admin Area Password Recovery

1. If you ever forget your password, click the **Forgot password?** link at `http://<your-domain>/<x-cart-5-directory>/admin.php?target=login`.
   
   You will be redirected to the **Forgot your password?** page:
   ![password-recovery.png]({{site.baseurl}}/attachments/ref_00nAL9h3/password-recovery.png)

2. Enter the email address associated with your administrator user account and click **Submit**.
   
   The confirmation URL link will be emailed to you shortly.
   
3. Check your email inbox. 
   
   You should get an email titled **\*\Your_company_name\*\: Confirm password reset request**. 

4. Use the link from this email to initiate the password recovery process. The link from the email will redirect you to the **Change password** page:
   ![password-recovery-2.png]({{site.baseurl}}/attachments/ref_00nAL9h3/password-recovery-2.png)
   
5. Enter a new password for your admin account, confirm the new password and click **Update**.
