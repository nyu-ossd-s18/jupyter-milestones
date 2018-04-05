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
git fetch
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
git fetch
git checkout [branch-name]
```
