# ACM VIT GenTech Git and GitHub Session

## Basic Git Commands

* ###    Initialization

This command is used to initialize an empty repository.

```git init <repository name>```

* ###    Configuration

This command sets the name and email address of the author of the commit. The `--global` flag is optional

```git config ––global user.name “<name>”```

``` git config ––global user.email “<email address>”```

* ###    Staging

This command adds a file to the staging area.

```git add <file>```

This command adds one or more files to the staging area.

```git add *```

This command adds all files in the working directory to the staging area.

```git add .```

* ###    Removing a File

This command deletes a specified file and stages its deletion, but doesn't remove it from the working directory. 

```git rm --cached <file>```

* ###    Committing

This command saves (or snapshots) the file permanently to the version history of the repository.

```git commit -m “<commit message>”```

This command works similarly to first doing `git add` on all modified and deleted files and then `git commit` for those files.

```git commit -a -m “<commit message>”```

* ###    Resetting

This command unstages the file, but it preserves the file contents. 

```git reset <file>```

This command reverts all the commits after the specified commit. But, the locally made changes are preserved. 

```git reset <commit>```

This command reverts to the specified commit. The locally made changes are __not preserved__ and are discarded.

```git reset –hard <commit>```

* ###    Branching

This command creates a branch. Branching allows developing software based on the main line without modifying it. It is essentially a new/separate version of the main repository.

```git branch <branch name>```

This command switches to the specified branch.

```git checkout <branch name>```

This command combines the above two.

```git checkout -b <new branch>```

* ### Merging

This command incorporates changes from the named commits (since the time their histories diverged from the current branch) into the current branch. It automatically creates a new commit for the merged histories.

```git merge <branch name>```

* ###    Checking Status

This command lists the current status of the repository. It can include files to be added, committed or pushed to the remote repository.

```git status```

* ###    Checking Logs

This command is used to check the commit history in a git repository.

```git log```

* ###    Diff (tool)

This command shows the differences between staged and unstaged versions of the file.

```git diff <file>```

This command shows the differences between the files in the staging area and the latest version present.

```git diff –staged```

This command shows the differences between two specified branches.

```git diff <first branch> <second branch>```

* ###    Remote repository

* ####    Setting-up Upstream

This command is used to add the remote repository as the upstream source of the local repository.

```git remote add origin <remote repository URL>```

* ####    Sync __To__ Upstream

This command syncs the changes made on a specified branch to the specified remote repository.

```git push -u <remote> <branch>```

In case of issues with authorisation, use the following command(s) or HTTPS upload rather than SSH

```git config --local credential.helper ""```
SSH: ```git remote set-url <remote> git@github.com:<username>/<repo>.git```
HTTPS: ```git remote set-url <remote> https://<username>@github.com/<username>/<repository name>.git```

* ####    Sync __From__ Upstream

This command will sync everything from the remote repository to the local repository.

``` git pull -u <remote> <branch>```

* ####    Cloning a Repository

This command is used to duplicate an existing repository.

```git clone <repository URL>```

## Tutorial
  Link : //does not exist

