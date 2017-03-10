---
layout: post
title: Fix apache2 after upgrading to ubuntu 16
date: 2016-10-16 16:01:07
---

After upgrading to ubuntu 16, my wordpress was acting weird. I get errors like **apache2.service – LSB: Apache2 web server Loaded: loaded (/etc/init.d/apache2; bad; vendor preset: enabled) Drop-In: /lib/systemd/system/apache2.service.d └─apache2-systemd.conf Active: failed (Result: exit-code)**, and **Your PHP installation appears to be missing the MySQL extension which is required by WordPress.**

Here are some of the steps I took to re-enabled my blog.
If you are using php 7.0, then do

```
sudo a2dismod php5
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt-get install php7.0
sudo apt-get install php7.0-mysql
sudo a2enmod php7.0
sudo systemctl restart apache2
```

Then then your blog should get back up, but for me all of my blog post content are missing. I still can see the post content in the editor, but not on the webpage. It turns out some of the plugins were not up-to-date yet. So turn on/off and update your plugins and at the end your posts should get back to normal.

**ref:**
[https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-lamp-on-ubuntu-16-04](
https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-lamp-on-ubuntu-16-04)
[https://www.digitalocean.com/community/tutorials/how-to-upgrade-to-php-7-on-ubuntu-14-04](https://www.digitalocean.com/community/tutorials/how-to-upgrade-to-php-7-on-ubuntu-14-04)

