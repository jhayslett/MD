###Mastering Git, Part 1 Notes 
#####Written by jhayslett  
#####Last Updated: 01/19/2016  
___  
####New Terms
- VCS - Version Control System
  - Centralized VCS
    - single server acts as the primary repository for all files
    - adv - large teams, control over file access, saves disk space on local machines
    - dis - centralized architecture failure, if power is out dev can't access files, difficult if dev are remote
  - Distributed VCS
    - peer-to-peer, no central server, devs copy whole directory and history of project to their local machine

####Commands
- git --version \\ identify if you have Git installed
- git config --global user.name "Jacob Hayslett" \\ set user.name global variable
- ~/.gitconfig \\ read the root file git config file
- git config --global core.editory "pico" \\ set core editor to pico
- git init \\ create a new repository
- git add -A \\ add all files in staging area
- git commit -m "My very first commit" \\ submit a commit message with the commit.
- git clone https://github.com/jashkenas/underscore.git my_directory \\ clone a repository from a remote location, my_directory is option but will save the directory as that name
- git remote add origin git@github.com:myname/my_project.gitv \\ set remote origin for repository
- git remote -v \\ list all remotes for repository


####Notes  
- Git is a modern, distributed VCS. Almost everything happens locally  
- Git has 3 stages  
  - Working Directory - 'git add' to put in staging area  
  - Staging Area - 'git commit' to put back in repository  
  - Repository - git 'checkout' to pull out to work with  
- Git Version 2.5.4 (Apple Git-61)  
- **Exercise Notes** -  
  - 2. git config --global core.editor "pico" - this set core.editor to pico for global scope  
    - to make this previous statement permanent for my default I would need to edit the .bashrc or .bash_profile config files  
  - **(insert manGitConfig.jpg)**
  - I found git config [\<filename\>] --get-color name [default], so I put in git config --get-color name blue and the terminal color turned blue.
- When writing, the new value is written to the repository local
  - configuration file by default, and options --system, --global, --file
  - <filename> can be used to tell the command to write to that location
  - (you can say --local but that is the default).
- **Workflow for Developers Working Along**
   1. Get a Git repository, either by initializing a new repository on your local machine or by cloning an existing one from a remote location.
  2. If the repository is new, set it up. This may include configuring Git to ignore unwanted files as well as adding the location of “remote” repositories that serve as backups or central locations for collaboration.
  3. Make changes, either by creating new files in the repository directory, deleting files in the directory, or changing existing files.
  4. Stage the changes you wish to commit to the repository.
  5. Commit the changes to the repository, along with a message describing the changes.
  6. Push the changes to any remote repositories.
  7. Repeat steps 3-7 as often as necessary.
- Use git init to create a new repository
- Create a .gitignore to list out all files you want to exclude from the repository, use wildcards and directories as normal
  - Example files include .DC_STORE macs, sass-cache temp css files etc
- Use git remote add - git remote add origin git@github.com:myname/my_project.git 
- Use git remote -v to list out all remote directories
-  **Exercise Notes** -
  - Cloned underscore.js
  - When inspecting the .gitignore I found the following list
    - raw
    - node_modules
    - *.log
    - *.idea
    - *.swp
    - nyc_output
    - coverage
- Make commits when you complete small, succint changes that may be readily summarized in a single commit message
- Use git status to check the state of files in your repository 
  - It will list out what is/isn't staged and commited or if no action is necesarry
  - It is useful to use this after you use git add to review the files that have been transferred from working to staging
- Use git reset HEAD to un-stage files, in a case where you are not ready to commit a file
- Use git commit to commit files in staging
- (**insert picture of process of creating a new text file, adding it, then commiting it**)
- After you commit there will be a success message that will have a string representing the commit reference number, next to branch name
- Use git checkout (reference number) to reset back to that commit \\ is this correct?
- Use git rev-parse HEAD to echo the hash string for the last commit
- Use git log to review the log of commits
- **Exercise Notes** -
