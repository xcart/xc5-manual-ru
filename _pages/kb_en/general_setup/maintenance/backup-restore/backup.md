---
lang: en
layout: article_with_sidebar
updated_at: '2018-03-14 15:40 +0400'
identifier: ref_1kRBEegE
title: Files and Database Backup
order: 120
published: true
redirect_from:
  - /general_setup/backup-restore/backup.html
---
The administrator of an X-Cart based store can back up the database in a few easy steps directly from the Admin area. 

If your X-Cart store uses any 3rd party or custom add-ons, and the data of these addons locate _not_ in the X-Cart database but elsewhere, these data will not include into the database backup created with the X-Cart's standard backup utilities.

Hence there can be cases when you have to back up the database manually, so the dump includes all the store data. For this purpose, you can use any adequate facility, including different client implementations of the SSH protocol like OpenSSH or PuTTY, Telnet, phpMyAdmin, MySQL console, a control panel of your hosting account, Remote Desktop client and other. 

{% toc %}

## Database Backup through the X-Cart Admin Area

To back up the database through the X-Cart Admin area:

 1. Open the "Backup database" page in your store Admin area (**System tools** -> **Database**).
    ![541-database-page.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-database-page.png)
 
 2. Make sure customer storefront is closed as described [here](https://kb.x-cart.com/general_setup/admin/overview.html#storefront-accessibility "Files and Database Backup"):
    ![541-database-page-closed.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-database-page-closed.png)

 3. Create a database backup using one of the following ways: 
    * Download SQL file : An .sql file will be downloaded to your local computer.
    * Create SQL file : An .sql file will be saved on the server your store is hosted at. You will be able to download the file from the server later and, after that, delete it from the server using the "Delete SQL file" button.

      {% note info %}
      If you do not have access to your server/hosting account through FTP, SSH or other suitable facility, use the "Download SQL file" variant and save the SQL file directly to your local computer.
      {% endnote %}

## Database Backup with Terminal Access

To back up the database using terminal access to the server:

1. Log in to your server or hosting account.

2. Go to the X-Cart root directory.

3. Run the following shell command.


```
mysqldump -h<db_host> -u<username> -p<password> -r<backup_filename> <db_name>
```

The abbreviations in the command mean:

{:.ui.compact.celled.small.padded.table}
|db_host | The DNS name or the IP-address of your MySQL server.|
|username | The username for your MySQL user account.|
|password | The password for your MySQL user account.|
|backup_filename | The name and the path to the newly created SQL file with the database dump.|
|db_name | The name of the MySQL database that you use for X-Cart.|


After you have run the command, the system will generate an SQL file and save it to the directory that you have specified in the <backup_filename> part of the command. If you have specified the name of the file for the backup only without mentioning the path, the file will be saved to the X-Cart root directory, the directory where you are currently located.

If necessary, you can use a different path, but it is yet recommended that it be a location within the X-Cart root directory.

## Backup of the Store Files

Creating a backup copy of the store files presumes that you pack all the files in the X-Cart root directory into an archive and then copy or move the archive to a new location on the remote server or your local computer.

{% note info %}
If you have previously saved the database dump into the file in the X-Cart root directory, the file will also be included into the archive.
{% endnote %}

To create an archive you need to use a file archive manager. The exact choice of the archive manager will depend on the operating system you use. On a UNIX-based server, the most popular archive manager, which is currently installed on the majority of servers, is TAR. Later in this section you will find an example of how to archive the X-Cart files with the TAR archive manager. On a Windows-based server, you can create the archive with one of the available file archive managers for Windows, including WinRAR, WinZIP, PKZip and 7Zip. You need to pack the whole X-Cart root directory to an archive and then save the archive to the directory that is parent to the X-Cart root directory.

Alternatively, if it is not possible to pack the X-Cart files into an archive directly on your server, you can copy the X-Cart root directory to your local computer or another remote server using FTP or other suitable facility. Before that, make sure the new location, to which you are planning to copy the X-Cart root directory, has enough free disk space. Besides, the control panel of your hosting provider may offer its own facilities for backing up your account data.

### Files Backup with the TAR Archive Manager (UNIX-based servers only)

In UNIX-based systems, TAR is known to be one of the most reliable and trustworthy utilities for creating and manipulating file archives. It is now commonly used in tandem with external compression utilities like GZIP, BZIP2 or LZMA, which enables you not only to create an archive, but also compress the data in the archive. As a result, with TAR you can create a lightweight archive of your store and then restore it using the same utility. To find out whether TAR is installed on your server, run the following shell command.

```
tar --version
```

If TAR is installed on your server, the system will display a message with the version of the utility; otherwise you will see an error message. In case of the latter, please contact your hosting team for help.

To back up files with the TAR archive manager:

1. Log in to your server or your hosting account.

2. Go to the X-Cart root directory.

3. In the X-Cart root directory run the following shell command.

```
tar -czvf ../store_backup.tgz *
```

After you have run the command, TAR will pack all the files in the X-Cart root directory to the file store_backup.tgz and compress it with the ZIP data compression algorithm. The file will be saved to the directory that is parent to the X-Cart root directory. For example, if the X-Cart root directory is u/user/public_html/xcart, the file store_backup.tgz will be saved to directory u/user/public_html.

## Backup Master Addon

To make the process of creating a full store backup more convenient and straighforward, you can use the [Backup Master](https://market.x-cart.com/addons/backup-master.html "Files and Database Backup") addon for X-Cart. Using this addon facilitates the creation of both database and full store files backups. 

To install the addon, go to the **My addons** section of the Admin area and follow the procedure described in {% link "Activating and Deactivating Addons" ref_uEnDBBA7 %}. 
![541-backup-master-addon-instaled.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-backup-master-addon-instaled.png)

Once the addon has been installed, open the addon settings page to configure the backup method.
![541-backup-master-settings-page.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-backup-master-settings-page.png)

* **Backup mode** : Select a backup mode from the list.
  
  Available options are: 
  * ZipArchive class biult into PHP
  * Linux Shell commands (enabled by default)
  * Linux Shell commands (without compression)
  
  {% note info %}
  Using Linux Shell commands is much faster, so it is the recommended option for Linux servers.
ZipArchive class may fail when working with large backup files, but it is the only option available on Windows servers, unfortunately.
  {% endnote %}

* **Include images into backup** : Turn the toggle on if you want to included images in a backup.
* **Include attachments into backup** : Turn the toggle on if you want to included images in a backup. 

To make a full store backup using the Backup Master addon go to the **System tool** -> **Backup** section and click a **'Create backup'** button.

<div class="ui stackable three column grid">
  <div class="column" markdown="span">![541-backup-master-page-1.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-backup-master-page-1.png)</div>
  <div class="column" markdown="span">![541-backup-master-page-2.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-backup-master-page-2.png)</div>
  <div class="column" markdown="span">![541-backup-master-page-3.png]({{site.baseurl}}/attachments/ref_1kRBEegE/541-backup-master-page-3.png)</div>
</div>

The addon will create a full cart backup and will list it in a history of backups where you can see a path to a backup file, a file size and date of creation. 

To delete a backup click the "Trash" icon next to it.
