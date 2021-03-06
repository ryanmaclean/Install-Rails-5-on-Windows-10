# Install Ruby on Rails 5 on Windows 10

## Install Git Bash

First, we'll install Git for Windows, which comes with Git Bash which also happens to include Msys2: https://git-scm.com/download/win

If you already have [Chocolatey](https://chocolatey.org/install) installed: `choco install git.install`

## Install Ruby

From within Git Bash, run `pacman -S ruby gcc libcrypt-devel --noconfirm`

## Update Gems

Run the following in order to update install gems: `gem update`

## Install Nokogiri

We'll manually install this as it's still problematic on Windows, though the next release promises to address some of the issues: 

```
wget https://rubygems.org/downloads/nokogiri-1.6.5-x64-mingw32.gem
gem install nokogiri-1.6.5-x64-mingw32.gem
```

## Install Ruby on Rails 5

Again from Git Bash, run `gem install rails -V`

This will take several minutes.

## Test Rails

In order to test your install, type the following: `rails new app`
