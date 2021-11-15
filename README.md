# nuggets
Any helpful tidbit of information that I want to be able to find later.

## Git

### branches
delete a branch remotely and locally
```
git push -d <remote_name> <branchname>
git branch -d <branchname>
```


### aliases
set these in your global `.gitconfig` file
```
[alias]
  s = status
  sb = status -sb
  cm = commit -m
  co = checkout
  cob = checkout -b
  br = branch --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) %(color:green)(%(committerdate:relative)) [%(authorname)]' --sort=-committerdate
  lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(dim green)(%cr) [%an]\" --abbrev-commit -20
  f = fetch -p
```

## bash

make `ls` more colorful
```
alias ls='ls --color=auto'
```

make `Tab` cycle through options and `Shift + Tab` cycle backwards
```
bind 'TAB:menu-complete'
bind '"\e[Z":menu-complete-backward'
```
