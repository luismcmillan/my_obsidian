[[GIT/GIT]]
```Shell
git init #Initializes empty Git repository

git status #Look which changes are in the Staging Area

git add filename #Adds filename to Staging Area
git add . #Adds Everything to staging Area
git rm --cached -r . #removes all files from staging Area

git commit -m "Initial commit" # Do a commit, which puts all changes from Staging Area to repository
git reset --soft HEAD-1 #removes last commit
git commit --amend --no-edit #edits last commit without creating a new commit
git push --force luis

git branch #which branch?
git log #Which Commits were made ?
git diff filename # show current differences from filename to repository
git checkout #rollback to last version in our repository
```
![[GitHub and Remote Repositories]]
![[Gitignore]]
![[Git Cloning]]
![[Git Branching and Merging]]![[Git Forking and Pull Requests]]