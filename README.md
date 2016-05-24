# Install (Ubuntu):
sudo apt-get install golang python-pygments
- vim ~/.bashrc

```
// add the following 3 lines:
 export GOROOT=/usr/lib/go
 export GOPATH=$HOME/go
 export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
 ```
- source ~/.bashrc
- go get -u -v github.com/spf13/hugo

## Install (OSX)
brew install hugo

...........................................
## create new site
- hugo new site sharon/docroot/ --force
- cd /sharon/docroot && hugo new about.md
- edit config.toml:
# Site settings
contentdir = "content"
layoutdir = "layouts"
publishdir = "public"
canonifyurls = false
baseurl = ""
languageCode = "en-us"
title = "Hugo Freelancer Theme"
theme = "hugo-freelancer-theme"

## test existing site
- hugo server

## generate site files
- hugo -w

hugo -w --source="docroot" & live-server "docroot/public'

.......................................................
