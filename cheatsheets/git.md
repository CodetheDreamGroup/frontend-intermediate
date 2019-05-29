- [Getting Git](#getting-git)
  - [Installing Git command line](#installing-git-command-line)
  - [Git GUI clients](#git-gui-clients)
  - [Official Documentation](#official-documentation)
- [Configuring Git](#configuring-git)
  - [Configure user name](#configure-user-name)
- [Creating/getting a repository locally](#creatinggetting-a-repository-locally)
  - [New local repository without existing code](#new-local-repository-without-existing-code)
  - [Cloning an existing repository](#cloning-an-existing-repository)
  - [Adding files to staging for committing](#adding-files-to-staging-for-committing)
  - [Commiting staged files](#commiting-staged-files)
  - [Undoing all changes](#undoing-all-changes)

## Getting Git

### Installing Git command line
If you are in Cloud 9 the git command line is already installed and can be accessed through the terminal window.

If you are on a Windows computer and working locally you can download the Git for Windows installer [here](https://git-scm.com/download/win).

If you are on a Mac you can download Git for Mac [here](https://git-scm.com/download/mac).

If you are on a Linux system there is a good chance that git is already installed, otherwise you will need to search for how to install it on the distribution of Linux that you are using.

### Git GUI clients

GitHub provides desktop clients that include a graphical user interface for the most common repository actions and an automatically updating command line edition of Git for advanced scenarios.

This client can't be installed in Cloud 9, but if you are working locally it can be installed and used for any Git work even if you are not using GitHub.

https://desktop.github.com/

### Official Documentation
The official documentation for Git can be found on the official http://git-scm.com site. It includes a book on how to use Git as well as a reference guide.


## Configuring Git
When you first use Git you will want to configure it with your information so that the commits you make have your details included. 

There are a lot of great configuration options for Git, but the two important ones to configure before using it are your user name and your email address.

Usually you can configure these settings globally on a computer that is only used by you, so that is what we will show.

### Configure user name

To configure your user name locally run the following command replacing [name] with your desired username:

```$ git config --global user.name "[name]"```

### Configure email address

To configure your email address locally run the following command replacing [email] with your desired username:

```$ git config --global user.email "[email]"```

## Creating/getting a repository locally
There are 3 typical ways to get a Git repository.

* You might be creating a new project, in which case you will usually create the folder and repository with a single command
* You might be creating a repository for existing files
* You want to clone a repository that already exists

### New local repository without existing code
If there is not already a folder containing code that you want to add to a Git repository then the easiest way to create a new Git repository and the corresponding folder is with the following command where [name] is replaced with the name of the project/folder you want to create:

```$ git init [name]```

This creates a new repository and folder with the specified name.

### Creating a new repository with existing code
To create a new Git repository for existing code you will want to be in the top level folder of the project. 

For example, if you have a folder of 'javascript-homework' that you want to make into a Git repository, first get in to that folder on the command line.

Then run the following command:

```$ git init```

This will create a Git repository within the current folder. You can then add all of the existing code the repository following the standard workflow.

### Cloning an existing repository
If there is an existing repository that you want to clone you will need to get the url for that repository. Once you have the url you can run the following command to clone that repository into a folder with the same name as the repository.

```$ git clone [url]```

When you run this command you will get the entire history of that repository copied to your system.


## Working in a repository
One of the important things to remember when working in a Git repository is that files can be in any of 3 states, which are:

* untracked - This means that the changes to the file are not yet committed to git and could be lost still
* staged - This is the state that you put files/changes in that you want to commit to Git. These changes could also still be lost
* committed - Once committed the changes to the file can always be retrieved as long as you don't delete the entire Git repository

This workflow is one of the most common challenges that people who are new to Git encounter because it is different than a normal workflow where you simply save changes as a single action.

### Checking the status of files
To check the status of the files in your repository to see if the latest changes to them are untracked, staged, or committed (you will not see anything for committed files) run:

```$ git status```

This should show you any untracked files, although if an entire folder is untracked you will not see the individual files within that folder listed, as well as any staged files.

### Adding files to staging for committing
To add untracked files to the staging area to be committed you use the `git add` command. 

You can add individual files to the staging area, if you don't want to commit all of your files with a single commit, or all of them at once. 

To add individual files to the staging area run:

```$ git add [filename]```

To add all of the untracked files to the staging area run:

```$ git add .```

### Commiting staged files
To commit the files that are in the staging are you can run:

```$ git commit -m "your commit message"```

I recommend running `git status` again after committing changes to make sure that the files are no longer listed as untracked or staged.

## Undoing things in git

### Undo all changes to a file since last commit
To return a single file back to the state after the last commit run:

```$ git checkout [filename]```


### Undoing all changes

Reverts **all** changes to the last commit

```$ git reset --hard```


### Removing a tracked file
To remove a tracked file from Git but not from the local file system run:

```
git rm --cached <filename>
```

This might be needed if there are some files that you didn't intend to add to be tracked by Git, such as the node_modules folder

