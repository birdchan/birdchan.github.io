---
layout: post
title: How to install Octave on OS X
date: 2016/06/09 23:17:30
---

I am taking Andrew Ng's [Stanford Machine Learning Class](https://www.coursera.org/learn/machine-learning/). It is required to install octave for the class assignments.

For the benefit of everyone, I want to type out all the steps I took to install octave on my osx El Capitan. Certainly you could just download the pre-built binary at the [official octave site](https://www.gnu.org/software/octave/download.html), but only if your internet connection is fast and stable. I am taking the homebrew path.

Oh… you have Xcode right??? Um… if not, install it first at the Mac App Store. Be warned Xcode is quite large and will take some time to install… ^^;

```
# install Homebrew http://brew.sh/
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# tap the science formulae
brew tap homebrew/science

# update/upgrade brew
brew update && brew upgrade

# install gcc, this will take like an hour to compile...
brew install gcc

# install xquartz
brew install Caskroom/cask/xquartz

# install octave
brew install octave

# install fltk for gnuplot
brew install fltk

# fix fontconfig
brew uninstall fontconfig
brew install fontconfig --universal

# install gnuplot
brew install gnuplot

# optional: if you don't want to use xquartz, you can use qt
brew uninstall gnuplot
brew install gnuplot --with-qt
```

Then you could run octave by issuing **octave** in your terminal.

ref:

[https://adampash.com/how-to-install-octave/](https://adampash.com/how-to-install-octave/)
[http://stackoverflow.com/questions/35249881/octave-fontconfig-error](http://stackoverflow.com/questions/35249881/octave-fontconfig-error)





