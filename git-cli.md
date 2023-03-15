## Git Branch

``git branch`` list all branches

``git branch -a`` list all remote branches

``git branch [branch name]`` create a new branch.  ``git init -b master`` This will initialize a repo with branch name master

``git branch -d [branch name]`` safe delete a branch if a branch has unmerged changes

``git branch -D [branch name]`` force delete even if a branch has unmerged changes

``git push origin --delete [branch name]`` delete a remote branch

``git push origin :[branch name]`` push a delete signal to delete a remote branch

``git branch -m [new branch name]`` rename a current check out branch to new name


## Git Checkout

``git checkout [branch name]`` check out a given branch

``git checkout -b [branch name]`` create a new branch and checkout that branch

``git checkout -b [branch name] [existig branch]`` create a branch from existing branch. like create a feature1 branch from release/master

> git checkout -b feature1 release/master


## Git Push

``git push origin`` push the pending changes to remote

`` git push --set-upstream origin [branch name]`` use ***--set-upstream origin*** to push the new branch for the first time

## Git Fetch

``git fetch --all`` fetch remote branches

## Git Merge

it has 2 ways. fast forward and 3 way. Fast Forward is like, main => feature => main. So, for this first check out main branch and then merge it.

``git checkout main``

``git merge feature`` 

This will merge all ***feature*** branch changes to ***main*** branch.

``git merge --no-ff [feature branch]`` keeps the merge commit info 

## Git Log
``git log`` use to show the commit logs

``git log -n 3`` retun only last 3 commits

``git log --author='rathod'`` filter by author

``git log --committer="rathod"`` filter by committer

``git log --after="2022-01-01"`` filter by date after

``git log --before="2021-01-01"`` filter by date before

``git log --after="2019-3-2" --before="2019-3-19"`` before and after filter

``git log [file]`` log for a given file

``git log [file] -s "part"`` check for log in a specific file with word ***part***

## Git Stash
``git stash help`` stash help

``git stash list`` list all stashed change

``git stash`` stash pending changes

``git stash pop`` pop last changes (remove last change) and apply it in current branch

``git stash pop --index [index]`` pop last changes (remove last change) and apply it in current branch

``git stash apply --index [index]`` apply given indexed stash in current branch

``git stash clear`` clear stash queue

``git stash branch [branch name] [index]`` create a new branch from stash index


## References

[Git/Tutorials](https://www.atlassian.com/git/tutorials/using-branches)

[Git/Get-Started](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line)