# git

## branches
delete a branch remotely and locally
```
git push -d <remote_name> <branchname>
git branch -d <branchname>
```


## config
set these in your global `.gitconfig` file
```
[pull]
    rebase = true
[fetch]
    prune = true
[alias]
    s = status
    sb = status -sb
    cm = commit -m
    co = checkout
    cob = checkout -b
    b = branch -a
    br = branch --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) %(color:green)(%(committerdate:relative)) [%(authorname)]' --sort=-committerdate
    lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(green)(%cr) [%an]\" --abbrev-commit -20
```
