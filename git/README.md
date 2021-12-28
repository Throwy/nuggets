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
    lg = log --pretty=format:\"%C(magenta)%H%Creset%C(red)%d%Creset - %C(yellow)%ad%Creset - %C(green)[%an]%Creset\n\t%s\" --abbrev-commit -20
```
