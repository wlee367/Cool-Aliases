# Cool-Aliases
#### This summer while working at a web dev company, the computer I got to use had some sweet Aliases set up for terminal in the Mac OS environment.
##### I would like to start a big ReadMe that has all the cool aliases for commands we use every day! Feel free to contribute if you would like.

Formatting changes and more aliases coming soon. 

```
Changing directories -> MULTIPLE LEVELS

alias -='cd -'
alias ..='cd ..'
alias ...='cd ../..'
alias ....='cd ../../..'
alias .....='cd ../../../..'
```
--------------------------------------------------------------------------------------
```
For those of you who work a lot with Apache... (needs Apache configured of course)

alias are='sudo echo "Restarting Apache..."; sudo apachectl graceful'
alias astart='sudo echo "Starting Apache..."; sudo apachectl start'
alias astop='sudo echo "Stopping Apache..."; sudo apachectl stop'
```
--------------------------------------------------------------------------------------
```
For those of you who like to use Apache to set up a local host for your web dev needs

alias edithost='subl -n /etc/hosts'
alias editvhost='subl -n ~/Sites/httpd-vhosts.conf'

*I should point out here that your httpd-vhosts.conf can be in a different directory, but you can figure that out
```
--------------------------------------------------------------------------------------
```
For when Google Chrome is just too much 

alias chromekill='ps ux | grep '\''[C]hrome Helper --type=renderer'\'' | grep -v extension-process | tr -s '\'' '\'' | cut -d '\'' '\'' -f2 | xargs kill'
```
--------------------------------------------------------------------------------------
```
For when you just want to clear that trash can full of pictures from the 7th grade: 

alias emptytrash='sudo rm -rfv /Volumes/*/.Trashes; sudo rm -rfv ~/.Trash; sudo rm -rfv /private/var/log/asl/*.asl'
```
--------------------------------------------------------------------------------------
```
FOR THE GIT-HUNGRY FOLKS:

alias g='git'
alias ga='git add -i'
alias gai='git apply -v --index'
alias gav='git apply -v'
alias gba='git branch -a'
alias gc='git commit -v'
alias gca='git commit -av'
alias gcam='git commit -am'
alias gcm='git commit -m'
alias gd='git diff'
alias gds='git diff --staged'
alias gf='git flow feature'
alias gl='git pull --rebase'
alias glog='git log --decorate'
alias gp='git push'
alias gpa='git push && gfp'
alias grepcommit='git log --pretty=oneline | grep'
alias gslog='git log --decorate --pretty=oneline --abbrev-commit'
alias gst='git status'
alias gundo='git reset --soft HEAD^'
```
--------------------------------------------------------------------------------------
```
Those damn hidden files and apple settings (MAC only)

alias hide='defaults write com.apple.finder AppleShowAllFiles -bool false && killall Finder'
alias hidedesktop='defaults write com.apple.finder CreateDesktop -bool false && killall Finder'
```
--------------------------------------------------------------------------------------
```
How can we forget? Editors are our lives.

alias v='vim'

This one isn't an alias, but sublime is so bae
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/sublime

```
--------------------------------------------------------------------------------------

