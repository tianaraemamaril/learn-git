# Git

## Commands

### help

Will display all of the available commands for git and how to use it. `--help` also works for each specific command

```
git --help // will display all the git commands available
git clone --help // specific to clone command
```

### clone

Will download a repository to my local machine at the current path (where you are in the terminal).

```
git clone https://github.com/tianaraemamaril/learn-git.git
```

Cloned a copy of the git repository to the computer.

### status

Displays paths that have differences between the index file and the current HEAD commit.

Shows the difference between what I have in my local computer compared to what is in the repository.

#### untracked files

Files that currently exist in my local machine but not in the git repository. 

#### tracked files

Files that have already been commited and have been modified.

### add

1. Stages file / folder to be added to the repository.

```
git add README.md
```



### commit

Leaves a message attached to the files that are currently staged.

```
git commit -m "Notes under 50 characters"
```

Example of a good commit message

```
git commit -m "<verb> <scope>: <message>"
git commit -m "add readme: initial notes about git"
```

> YOU CAN'T LEAVE A COMMIT MESSAGE WITHOUT FIRST USING `GIT ADD`. ALL COMMIT MESSAGES ARE ATTACHED TO STAGED FILES.



For files that are already tracked (not new files), you can skip `git add`.

```
git commit -am "my notes about this commit message"
```

`-am` will add ALL the files that have been modified and will attach the commit message to all of them.

### push

Submits / uploads all the commited changes to the git repository. 



### log

Displays all the previous commits in my local machine along with their git hash. A git hash is an automatically generated unique "id" attached to each commit.

```
git log

commit b5909a77c344a4cbf012e2714b30a400ed17fea8 (HEAD -> master, origin/master)
Author: Tiana Mamaril <tianamamaril@Tianas-MacBook-Pro.local>
Date:   Sun Sep 23 16:33:48 2018 -0700

    update README.md: noted usage of git commit -am

commit 9560b4319537de9f41120faa92e6fec2ca4529ad
Author: Tiana Mamaril <tianamamaril@Tianas-MacBook-Pro.local>
Date:   Sun Sep 23 16:28:55 2018 -0700

    update README.md: noted commit and push commands

commit 6add78b0ec03319f113f2566d933854fca8913ee
Author: Tiana Mamaril <tianamamaril@Tianas-MacBook-Pro.local>
Date:   Sun Sep 23 16:19:23 2018 -0700

    added README.md
(END)
```



### diff

Shows the difference for all the files or a specific file / folder since the last commit where green (+) are lines added and where red (-) are lines deleted. 

If all the changes are too long to fit on one page, press space to scroll down.



### checkout 

Switches to an existing branch or creates a new branch with `-b` flag.

``` 
➜  learn-git git:(master) git checkout -b new-branch
M	README.md
Switched to a new branch 'new-branch'
➜  learn-git git:(new-branch) ✗ git checkout master
M	README.md
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
➜  learn-git git:(master) ✗ git checkout new-branch
M	README.md
Switched to branch 'new-branch'
```

