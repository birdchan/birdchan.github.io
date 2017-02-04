title: Git push asks for username and password
link: https://brianchan.us/home/2015/03/16/git-push-asks-for-username-and-password/
author: admin
description: 
post_id: 4214
created: 2015/03/16 18:54:27
created_gmt: 2015/03/17 01:54:27
comment_status: open
post_name: git-push-asks-for-username-and-password
status: publish
post_type: post

# Git push asks for username and password

If **git push** keeps asking you for user/pass, chances are that you did a **git clone** using HTTPS. Fix that by going to your repo page on github, then click on the SSH link below the **clone URL** field, then copy that URL over (something like **git@github.your_username/your_repo_name.git**). Then update your local git repo with something like the following command

## Comments

**[isprogfun](#276090 "2015-04-22 04:17:30"):** Thank you!

