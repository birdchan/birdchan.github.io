---
layout: post
title: Reattach to a terminal process when x11 is restarted
date: 2016/07/22 13:27:39
---

Let me describe my case. I was running 4 long commands in 4 terminals. They were all splitting out log files to stdout so I could see the progress. Then all of a sudden I found my X11 frozen. I thought it would just go away when my tasks became less busy. But after like an hour I decided that I needed to do something since my screen was still frozen. I grabbed my laptop and ssh'ed to my box and found the 4 tasks still running, so the system is ok. Then I had no choice but to restart my display session. I did:

```
sudo restart lightdm
```

Depending on your display manager, you may run slightly [different commands](http://askubuntu.com/questions/1220/how-to-restart-x-window-server-from-command-line). Then I saw my login window came back. I logged back in, and it was a clean empty desktop. I did a **top** and saw that my 4 tasks were still running. So now, it would be nice to see the stdout lines they spit out.

I found many articles talking about gdb. I tried once but was too scared to move forward. Then I found this tool called **strace**, which really does the thing I wanted. The command is:

```
sudo strace -ewrite -p 12345 -s 1024
```

The **-p** flag is to specify your task’s PID. The **-s** flag is to specify the length of your line, default is 32 characters but it is not quite readable.

When you run that, the output from your task comes out which is good. However the output line is a bit strange. It would look something like the following.

```
write(1, "The output of your original line\n", NNN) = NNN
```

The **NNN** is the length of your line I guess. But if you really want to take away the extra prefix and suffix, here is the command you want:

```
sudo strace -ewrite -p 12345 -s 1024 2>&1 | sed -r 's/write\(1, \"(.*)\\n\"(.*)/\1/'
```

strace prints things out to stderr, so the **2>&1** is to redirect the output back to stdout for us to pipe. The **sed** is just using regex match to parse out the middle part.


