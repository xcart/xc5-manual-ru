---
lang: en
layout: article_with_sidebar
updated_at: '2017-01-15 07:19 +0400'
identifier: ref_RrLo9hcw
title: Changing Logo Size (for Crisp White Skin)
order: 200
published: true
redirect_from:
  - /look_and_feel/changing_logo_size_for_crisp_white_skin.html
---
For Crisp White skin, the default logo block height is 60px, and the default menu block height is 60px; the total height of the header block is 140px (as regards to the desktop view).

If you want to use a larger logo image, you will need to increase the height of these blocks, respectively.

{% note info %}
The logo's height of 60px is not a random value. This way we make sure that the top menu is not too large and it does not eat up too much space, which otherwise could have been used to display relevant content to your customers.

If you need to enlarge the logo's height, please consider a possibility of making your logo image fit into 60px height. It will probably be overall better solution for the look of your store.
{% endnote %}

{% note info %}
Before deploying the changes make sure they do not interfere with the modifications applied via the {% link "Custom CSS" ref_10vugyja %} feature. 

Check the **Custom CSS** section of the store admin area (**Look & Feel** -> **Custom CSS & JS**) for any possible code added.
{% endnote %}

For example, let's add 20px to the height of the logo and menu blocks, and also add 40px to the height of the header block. Here is the code that should be added to your "Custom CSS" section:

```
/* DESKTOP VIEW */

/* Increase total height of header block +40px */
@media (min-width: 992px) {
  #header-area:after {
    margin-top: 180px;
  }
}

/* Increase logo and menu blocks height +20px */
@media (min-width: 992px) {
  #logo, .company-logo {
    height: 80px;
  }
  #header-bar {
    height: 80px;
  }
}

.header-right-bar {
  height: 80px;
}

/* Increase logo image height +20px */
#logo img, .company-logo img {
  max-height: 60px;
}

/* Adjust paddings for menu items */
/* Original padding: 20px 17px; */
.navbar-nav>li>a, .navbar-nav>li>span {
   padding: 30px 17px 25px 17px;
}

```

As regards the mobile view, let's increase the height of the header and logo blocks too (by adding +20px), e.g.:

```
/* MOBILE VIEW */

/* Increase header block height +20px */
@media (max-width: 991px) {
  #header-area:after {
    margin-top: 100px;
  }
}

/* Increase logo block height +20px */
.mobile_header ul.nav-pills {
  height: 80px;
}

/* Adjust paddings for menu items */
/* Original padding: 20px 10px; */
.mobile_header .nav .mobile_header-slidebar a {
  padding: 30px 10px;
}

/* Increase logo image height +20px */
.mobile_header .nav .mobile_header-logo #logo img, .mobile_header .nav .mobile_header-logo .company-logo img {
  max-height: 80px;
}

```
