---
layout: post
title: "ImportError: No module named MySQLdb"
date: 2016/06/28 21:10:04
---

I was trying to run GAE dev_appserver.py on my osx El Capitan, and kept getting that ImportError. I fixed it by

```
pip install MySQL-python
```

If still no use, try

```
easy_install mysql-python
```


