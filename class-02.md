### Class 02 Reading Notes #


## Command Line Tutorial

https://ryanstutorials.net/linuxtutorial/navigation.php

GUI= Graphical User Interface

Terminal is NOT a GUI :D

You can have more than one Terminal open at a time. Ie:
	1 in which I am doing my work
	2 Bringing up ancillary data
	3 Viewing Manual pages

Command line: text based interface to the system

Linux file system is hierarchical
Root dir

Absolute Path- specify a location in relation to the root directory

 Relative Paths- specify a location in relation to where we currently are in the system


Linux is Case Sensitive- Beware of silly typos.

Everything is a file under Linux


## Terminal Commands
- cd *Change Directory*
- ls *list all the directories in the folder*
- touch *create a new file*
- clear *clears terminal*
- mkdir *makes folder/directory*
- ls -a *shows up hidden files*
- code . *opens code editor in the current folder*

 ## Terminal Commands


pwd = Print Working Directory (tells you what current directory is.
cd  = change directory

cd = 'Folder Name = will put you in that Folder
cd .. = moves you back to parent directory 
ls = list: will give you a list of what is in the folder

ls -l = Long Listing
ls /etc = List that directories contents
ls -l /etc = long listing of directory /etc 

~ Tilde= Shortcut for home directory
. = reference to your current directory
.. = reference to parent directory

mkdir projects = will create a folder called projects 

cd project = navigates you into the projects folder

git clone   " git hub url of you repository"

ls = so you can see that the repo folder is in the projects folder and was downloaded successfully

ls -a = List the contents of a directory, including hidden files. 
cd " name of repo" = you are now in the git repo and can begin adding to the project.

git status = will verify that you are on main branch

code . = will open the VS code text editor

Once in the editor you can add changes to your project.

git status = to verify that you are on master branch and up to date with origin(remote github master branch)
Add in your changes ACP

git add "fileName"     or git add .  = the period means all files

git commit -m ' add commit message here'

git push origin master

If you use git status between the A C P process you can see the file name change color from red to green and then see that the commit has put your local branch ahead of the remote master, so that you know you have changes locally that can be pushed to the online repo.

- = option (typically used to modify the behavior of the command.

Echo $SHELL: will tell you which shell you are using. (Bash is common..we are using zsh)

*Shortcut: The up and down arrow will toggle through commands you have already entered! 

File [path]  obtain information about what type of file a file or directory is. 

.before file name makes it hidden

Man [command] = explain the command
(Use “q” (quit) to exit the man






