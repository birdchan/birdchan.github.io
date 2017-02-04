title: Reattach to a terminal process when x11 is restarted
link: https://brianchan.us/home/2016/07/22/reattach-terminal-process-x11-restarted/
author: admin
description: 
post_id: 4332
created: 2016/07/22 13:27:39
created_gmt: 2016/07/22 20:27:39
comment_status: open
post_name: reattach-terminal-process-x11-restarted
status: publish
post_type: post

# Reattach to a terminal process when x11 is restarted

Let me describe my case. I was running 4 long commands in 4 terminals. They were all splitting out log files to stdout so I could see the progress. Then all of a sudden I found my X11 frozen. I thought it would just go away when my tasks became less busy. But after like an hour I decided that I needed to do something since my screen was still frozen. I grabbed my laptop and ssh'ed to my box and found the 4 tasks still running, so the system is ok. Then I had no choice but to restart my display session. I did: