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
```
