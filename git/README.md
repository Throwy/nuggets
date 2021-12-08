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
    f = fetch
    b = branch
    br = branch --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) %(color:green)(%(committerdate:relative)) [%(authorname)]' --sort=-committerdate
    lg = !git log --pretty=format:\"%C(magenta)%H%Creset - %C(yellow)%ad%Creset - %C(green)(%cr) [%an]%Creset\n\t%C(red)%d%Creset %s\" --abbrev-commit -20
```
