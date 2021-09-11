# Revisions and the cloud with git

Git is an important tool in modern coding. It automates something called version control, which saves and organizes all previous versions of a project into one place. This is useful for reverting to past changes, finding out what went wrong with a new change, and allowing multiple people to easily collaborate on a single project. 
GitHub is way of saving git repositories in the cloud, so that they may be worked on by multiple people simutaneously and remotely, and also adding redundancy to the code's storage so that in case of a local hardware failure it is still safe.

## Branches in git

The chains of past versions that git creates are called 'branches'. The most recent and up to date version is called the "head". New branches can be split off from the head, or previous branches. 

## The ACP process
ACP is an essential process in working with git. It stands for "Add, Commit, Push". First, you work on a piece of code, making changes, additions, or deletions to it. Then, you **add** that file so that github knows you'd like to save it to the version control system; the file is now considered tracked. Next, you **commit** those changes, which is a process sort of like saving, and the local branch of your code is updated with those changes, and the version control process is taken care of automatically, saving the past and current version of your code. After that, you **push** the changes, uploading those changes onto the copy of your code saved on GitHub.

## Important git commands 
There are a number of commands which are essential for working with github.

* git clone \[repository link\]: this command will download a repository (group of files) from github onto your computer, and automatically set them up for git. This process only needs to be done once; after that, all control of your code will be completed with the other commands.
* git status: this command shows the current status of the git repository you are working it. It will let you know which files have been changed, and whether they need to be added, committed, or pushed.
* git add \[file\]: after editing a file, this command is used to inform git that you'd like to include it in the next commit.
* git add .: this command does the same as above, but selects all files at once so you don't have to add them individually.
* git commit -m "message": this command commits the files which have been added (saves them and automates the version controll process) **locally**. Including a brief message summarizing the changes is essential because it will make digging through past versions much easier, and informs other developers working on the code with you what changes you have made. Files should not be committed without adding a message.
* git push origin main: this command pushes the files to GitHub, uploading your changes and making the online branch up to date with your local branch. 
* git help \[command\]: this will give you documentation on how to use a command, or if you don't include a command, it will give you a list of possible commands. 
* git init: this will begin the process of creating a git repository in your current working directory. It should be followed by `git add *.c`, `git add LICENSE`, and then `git commit -m "message"` to create the first working commit. 