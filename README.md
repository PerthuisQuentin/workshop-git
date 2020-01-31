# workshop-git

Little project used as a support for a git workshop

## #1 - Cloning the repo

```
git clone https://github.com/PerthuisQuentin/workshop-git.git
cd workshop-git
```

`git clone` will clone the repository into a newly created directory, with the name of the repo.
Also, it creates a remote "origin". Remotes are like aliases to track remotes repositories.

You can see the remotes with :
```
git remote -v
```
After cloning, it must output :
```
origin  https://github.com/PerthuisQuentin/workshop-git.git (fetch)
origin  https://github.com/PerthuisQuentin/workshop-git.git (push)
```

## #2 - Master is sacred

By default, we are on a branch called "master".

We never work on master, to keep it safe from mistakes (like erasing everything 😐).

So, to start doing something, we create an another branch :
```
git checkout -b new-work
```
It creates a new branch named "new-work" and move us onto it.

We can see the branches and where we are with :
```
git branch
```
It outputs :
```
  master
* new-work
```
Our current branch has a * n front of her name

Branches are aliases to a precise commit, we can see them with :
```
git branch -v
```
It outputs :
```
  master   442bb93 Initial commit
* new-work 442bb93 Initial commit
```
We did nothing on "new-work", so it's same commit that the branch from which we come : "master".