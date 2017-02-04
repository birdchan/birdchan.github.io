title: osx Lion mysql sock path
link: https://brianchan.us/home/2011/07/20/osx-lion-mysql-sock-path/
author: admin
description: 
post_id: 2153
created: 2011/07/20 12:57:25
created_gmt: 2011/07/20 19:57:25
comment_status: open
post_name: osx-lion-mysql-sock-path
status: publish
post_type: post

# osx Lion mysql sock path

I just installed Lion and for some reasons my internal website stopped working due to the mysql lock file not being found. I found out that the new osx installation changed the mysql sock file default path from /var/mysql/mysql.sock to **/tmp/mysql.sock**.

## Comments

**[Trevor](#2046 "2011-08-10 20:24:24"):** I guess it right, you're one of the best out there in what you do. Cheers

**[Federico Bozo](#2005 "2011-07-29 12:34:19"):** Thank you very much! :D

**[Miguel](#1987 "2011-07-23 20:05:53"):** Thanks very much for the timely tip

**[W](#1984 "2011-07-23 15:26:49"):** You saved my day! Now I'll have to figure out how to live without Adobe.

**[Rob](#2084 "2011-08-19 22:30:30"):** Thanks for this, had just installed a clean version of Lion and was migrating stuff manually from Snow Leopard. This was what I was missing :-)

**[Jon](#2088 "2011-08-20 14:48:56"):** Thank you, quick easy fix. Seems like someone at apple could figure this out, when I installed mysql the first time it was a nightmare.

**[Michael](#1980 "2011-07-22 11:51:04"):** Thank you so much. That did it. Totally awesome.

**[Kyle](#1981 "2011-07-23 01:12:19"):** thank you. How in the world did u figure this out?

**[Angel](#1975 "2011-07-21 22:26:07"):** Found this after trying to solve it for 6 hours (reinstalled mysql, etc). FML, but thanks!

**[Brian](#1966 "2011-07-20 23:41:19"):** Hi Ngoc, did you replace all the "/var/mysql/mysql.sock" in your php.ini file? If so, be sure to restart your apache.

**[rayjnorris](#1971 "2011-07-21 16:17:36"):** wow - what a life saver .....

**[Jay](#1962 "2011-07-20 13:21:19"):** Thanks for this! Totally solved my problem. :)

**[Ngoc Pham](#1967 "2011-07-21 00:05:56"):** Sorry I got it work. My fault! I did not check the php.ini file carefully :(

**[Jay Haase](#1969 "2011-07-21 12:40:49"):** Dude! Thanks, your steps worked for me and I feel 100% less frustrated now.

**[Ngoc Pham](#1965 "2011-07-20 23:27:13"):** Doesn't work for me although I think it's correct as I still can connect to MySQL server from command-line and there is "mysql.sock" file in /private/tmp/ directory.

**[Frank](#2538 "2011-11-20 07:24:00"):** Thx, at last this solved my probs.

**[Fernando](#2603 "2011-11-30 16:01:50"):** Thanks!! really helpful

**[Antony Koch](#4318 "2012-06-10 07:42:32"):** Nice one for this!

**[Roosevelt](#62952 "2013-08-26 13:02:02"):** Thanks dude! Don't know why these guys cannot keep things consistent ><!

