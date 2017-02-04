title: jeditable textile textarea renderer issue
link: https://brianchan.us/home/2012/02/24/jeditable-textile-textarea-renderer-issue/
author: admin
description: 
post_id: 2695
created: 2012/02/24 19:28:30
created_gmt: 2012/02/25 03:28:30
comment_status: open
post_name: jeditable-textile-textarea-renderer-issue
status: publish
post_type: post

# jeditable textile textarea renderer issue

If you have ever played with jeditable, eventually you will get to this issue, which is dealing with the textarea. The [Textile renderer](http://www.appelsiini.net/projects/jeditable/default.html) on the official jeditable demo page works perfectly fine, but when I tried it I experienced quite some difficulty.

## Comments

**[mark pollak](#3880 "2012-05-09 11:17:22"):** hi

**[Brian](#3912 "2012-05-14 10:53:40"):** Hey Mark, try changing that line to the following see if it works? Basically I took away the double quote escaping.

**[Geffrey](#5814 "2012-08-18 08:41:40"):** Okay, ran into this problem too. Yet, I'm not sure where to put the str_replace , in my save script... or load page?

**[Brian](#5819 "2012-08-18 13:33:09"):** Hey Geffrey, your save script and load script should just do the plain saving and loading operations. That is to say, in your database table, you should not have any "<br>"s.

**[masaki](#44216 "2013-03-27 05:25:58"):** Hi I´ve published on jquery forum a cleanup on the textarea by vonverting back to new line and cleaning up extra new line may have.

**[masaki](#44219 "2013-03-27 05:35:33"):** Little adjust to replace all not just first

**[Tina](#39981 "2013-03-08 01:18:10"):** "Hope this can save you some time" << it DID! Thanks a alot!

**[don](#217192 "2014-10-30 11:20:37"):** actually for this work without issue the code needs both callback and data functions:

