---
lang: en
layout: article_with_sidebar
updated_at: '2019-06-19 14:24 +0400'
identifier: ref_0aebLCRA
title: Server Requirements
order: 100
published: true
---
Before you get started with the {% link "software installation" ref_VG5mIoLT %} you should check whether your web server spec meets the X-Cart system requirements. 

{% toc %}

## System Requirements

Here is the system requirements list:

*   **X-Cart v5.4.0.x and later** : PHP __7.2__ or higher / MySQL __5.7.7__ or higher

    **X-Cart v5.3.4.5 and later** : PHP __5.4__ - __7.2__  / MySQL __5.1.31__ or higher
    
    {% note info %}
    You can also use the MySQL-compatible database engine MariaDB (minimum allowed MariaDB version is 10.2.4). 
    {% endnote %}
    
*   __PDO__ extension with MySQL driver
*   __Phar__ extension (Required for the processes of updating/upgrading your X-Cart 5 store and addon installation. Phar version requirements may differ depending on the other components of your system. If you experience problems while trying to run an update/upgrade or to install an addon, try using Phar v.2.0.1 or later.)
*   __mbstring__ extension is highly recommended (though X-Cart has a polyfill for it, native extension will speed up string processing)
*   200-300Mb of disk space
*   libCURL module support (The minimum required CURL version is 7.39.0; version 7.43.0 is recommended.)
*   `ini_set` enabled
*   `safe_mode` disabled
*   `file_uploads`  enabled
*   `post_max_size` set to 2M+ and larger than the `upload_max_filesize` value (critical for installation)
*   `upload_max_filesize` set to 2M or higher
*   `magic_quotes_runtime` disabled (for PHP versions prior to 5.4.x)
*   `memory_limit` set to 128M or higher (if you are using 64-bit processors in your server environment, the `memory_limit value` must be 256M or higher)
*   GDLib 2.0 or ImageMagick (recommended for proper image resizing routines)
*   {% link "PHP time limit" ref_xqnpttd4 %} properly set according to your server config
*   mod_rewrite-like components to enable proper work of {% link "SEO-friendly URLs" ref_nJxrzFEZ %}
*   if xdebug is enabled, `xdebug.max_nesting_level` must be set to 300
*   if OPcache is enabled, the following settings must be applied: 
	
	```
	opcache.use_cwd=1
	opcache.revalidate_path=1
	opcache.validate_timestamps=1
	opcache.revalidate_freq=0
    opcache.save_comments=1
    opcache.load_comments=1
    ```
    
    Any other cachers should not strip comments from the code, too.
*   [Suhosin](https://suhosin.org/stories/index.html "Installation Guide") PHP extension might interfere with the proper work of X-Cart 5, so you should disable it. 


## Hardware Requirements

{% note warning %}
X-Cart does NOT recommend shared web hosting due to limited resources. Please consider using VPS or dedicated servers as a host for your store. 

Use only \*NIX-based servers (Ubuntu, Debian, CentOS etc.)!
{% endnote %}

<table class="ui celled padded compact small table">
  <thead>
    <tr>
      <th style="text-align: center;" class="confluenceTh">&nbsp;</th>
      <th colspan="5" style="text-align: center;" class="confluenceTh">Traffic (Visitors/Month)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Catalog size</strong></td>
      <td><strong>up to 2K</strong>
      </td>
      <td><strong>2K-10K</strong>
      </td>
      <td><strong>10K-50K</strong>
      </td>
      <td><strong>50K-100K</strong>
      </td>
      <td><strong>over 100K</strong>
      </td>
    </tr>
    <tr>
      <td><p><strong>up to 1000 SKUs</strong></p><p><strong>up to 100 Categories</strong></p></td>
      <td>
        <p>VPS hosting</p>
        <p>- 1 Core</p>
        <p>- 1 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 1 Core</p>
          <p>- 2 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 2 Core</p>
        <p>- 4 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 8 Core</p>
          <p>- 16 GB RAM (DDR4)</p>
      </td>
      <td>Dedicated server
      </td>
    </tr>
    <tr>
      <td><p><strong>up to 10 000 SKUs</strong></p><p><strong>up to 500 Categories</strong></p></td>
      <td>
        <p>VPS hosting</p>
        <p>- 1 Core</p>
        <p>- 2 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 1 Core</p>
          <p>- 2 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 2 Core</p>
          <p>- 4 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 8 Core</p>
          <p>- 16 GB RAM (DDR4)</p>
      </td>
      <td>Dedicated server
      </td>
    </tr>
    <tr>
      <td><p><strong>up to 20 000 SKUs</strong></p><p><strong>up to 1000 Categories</strong></p></td>
      <td>
        <p>VPS hosting</p>
        <p>- 2 Core</p>
          <p>- 4 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 2 Core</p>
          <p>- 4 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 8 Core</p>
          <p>- 16 GB RAM (DDR4)</p>
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
    </tr>
    <tr>
      <td><p><strong>up to 50 000 SKUs</strong></p><p><strong>up to 2000 Categories</strong></p></td>
      <td>
        <p>VPS hosting</p>
        <p>- 8 Core</p>
          <p>- 16 GB RAM (DDR4)</p>
      </td>
      <td>
        <p>VPS hosting</p>
        <p>- 8 Core</p>
          <p>- 16 GB RAM (DDR4)</p>
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
    </tr>
    <tr>
      <td><p><strong>over 50 000 SKUs</strong></p><p><strong>over 2000 Categories</strong></p></td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
      <td>Dedicated server
      </td>
    </tr>
  </tbody>
</table>

## Not Supported

* LiteSpeed
