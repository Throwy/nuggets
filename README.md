# nuggets
Any helpful tidbit of information that I want to be able to find later.

## Git
aliases
```
[alias]
  s = status
  co = checkout
  cob = checkout -b
  lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(dim green)(%cr) [%an]\" --abbrev-commit -30
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
