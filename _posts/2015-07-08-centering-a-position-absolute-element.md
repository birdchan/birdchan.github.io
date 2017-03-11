---
layout: post
title: "Centering a position:absolute element"
date: 2015/07/08 11:02:37
---

Sometimes we have a one-line div, having 3 elements. One floats to the left, one floats to the right, and one in the middle. The one in the middle often gets pushed around by the left/right element, resulting off-centered. [related question](http://stackoverflow.com/questions/2603700/how-to-align-3-divs-left-center-right-inside-another-div).

```
<div id=container class=text_align_center>
  <div class=float_left></div>
  <div class=float_right></div>
  <div class=center></div>
</div>
```

The fix is to give the following css to the center div.

```
position: absolute;
margin-left: auto;
margin-right: auto;
left: 0;
right: 0;
```

Thanks to the following link. =)

[http://stackoverflow.com/questions/8508275/how-to-center-a-position-absolute-element](http://stackoverflow.com/questions/8508275/how-to-center-a-position-absolute-element)






