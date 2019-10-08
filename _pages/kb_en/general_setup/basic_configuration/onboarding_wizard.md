---
lang: en
layout: article_with_sidebar
updated_at: '2019-06-28 12:29 +0400'
identifier: ref_5xTo5Gmg
title: X-Cart Quickstart Onboarding Wizard
order: 10
published: true
---
When you enter your X-Cart store Admin Home page for the first time after the installation of X-Cart software, you cannot miss the green box that says "Let's set up your store! - **Proceed**". That is the place to start X-Cart's Quickstart Onboarding Wizard. The Onboarding Wizard is an addon that is aimed to help the store administrator with the initial store configuration and setup.

![onboarding-wizard.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/onboarding-wizard.png)

To start the store configuration process using the Onboarding Wizard, click **Proceed**.

{% toc %}

## Onboarding Wizard Welcome

First of all, the Onboarding Wizard will welcome you and provide an outline of the steps that you will need to take to complete your store configuration.

![quickstart-1.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-1.png)

To continue with your store configuration, click **Let's set up your store!**. This will take you to the first step of the wizard.

If you don't wish to use the wizard now, you can close it using one of the buttons: 

* **Skip and remind me later** - This button will close the wizard so it will not be in your way while you are exploring your store's Admin area; however, you will be able to access the wizard at any time later via the green "Let's set up your store!" box.
* **Close and don't show again** - This button will close the wizard for good; the green box will no longer be displayed on the Admin Home page.
 
## Step 1 - Add Your First Product

The wizard will suggest that you should start the store configuration with adding your first product. 

![quickstart-2.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-2.png)

If you are not ready to add a product right now, you can skip this step and add products later. 

Your newly installed X-Cart store has a pack of demo products that you can use to test the basic store functionality.

You can add your own products later on, and not necessarily by doing it manually one-by-one. The built-in {% link "Import-Export" ref_TANvG2De %} tool can help you to add your entire product catalog at once.

If you decide to move on with adding your first product, you will need to name this product, set the product price and upload an image of the product either from your local computer or via URL. (Just tap on the image area to see your options). 

This is what this step may look like after all the required product fields have been completed:

![quickstart-2-2.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-2-2.png)

If you wish to set more product details (like product weight, description, sale price, etc.), use the "Add other options" link. As a result, the full version of the {% link "product details page" ref_2D8wAeXP %} for the product you are configuring will be opened in a new browser tab. There you will be able to finish configuring the product details and save your changes. Again, you do not have to complete all the product fields right now - you can go back to editing any of the products in your store catalog at any time later. Detailed information on how to create and manage products in your X-Cart store without using the Onboarding Wizard and how to configure all the product fields is available in the section {% link "Products and Catalog" ref_uymkBt6a %} of this manual. 

Let us suppose you have configured all the required product fields at the first step of the Onboarding Wizard to create your first product. Now you can click the button **Save and go to the next step**.

The wizard will suggest that you take a look at your new product on the storefront. 

![quickstart-3.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-3.png)

Note that this page also gives you an opportunity to delete all the demo products that are present in your store. You can do that if you are ready to populate the store catalog with your own products. If not, keep the demo products a bit longer. You may need them to test the basic store functioning.

Click **Proceed to the next step** to go further.

## Step 2 - Upload Your Company Logo

In Step 2 you can upload your company logo. By a company logo we mean an image representing your business name that is displayed at the top of all the store pages. The store logo serves not only as branding for your site, but it also links back to your store's home page.
![quickstart-4.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-4.png)

Similarly to a product image, your store logo can be uploaded from your local computer or via URL. Tap on the logo area to see the options. 

As to the recommended size of your company logo image, you do not have to worry too much about resizing the image to a specific size before upload. With X-Cart, you can upload images larger than needed for display; X-Cart will automatically resize them for optimal user experience. In X-Cart versions 5.4 and later, the size to which your company logo image will be resized can be found (and, if necessary, adjusted) via the image size chart provided in the Images section of your X-Cart store Admin area (**Look & Feel** > **Images**). If your store is configured to provide x2 size images for Retina displays (i.e. the setting **generate_retina_images** in the file etc/config.php of your X-Cart installation is set to "On"), the minimum size of an image you should upload for use as your company logo needs to be twice as large as the size specified in the image size chart. For example, in Crisp White skin, according to the image size chart in the Images section, the size to which your uploaded company logo image will be resized is 221х40 px. This means that to ensure optimal image viewing experience for both your regular screen users and Retina screen users, the recommended size of your company logo image for upload should be at least 442x80 px. 

