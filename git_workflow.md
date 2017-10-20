# Git Workflow

A short guide on how to use Git for group projects, including syntax for merges and branch deletions.

### Adding repository

- remember to do initialization first: `git init`
- following which just clone the repo: `git clone repo-name`

### When pushing up local branch to its remote branch

- make sure you're in the branch you want to push (i.e. not master), and that you've added and committed the latest changes locally, then just go: `git push`
- if this is your first time pushing, and this branch doesn't exist remotely yet, do this instead: `git push -u origin branch-name`

### Taking care of merges

- if want to merge remote branch to master, submit a pull request on Github

### Adding gitignore file

- multiple gitignore files are possible, though not recommended
- if files supposed to be in gitignore are already placed in, remove them as such: `git rm -r --cached .`
  - remember to commit new files first before this move
  - to remove files of a certain extension (forever), use the following command: `find . -name "*.extension_type" -type f -delete`

### Deleting branches

- can be done easily on Github
- on locally, do as follows: `git branch -d branch-name`

### Merge changes in master to feature branch
- do `git merge`
- in the subsequent (kind of disgusting) screen, calmly type `:quit`. Merge will be smoothly made if no conflicts

### Adding changes
- there's always the short and simple `git add -A` to add all your changes
- but there's also `git add -p` that allows you to view the changes one-by-one in terminal, and giving you the option to accept or decline the change. can prevent too many trivial commits to fix earlier over-adding issues