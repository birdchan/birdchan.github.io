title: Datatable clear filtering
link: https://brianchan.us/home/2012/11/26/datatable-clear-filtering/
author: admin
description: 
post_id: 3164
created: 2012/11/26 13:04:10
created_gmt: 2012/11/26 21:04:10
comment_status: open
post_name: datatable-clear-filtering
status: publish
post_type: post

# Datatable clear filtering

Here is how to clear all filtering in [datatable](http://datatables.net/).

## Comments

**[May Saghira](#78826 "2013-12-24 14:19:09"):** Yeah it clears the filtering but it doesn't clear the input filter ... plz how can i do it ??

**[deva](#87683 "2014-02-19 07:46:47"):** oTable.fnDraw();

**[deva](#87684 "2014-02-19 07:47:46"):** use pcsTable.fnFilter(""); insted of oTable.fnDraw();

**[Jas](#109211 "2014-04-29 05:52:43"):** Wow ! This is what I had been looking for ! Works great !