Your store logo will be a part of your company style and will visualize your brand to the site visitors. If you do not have a good selling logo, feel free to [ask](https://www.x-cart.com/contact-us.html#design), and we will be happy to help you with it. 


## Step 3 - Set Up Your Store Locale and Company Info

In Step 3 you can configure the geographic settings to connect your store with local customers and set your company info that will be used to form invoices, send email notifications and calculate shipping rates for your store.

Start with the store locale. The wizard will try to guess your country, currency and weight values based on the info that could be derived during the software installation. However, these values may not be correct. You need to verify the information on the screen and make changes, if required.

![quickstart-5.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-5.png)

If everything is correct, click **Proceed to the next step** to move on with the company details info. 

If you need to go deep into the store localization click **More localization settings** and the wizard will open the Store setup -> Localization page in a new tab where {% link "more options" ref_cc4sCpa5 %} area available.

On the Company info page you'll need to fill in the company name and business address. This address will be used as a "from" address for the store shipping setup.

![quickstart-6.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-6.png)

Click **Save and go to the next step** when you are ready.

## Step 4 - Set Up Delivery Options

Step 4 of your store configuration is devoted to shipping. 

First of all here you'll need to choose whether you'll sell tangible goods that need shipping or whether these will be e-goods and services that are non-shippable. 

![quickstart-7.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-7.png)

If you are selling e-goods and services everything is pretty simple. Click **Mark all products as non-shippable** and that's it! The wizard will set the [Requires shipping product option](https://kb.x-cart.com/products/products/managing_products/adding_products/basic_product_setup.html#shipping) for all products in your store to NO and all shipping methods will be disabled automatically.

If you sell tangible goods, the process is a bit more complicated. You need to set up shipping options for them. For this purpose click the **Set up shipping** button.

You'll see a page where you can configure shipping rates for your store:

![quickstart-7-1.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-7-1.png)

On this page you can choose between shipping carriers with real-time shipping quotes and your own flat shipping rate that you can create directly on this page. Just choose the destination country and set the rate, then click the **Create shipping rate** button. This shipping method will become available at checkout. 

For a more detailed shipping setup click the **Advanced shipping options** button and the wizard will open the Store setup -> Shipping page of the Admin area in the new tab where you can {% link "move on further" ref_3TG6AuN0 %}. 

If you choose real-time shipping carriers, click on the carrier logo and you'll be redirected to the carrier service page to set up an account with them. 

When the shipping setup is over you can proceed to the last step of this wizard - payments setup.

## Step 5 - Set Up Payment Methods

Payment methods setup is the last but not the least step of the Onboarding Wizard. 
![quickstart-8.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-8.png)

X-Cart allows to choose whether you'll use one or more of over 120 integrated online payment systems or whether you will process payments offline by your own means. 

By default, off-line demo payment methods are pre-configured and enabled. They are quite enough to test your new X-Cart store functioning. So if that's the purpose, leave the present configuration settings as is and **Proceed to the next step** (complete the store setup with the wizard).

However, if you want to process real orders, you need to configure real payment methods that will work for your customers. Click the **Set up offline & online payments** button for the wizard to open the Store setup -> Payments page in a new tab. Configure payment methods for your store {% link "following the guides of this manual" ref_Jq6Bsdrt %}. 

Once the payments setup is complete, you are finished and can close the wizard.

![quickstart-9.png]({{site.baseurl}}/attachments/ref_5xTo5Gmg/quickstart-9.png)

Please do mind that the Onboarding Wizard allows setting up the very basic store configuration. For a more robust store setup read on the guides from this manual that are aimed to help you to configure your online store to meet your business requirements and make your dreams of selling online come true!
