# jupyter-milestones
Used for coordinating work on Jupyter Notebook

## setting remotes
```
git remote --v
origin	https://github.com/nyu-ossd-s18/notebook.git (fetch)
origin	git@github.com:nyu-ossd-s18/notebook.git (push)
upstream	https://github.com/jupyter/notebook.git (fetch)
upstream	git@github.com:jupyter/notebook.git (push)
```

if your `origin` is not as above, do and run `git remote --v` again:
```
git remote set-url origin https://github.com/nyu-ossd-s18/notebook.git
git pull
```

## working on issues
the person creating the branch to fix the issue:
```
git checkout -b [branch-name]
git add .
git commit -m [commit-message]
git push
```
everyone else:
```
git pull
git checkout [branch-name]
```
## syncing our fork with the OG notebook
https://help.github.com/articles/syncing-a-fork/
```
# make sure upstream is set to https://github.com/jupyter/notebook.git
git fetch upstream
git checkout master
git merge upstream/master
git push
```
