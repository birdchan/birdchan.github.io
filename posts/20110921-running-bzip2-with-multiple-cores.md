title: Running bzip2 with multiple cores
link: https://brianchan.us/home/2011/09/21/running-bzip2-with-multiple-cores/
author: admin
description: 
post_id: 2277
created: 2011/09/21 19:41:32
created_gmt: 2011/09/22 02:41:32
comment_status: open
post_name: running-bzip2-with-multiple-cores
status: publish
post_type: post

# Running bzip2 with multiple cores

I was trying to bzip a 40Gb file and it was taking forever. I then checked the Activity Monitor. It turns out the default bzip was only using one cpu core!!! If you really want to make use of your other cpu cores while doing bzip'ing, here is a nice way I found.