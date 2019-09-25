---
lang: en
layout: article_with_sidebar
updated_at: '2019-05-27 13:45 +0400'
identifier: ref_1i0r1QYO
title: Does X-Cart 5 Have to Be On the Same Server?
order: 30
published: true
redirect_from:
  - >-
    /general_setup/migration/migration-from-xcart4/step-1-new-or-same-server.html
  - /migration/migration-from-xcart4/step-1-new-or-same-server.html
---
The short answer is no, but there are subtle details. 

There are three possible cases of how your X-Cart 4 and X-Cart 5 stores can be installed.

1. You install X-Cart 5 on the same server as X-Cart 4. In this case, everything will just work.

2. You want to install X-Cart 5 on another server (some test server, local machine, etc). If you transfer the entire X-Cart 4 store there, everything will work just fine as well. 

	To make X-Cart 4 transfer easier, you can only transfer X-Cart 4's database and the following directories to save you some time:
	- `<X-Cart>/images/`;
	- `<X-Cart>/skin/common_files/pages/`;
	- `<X-Cart>/files/`, if you have e-goods.


	Put the database to MySQL server and place these directories inside some folder that would 'pretend' being X-Cart 4 for our migration task.

3. You want to install X-Cart 5 on a new server, but keep X-Cart 4 on the old one. To make this case is possible, you need to:
	- make sure that the MySQL on X-Cart 4 server allows remote connections. Contact your hosting team about that, if you face any troubles;
	- set the _enable_copy_ext_images_ option in {% link "Migration Wizard's settings" ref_1IAKq4cq %} to 'true'.
