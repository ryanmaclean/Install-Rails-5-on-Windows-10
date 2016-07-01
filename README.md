# Install Ruby on Rails 5 on Windows 10

## Install Git Bash

First, we'll install Git for Windows, which comes with Git Bash which also happens to include Msys2: https://git-scm.com/download/win

If you already have [Chocolatey](https://chocolatey.org/install) installed: `choco install git.install`

## Install Ruby

From within Git Bash, run `pacman -S ruby gcc --noconfirm`

## Install Ruby on Rails 5

Again from Git Bash, run `gem install rails -V`

This will take several minutes.

## Test Rails

In order to test your install, type the following: `rails new app`
