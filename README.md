
Bash Commands
-------------


## ls - listing 
```markdown
[root@lab demo]# ls
Apple  Banana  Cat  Dog  Eagle
```

## ll - long listing
```markdown
[root@lab demo]# ll
total 20
drwxr-xr-x. 2 root root 4096 Dec 28 11:15 Apple
drwxr-xr-x. 2 root root 4096 Dec 28 11:15 Banana
drwxr-xr-x. 2 root root 4096 Dec 28 11:15 Cat
drwxr-xr-x. 2 root root 4096 Dec 28 11:15 Dog
drwxr-xr-x. 2 root root 4096 Dec 28 11:15 Eagle
```

## la - longlisting with all hidden files
```markdown
[root@lab demo]# ll -la
total 32
drwxr-xr-x.  7 root root 4096 Dec 28 11:18 .
dr-xr-x---+ 37 root root 4096 Dec 28 11:14 ..
drwxr-xr-x.  2 root root 4096 Dec 28 11:15 Apple
drwxr-xr-x.  2 root root 4096 Dec 28 11:15 Banana
drwxr-xr-x.  2 root root 4096 Dec 28 11:15 Cat
drwxr-xr-x.  2 root root 4096 Dec 28 11:15 Dog
drwxr-xr-x.  2 root root 4096 Dec 28 11:15 Eagle
-rw-r--r--.  1 root root    0 Dec 28 11:18 .hiddenfilewithDOT
```

## cd - change directory
```markdown
[root@lab demo]# cd Apple
[root@lab Apple]# 
[root@lab Apple]# cd ../Banana
[root@lab Banana]# cd ../Cat/
```

## pwd - present working directory
```markdown
[root@lab demo]# cd Apple/
[root@lab Apple]# pwd
/root/demo/Apple
[root@lab Apple]# cd ../Banana/
[root@lab Banana]# pwd
/root/demo/Banana
```

## mkdir - make directory
```markdown
[root@lab demo]# mkdir {Apple,Banana,Cat,Dog,Eagle}
```

## touch - create blanked file
```markdown
[root@lab demo]# cd Apple/
[root@lab Apple]# touch Juice
[root@lab Apple]# ls
Juice
[root@lab Apple]# 
```

## rm - remove
```markdown
[root@lab Apple]# ls
Juice  Shake
[root@lab Apple]# rm Juice 
rm: remove regular empty file 'Juice'? y
[root@lab Apple]# rm -rf Shake 
[root@lab Apple]# ls
[root@lab Apple]# 
```

## mv - move
```markdown
[root@lab demo]# ls
anaar  Apple  Banana  Cat  Dog  Eagle
[root@lab demo]# mv anaar Apple/
[root@lab demo]# ls
Apple  Banana  Cat  Dog  Eagle
[root@lab demo]# ls
Apple  Banana  Cat  Dog  Eagle  pencil
[root@lab demo]# mv pencil pen
[root@lab demo]# ls
Apple  Banana  Cat  Dog  Eagle  pen
```

## tree - directory hirarchy
```markdown
[root@lab demo]# tree
.
├── Apple
│   └── anaar
├── Banana
├── Cat
├── Dog
├── Eagle
└── pen
```

## cat - concatenation
```markdown
[root@lab demo]# cat > file
Hey im ashish for saving this file i'll say ENTER then CTRL+d
[root@lab demo]# cat >> file 
With single > will overwrite, but
with >> double append in file
[root@lab demo]# cat file
Hey im ashish for saving this file i'll say ENTER then CTRL+d
With single > will overwrite, but
with >> double append in file
```

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
