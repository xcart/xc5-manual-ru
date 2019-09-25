---
lang: en
layout: article_with_sidebar
updated_at: '2019-09-18 13:17 +0400'
identifier: ref_1C23rFdB
title: 'Step 1: Migration environment'
order: 10
published: true
---
The first step of your X-Cart v4 based store upgrade to v5 is environment preparation.

The preparation step includes:

* checking what data can be migrated from your current XC4 based store to a new XC5 store automatically using the {% link "XC4 to XC5 Migration Wizard" ref_enOvcLbO %}.
  
  In case any data can't be migrated from XC4 automatically and you want to have them in your new XC5 based store, you'll need to transfer such data manually after the main data migration is complete. If you need help, [contact X-Cart Team](https://www.x-cart.com/contact-us.html "Step 1: Migration environment").

* checking the current server for compatibility with {% link "XC5 system requirements" ref_3olOLKdu %} and for enough disk space to run 2 X-Cart stores at a time. 
  
  In case your current server needs enhancements either in properties or in disk space or even in both make sure to upgrade the current server or find a new better one or perform the upgrade on your local machine if it suits the requirements.

* installing a fresh X-Cart 5 based store as described in the {% link "Installation Guide" ref_VG5mIoLT %}.
  
  {% note info %}
  Do not apply any customizations to X-Cart 5 before running the migration process and also make sure to remove all demo data from the installation. You can remove existing data from X-Cart via **System tools** -> **Remove data** section of your X-Cart 5 Admin area.
  {% endnote %}

* fine-tuning X-Cart 5 advanced settings for a smooth migration process.

All the preparation steps are described in details in the guides of this section.

_In this section:_
*   {% link "What Data Is Migrated?" ref_32GoV7A0 %}
*   {% link "System Requirements for X-Cart 4 to X-Cart 5 Migration" ref_19hsx4O9 %}
*   {% link "Does X-Cart 5 Have to Be On the Same Server?" ref_1i0r1QYO %}
*   {% link "Installation Guide" ref_VG5mIoLT %}
*   {% link "Advanced Settings" ref_1IAKq4cq %}

_Read on:_
*   {% link "Step 2: Initial Data Migration" ref_5IyEU6KK %}
*   {% link "Step 3: Migration Checklist " ref_00LtsZrX %}
*   {% link "Step 4: X-Cart 5 Goes Live" ref_2c9QNlDx %}
*   {% link "Step 5: Performance Check-Up" ref_56ZrgCGO %}
