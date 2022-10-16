[Return to maine page](../readme.md)

# Initalize git in current folder

```git
    git init
```

# Add repository to current folder

```git
    git remote add origin repository-location
```

# Check unsaved file in git

```git
    git status
```

# Add file using git

```git
    git add filename or
    git add .
```

# Commit your files

```git
    git commit -m'enter your message'
```

# Push on github repository

```git
    git push origin master
```

# Remove file from git and directory

```git
 git rm 'file name'
 git commit
 git push origin 'name'
```

## Remove only from git

```git
git rm --cached 'file name'
git commit
git push origin 'name'
```

# Not able to push due to ref erro

```git
git show-ref
git push origin HEAD:master
```

# Remove recent commit

```git
git reset --soft HEAD~1
```

# Remove recent commit with work

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

# Revert in git

```git
    git revert sha-key
```

# Check repository

```git
    git config --get remote.origin.url
```
