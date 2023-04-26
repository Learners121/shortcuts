[return to maine page](../readme.md)

# initalize git in current folder

```git
    git init
```

# add repository to current folder

```git
    git remote add origin repository-location
```

# check unsaved file in git

```git
    git status
```

# add file using git

```git
    git add filename or
    git add .
```

# commit your files

```git
    git commit -m'enter your message'
```

# push on github repository

```git
    git push origin master
```

# remove file from git and directory

```git
 git rm 'file name'
 git commit
 git push origin 'name'
```

## remove only from git

```git
git rm --cached 'file name'
git commit
git push origin 'name'
```

# not able to push due to ref error

```git
git show-ref
git push origin HEAD:master
```

# remove recent commit

```git
git reset --soft HEAD~1
```

# remove recent commit with work

```git
git reset --hard HEAD~1
```

# Remove origin

```git
git remote rm origin
```

# Download Specific Folder From Git using svn

```git
 svn checkout https://github.com/location/trunk/location

 remove master and use trunk instead of tree
```

# revert in git

```git
    git revert sha-key
```

# check repository

```git
    git config --get remote.origin.url
```
# merge current branch data into another branch
```git
    git merge [branch name]
```
# remove file from staging area
```git
    git restore --staged [filename]
```
# read only upper 10 lines of data from file
```git
    head [file name with extension]
```
# read only lower 10 lines of data from file
```git
    tail [file name with extension]
```
# read specific lines of data
```git
    head -n [number of lines data you want to read] filename with extension
```
# export one file data into another file
```git
    cat [filename with extension] > [new file name with extension]
```
# rebasing (alter commits) as moved to the new branch
```git
    git rebase -i [branch name]
```