title: SVN Working Copy locked
link: https://brianchan.us/home/2011/06/22/svn-working-copy-locked/
author: admin
description: 
post_id: 2095
created: 2011/06/22 11:09:29
created_gmt: 2011/06/22 18:09:29
comment_status: open
post_name: svn-working-copy-locked
status: publish
post_type: post

# SVN Working Copy locked

I had some kind of ssh error when using subversion. I then did a force quit coz it hung for too long. Then when I started svn again but it kept saying my work directory is locked. I am using osx so I did a "Get Info" on my work directory and toggled the "Locked" checkbox but that didn't help. Someone said do a recursive "/Developer/Tools/SetFile -a l", but later on I found out that's a solution for another problem. The root question here for me is, why does svn think that my work directory is locked?