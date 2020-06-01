---
lang: en
layout: article_with_sidebar
updated_at: '2018-03-12 15:45 +0400'
identifier: ref_10vugyja
title: Custom CSS
order: 130
published: true
---
**Custom CSS** is a tool of the {% link "Theme Tweaker" ref_2Kfe2OX6 %} addon that aims at changing the design elements of the skin and adding a custom CSS code to the existing X-Cart pages so that a modified code is aggregated with the other software files automatically. Using **Custom CSS** you can change the skin colors, fonts, background, etc.

{% toc %}

## Adding Custom CSS Code to the Site

All changes that are applied through the **Custom CSS** tool facilities are applied storewide (i.e. to a store as a whole, but not to a single page of a store) and are recorded in the **Look and Feel** > **Custom CSS & JS** section of your store Admin area. 

### Adding Custom CSS Code in the Admin Area

To add Custom CSS code:

1. Open the **Custom CSS** section of the Admin area (**Look & Feel** -> **Custom CSS & JS**)
   ![custom_css.png]({{site.baseurl}}/attachments/ref_10vugyja/custom_css.png)
2. Turn on the **Use custom css** toggle
3. Clean the text area beneath the toggle and paste your custom CSS code there
   ![code_deleted_1.png]({{site.baseurl}}/attachments/ref_10vugyja/code_deleted_1.png)
4. **Save** the changes.

### Adding Custom CSS Code in the Storefront

If you need to see the changes while you are adding them, use the **Webmaster mode** -> **Custom CSS** tool in the store frontend. 

{% note info %}
Please don't forget to be logged in as an admin.
{% endnote %}

For this purpose: 
1. Enable the Webmaster mode by clicking the ‘Gear’ icon in the bottom left corner.
2. Choose the **Custom CSS** tool and turn ON the _Use Custom CSS_ option.
   ![custom_css_customer.png]({{site.baseurl}}/attachments/ref_10vugyja/custom_css_customer.png)
   
   {% note info %}
   The custom css code that you see when opening the tool for the first time is a demo one that represents the basic page layout structure. You can edit the code or delete it completely. The code deletion will not affect the skin anyhow.
   
   ![code_deleted_2.png]({{site.baseurl}}/attachments/ref_10vugyja/code_deleted_2.png)
   {% endnote %}
3. Paste your custom CSS code to the text area.
4. Save the changes.

Let's check how the skin changes are applied based on the demo css code provided. 

The figures below show one and the same page with the custom css code enabled and disabled.

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![css_off.png]({{site.baseurl}}/attachments/ref_10vugyja/css_off.png)</div>
  <div class="column" markdown="span">![css_on.png]({{site.baseurl}}/attachments/ref_10vugyja/css_on.png)</div>
</div>

As you see the custom css code changes the background and positioning of the main blocks of the sidebar (Categories, Sale, New arrivals Recently viewed and so on). 

The blue background and the font color is set by the following piece of code:

```
/**
 * Specific styles for the Top categories block in the side bar
 */
.sidebar .block.block-top-categories .head-h2 {
  background: #f7fcff;
}

.sidebar div.block.block-top-categories div.content {
  background: #f7fcff;
}

.sidebar div.block.block-top-categories div.content a {
  color: #6f9cd9;
}
```

If we change #f7fcff to #F5F5DC the background will look as follows:

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![css_blue.png]({{site.baseurl}}/attachments/ref_10vugyja/css_blue.png)</div>
  <div class="column" markdown="span">![css_beige.png]({{site.baseurl}}/attachments/ref_10vugyja/css_beige.png)</div>
</div>

You can use the demo css code to learn how to apply similar changes to your store skin. 

## Adding JS Code to the Site

It's also possible to add javascrips to your site. 

For this purpose:
1. Open **Custom JavaScript** section of the Admin area (**Look and feel** -> **Custom CSS & JS**).
   ![custom_JS.png]({{site.baseurl}}/attachments/ref_10vugyja/custom_JS.png)
2. Turn the **Use custom js** toggle on
3. Paste your custom JS code to the text area.
4. Save the changes.

Javascripts are stored in one file and both custom CSS and JS are added to the <HEAD> tag after all style files applied.
