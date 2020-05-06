# Git Essentials

Summary of [git - the simple guide](https://rogerdudler.github.io/git-guide/index.html).

## Workflow

Repository consists of three "trees"
  - Working Directory (actual files)
  - Index (Stage)
  - HEAD (Last commit)
  
Working Directory &ndash;`add`&rarr; Index &ndash;`commit`&rarr; HEAD

## Commands

Repository
```sh
# create repo
git init
```

Workflow

```sh
# add to Index
git add * OR <filename>

# commit to HEAD
git commit -m "Message"

# remove last commit (locally)
git reset --hard HEAD^

# revert last commit
git revert HEAD
```

Branches

```sh
# create and checkout branch
git checkout -b feat/xy

# delete branch
git branch -d feat/xy

# push branch to remote repo
git push origin feat/xy
```

Tagging

```sh
# tag commit
git tag 1.0.0 1b2e1d63ff # first 10 characters of the commit id
```
