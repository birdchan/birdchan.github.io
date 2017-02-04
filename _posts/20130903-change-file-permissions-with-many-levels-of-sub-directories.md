title: Change file permissions with many levels of sub-directories
link: https://brianchan.us/home/2013/09/03/change-file-permissions-with-many-levels-of-sub-directories/
author: admin
description: 
post_id: 3637
created: 2013/09/03 14:46:36
created_gmt: 2013/09/03 21:46:36
comment_status: open
post_name: change-file-permissions-with-many-levels-of-sub-directories
status: publish
post_type: post

# Change file permissions with many levels of sub-directories

Sometimes you need to set o+x to all sub directories recursively, but don't want to set that for any files. (**chmod -R o+x *** is overkill...) Here is how.