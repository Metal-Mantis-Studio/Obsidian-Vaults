---
tags: Source-Control, Git, CLI
---
The foundation of [[GitHub]]
## Git Basics
#git-log
```SH
git log
git stash
git checkout <SHA1>
git branch
```

#git-merge
```SH
#condenses the entire branch into a single commit and merges
git merge --squash 

#used to merge a branch new branch into another
git merge --allow-unrelated-histories 
```

#git-rebase
```SH
#rewrites commit history by applying changes from one branch to another
git rebase
```

#git-tag
Create a tag called "v3.0" with the commit message "Release v3.0"
```SH
git tag -a v3.0 -m "Release v3.0" 
```

#git-gc
```SH
#combines garbage collection with resetting outdated reflogs in the repository
git gc --prune=reset

git gc --aggressive now
```

#git-prune
```sh
git prune --expire now
```

#git-restore
```sh
#reverts the repository to a specific commit, discarding changes after that commit
git restore <SHA1>
```

#git-diff
```sh
#gets the difference from 1.4.16 to 1.6.12 and pipes it through the helper and outputs it to a changes.txt file
get diff v1.4.16 v1.6.12 | helper-script > changes.txt
```


