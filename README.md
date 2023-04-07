# GitRelated

![image](https://user-images.githubusercontent.com/61017530/204445074-7bc97a94-9dd9-418d-b405-05e53070f2db.png)


## 1. git init

It creates a new Git repository. It can be used to convert an existing, unversioned project to a Git repository or initialize a new, empty repository. 


## 2. git pull/clone

clone: copying the remote server repository to your local machine. 
pull: get new changes other have added to your local machine.

pull = clone + merge。


## 3. git remote 

3.1 git remote add origin https://.....git

Add a new remote repository.

origin:：remote repository name, by default is origin and can be user-defined.

https://.....git:：remote repository URL.

3.2 git remote update origin

Update remote repository information.


## 4. git branch -r

git branch -D: delete a branch.


## 5. git checkout -b local_branch_name origin/remote_branch_name

local_branch_name：local branch name.

remote_branch_name：remote branch name.

origin: the same name when you use the "git remote add".


## 6. git stash

Use git stash when you want to record the current state of the working directory and the index, but want to go back to a clean working directory.

\# before checkout

git add .

git stash

\# after checkout

git stash pop



## 7. git status/diff highlight

git config --global color.status auto

git config --global color.diff auto 


## 8. git cancel add

git reset file_name


## 9. git lfs

git lfs install：initialize git lfs.
git lfs track：track files.
git lfs ls-files：list all tracked files.
git lfs pull --include "a.dat"：only download certain lfs file.


## 10. git reflog

git reflog will output the reflog of the HEAD ref

git reflog --date=iso: list with time.


## 11. git reset 

git reset is a powerful command that is used to undo local changes to the state of a Git repo.

git reset --hard b8cc0e3


## 12. git push

The git push command is used to upload local repository content to a remote repository.

git push origin local_branch_name:remote_branch_name

git push -f: force push
git push origin --force: force push

## 13. git merge 

The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.

git merge branch_name
git merge --squash branch_name: squash all commits in branch_name to one commit.


## 14. git rebase 

It changes the base of the developer's branch from one commit to another.

git rebase -i commit_hash


## 15. 
