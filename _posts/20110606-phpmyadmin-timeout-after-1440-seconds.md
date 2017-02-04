title: phpMyAdmin timeout after 1440 seconds
link: https://brianchan.us/home/2011/06/06/phpmyadmin-timeout-after-1440-seconds/
author: admin
description: 
post_id: 2077
created: 2011/06/06 16:30:17
created_gmt: 2011/06/06 23:30:17
comment_status: open
post_name: phpmyadmin-timeout-after-1440-seconds
status: publish
post_type: post

# phpMyAdmin timeout after 1440 seconds

I keep getting this timeout error from phpmyadmin: "**No activity within 1440 seconds; please log in again**". @#%@#$@$@ So I decided to change that setting. Open up your config.inc.php file and add the following line: (If you don't have config.inc.php, copy from config.sample.inc.php)

## Comments

**[subhojit777](#4900 "2012-07-10 00:05:53"):** Superb and complete article. Thanks :)

**[bird](#4904 "2012-07-10 01:30:33"):** nice

**[mahrizal](#35339 "2013-02-05 21:33:57"):** Thanks....

**[Senatoz](#38371 "2013-02-28 05:01:54"):** THANKS!

**[Joe](#57755 "2013-06-23 19:13:12"):** Instead of setting the global session timeout, the following solution might be better in a secure environement:

**[Gawain Lynch](#91172 "2014-03-15 01:10:47"):** Thanks mate, really good.

