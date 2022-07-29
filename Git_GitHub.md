## Version Control System 


[![N|Solid](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQmA6wKasZc0OmuftYXhbshTalfrLTwOfENBg&usqp=CAU)](https://www.geeksforgeeks.org/version-control-systems/)

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later. So ideally, we can place any file in the computer on version control.

We have two types

- Centralized Version Control System
            - SubVersion 
- Distributed Version Control System
            - **Git**
            - **Mercurial**

## Centralized Version Control Systems

Centralized version control systems contain just one repository globally and every user need to commit for reflecting one’s changes in the repository. It is possible for others to see your changes by updating. 

Two things are required to make your changes visible to others which are:  

- You commit
- They update

[![N|Solid](https://media.geeksforgeeks.org/wp-content/uploads/20190624140224/cvcss.png)](https://www.geeksforgeeks.org/version-control-systems/)


## Distributed Version Control Systems

Distributed version control systems contain multiple repositories. 

- Each user has their own repository and working copy. Just committing your changes will not give others access to your changes. 
- This is because commit will reflect those changes in your local repository and you need to push them in order to make them visible on the central repository. 
- Similarly, When you update, you do not get others’ changes unless you have first pulled those changes into your repository. 

To make your changes visible to others, 4 things are required:  

- You commit
- You push
- They pull
- They update

[![N|Solid](https://media.geeksforgeeks.org/wp-content/uploads/20190624140226/distvcs.png)](https://www.geeksforgeeks.org/version-control-systems/)


 # What is Git?
 
 > Git is a distributed version control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows. 

Git is a popular version control system. It was created by Linus Torvalds in 2005, and has been maintained by Junio Hamano since then.

> Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people. 

- Git is a Distributed Version Control System. So Git does not necessarily rely on a central server to store all the versions of a project’s files. 
- Instead, every user “clones” a copy of a repository (a collection of files) and has the full history of the project on their own hard drive. 
- This clone has all of the metadata of the original while the original itself is stored on a self-hosted server or a third-party hosting service like GitHub.


######  USES 

```diff
- Tracking code changes
+ Tracking who made changes
+ Coding collaboration
- Code Histroy for your Projects

```

##### What does Git do?
- Manage projects with Repositories
- Clone a project to work on a local copy
- Control and track changes with Staging and Committing
- Branch and Merge to allow for work on different parts and versions of a project
- Pull the latest version of the project to a local copy
- Push local updates to the main project



## What is GitHub?

 > GitHub is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features.
 
 ```diff
- Git Hub is implementation or specification for git tool
+ It will store all remote repositories
- Manages different projects 
+ Provides features
    - like branching & Pull Request creation
    - delete the branchs & repos
    - view the commit history 
    - resolve merge conflicts 
    - integration with other CI/CD tools.
```



## Installation

 - Install the git from 
 https://git-scm.com/download/win
  
    Verify by typing 
    ```
    git --version
    ```
     Open any floder in File Explore , right click you should be able to see git bash , git gui options

- Create a new Github Account 
          https://github.com/



##### What is Git Repository ?

> A repository a.k.a. repo is nothing but a collection of source code.
> Think of it as a floder in remote server 

### Workflow
There are four fundamental elements in the Git Workflow.

- Working Directory,
- Staging Area,
- Local Repository,
- Remote Repository.

![N|Solid](https://miro.medium.com/max/1400/1*iL2J8k4ygQlg3xriKGimbQ.png)

## Commands 
##### 1 .`git config `
This command sets the author name and email address respectively to be used with
your commits.

Basically introducing yourself to the GIT , it's only firsttime 


```
 Usage: git config –global user.name “[name]”
 
 Usage: git config –global user.email “[email address]”
```


##### 2. `git init`
Stands for  git initialization , used to start a new repository.

```
Usage: git init [repository name]

Usage: git init . 
```

##### 3. `git clone`

This command is used to obtain a repository from an existing URL
It Creates a local repository from remote repository URL 
Basicallly setting a up a local clone copy 

```
Usage: git clone [url
 
```


##### 4. `git add`
To add files to the Staging Area
This Command will add one or more files to the Unstaging - > Staging 

```
Usage: git add *

Usage: git add -A

Usage: git add [filename1] [filename2] ...[filenamen]
```
- A , *  -> will add all modified/changed files in WORKDIR

##### 5. `git status`

This Command will give the status of every stage during the workflow
- unstagged files will have RED color 
- stagged files will have GREEN color

NOTE: better to check status before doing git pull command everytime.
```
Usage: git status
```

##### 6. `git commit`

This command records or snapshots the file permanently in the version history.
It creates a commit id for tracking 
It helps other developers to know what changes have made in the REPO.

```
git commit -m “[ Type in the commit message]”

Usage: git commit -a

```
***git commit - a***
 - This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then.

##### 7. `git diff`
This command shows the file differences which are not yet staged.
```
Usage: git diff  
```
This command shows the differences between the files in the staging area and the latest version present.

```
 Usage: git diff –-staged 
```

This command shows the differences between the two branches mentioned.

```
Usage: git diff [first branch] [second branch]  
```

##### 8. ``git remote``

This command is used to connect your local repository to the remote server.

```
Usage: git remote add [variable name] [Remote Server Link]  
```

This command will show the REMOTE REPO URL to which it is pushing & pulling 

```
Usage :git remote  -v
```


##### 9. ``git push``

This command sends the committed changes of master branch/specific to your remote repository.

```
git push [variable name] [master]

git push [variable name] [branch]  

git push –-all [variable name]  
This command pushes all branches to your remote repository

Usage: git push [variable name] :[branch name]
This command deletes a branch on your remote repository.


```

##### 10. `git pull`

This command fetches and merges changes on the remote server to your working directory.

This command is commbination of git fetch + git merge 

**git fetch** : fetch the changes from remote REPO -> LOCAL REPO

**git mereg** : merge the changes from LOCAL REPO -> WORKDIR

```
Usage: git pull [Repository Link]
```

##### 11. `git merge`

This command merges the specified branch’s history into the current branch.
It will merge all changes from specified branch

```
Usage: git merge [branch name]  
```
##### 12. `git checkout`

This command is used to switch from one branch to another.
Will allow to work on different LOCAL REPOSITORY branches

```
Usage: git checkout [branch name]
```


This command creates a new branch and also switches to it.
```
Usage: git checkout -b [branch name]  
```


##### 13. `git branch` 
This command lists all the local branches in the current repository.

This command creates a new branch.

```
Usage: git branch [branch name]  
```

This command deletes the feature branch.

```
Usage: git branch -d [branch name]  
```

##### 14. `git tag`

This command is used to give tags to the specified commit
```
Usage: git tag [commitID]  
```

##### 15. ``git show``

This command shows the metadata and content changes of the specified commit.

```
Usage: git show [commitID]  
```

##### 16. `git rm`

This command deletes the file from your working directory and stages the deletion.

```
Usage: git rm [file] 
```

##### 17. `git log`

This command is used to list the version history for the current branch.

```
Usage: git log  
```
This command lists version history for a file, including the renaming of files also.

```
Usage: git log –-follow [filename]  
```

##### 18. `git  stash`

This command temporarily stores all the modified tracked files.

```
Usage: git stash save
```
This command restores the most recently stashed files.

```
Usage: git stash pop
```

This command lists all stashed changesets.

```
Usage: git stash list

```

This command discards the most recently stashed changeset.

```
Usage: git stash drop
```


##### 18. `git  reset`
This command unstages the file, but it preserves the file contents.

```
Usage: git reset [file]  
```
This command undoes all the commits after the specified commit and preserves the changes locally.

```
Usage: git reset [commit] 
```

This command discards all history and goes back to the specified commit.

```
Usage: git reset –hard [commit]
```



## License

MIT

**Anil K Rajamoni!**

