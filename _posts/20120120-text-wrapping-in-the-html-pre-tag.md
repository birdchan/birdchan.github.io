title: text wrapping in the html pre tag
link: https://brianchan.us/home/2012/01/20/text-wrapping-in-the-html-pre-tag/
author: admin
description: 
post_id: 2535
created: 2012/01/20 15:49:39
created_gmt: 2012/01/20 23:49:39
comment_status: open
post_name: text-wrapping-in-the-html-pre-tag
status: publish
post_type: post

# text wrapping in the html pre tag

If you ever have a <pre> tag in a div or table, and you are providing say text from your database to the pre element, be very careful that the default style of the pre tag will let the text keep running until hitting the newline character. This is probably not desirable because these long text lines will push their container thus expanding the container unexpectedly.