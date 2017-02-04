title: Commit failed (details follow): File 
link: https://brianchan.us/home/2011/11/30/commit-failed-details-follow-file-your_file-is-out-of-date/
author: admin
description: 
post_id: 2413
created: 2011/11/30 14:12:06
created_gmt: 2011/11/30 22:12:06
comment_status: open
post_name: commit-failed-details-follow-file-your_file-is-out-of-date
status: publish
post_type: post

# Commit failed (details follow): File 

I have no idea, but all of a sudden I got this svn error during my commit.

## Comments

**[Michael Nesterenko](#2817 "2011-12-17 17:28:22"):** Hello, that is not a workaround, you just loose changes that came from svn server. Committing your changes involves clearing changes made by someone else. Instead you have to update and let svn merge (possible resolving conflicts) your and some one else's changes, and only then commit.

