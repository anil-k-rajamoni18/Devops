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

[![N|Solid](data:image/png;base64,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)](httpshttps://github.com/)
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








Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.

Install the dependencies and devDependencies and start the server.


cd dillinger
npm i
node app
```

For production environments...

```sh
npm install --production
NODE_ENV=production node app
```

## Plugins

Dillinger is currently extended with the following plugins.
Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:

```sh
node app
```

Second Tab:

```sh
gulp watch
```

(optional) Third:

```sh
karma test
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```

## License

MIT

**Anil K Rajamoni!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
