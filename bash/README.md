# bash

All of these go in your `.bashrc` file

### make `ls` more colorful
```
alias ls='ls --color=auto'
```

### make `Tab` cycle through options and `Shift + Tab` cycle backwards
```
bind 'TAB:menu-complete'
bind '"\e[Z":menu-complete-backward'
```