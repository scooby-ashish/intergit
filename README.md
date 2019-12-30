Git Commands
-------------

```markdown
git init
git add
git commit -m
git status
git log --oneline
added .gitignore
added .gitkeep
git clean -n #shows file in untracked staged trying to remove but not remove completely
git clean -f #will remove file from untracked stage and delete it from repo
git clean -fd #remove folders
git clean -i #provides option
git reset HEAD filename
git checkout -- filename
git config --global user.name 'NAME'
git config --global user.email 'mail@*.com'
git config --global --list
git reset HEAD filename #take staged file to untracked area
git branch branchName
git checkout -b branchName #also create and switched to named branch
git log --oneline --all #all branch logs were deprecated
git mv filename newname
git commit --amend #to change commit
git remote add origin URL
git remote -V
git push origin --all
git merge branchname
git merge branchname hashID
git hash-object filename #hash algorithm SHA-1 short digest
git stash save 'message'
git stash apply stashvalue
git stash pop topone
git stash drop stashvalue
git stash list
git stash clear
git rebase ??
The commit hash is using SHA-1 algorithm of 128 bit
```

