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

