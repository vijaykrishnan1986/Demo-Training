# Demo Git Repository

This is the first line in this repo.

## Git Learnings
Learn the key concepts of the Git source control system
Step through the entire basic Git workflow
Configure SSH for authentication
Create and use a remote repository on GitHub

## git commands
1. git version
2. git help
   git help -a
   git help -g

3. pwd (present working directory)

4. git configuration
git config --global user.name "Vijay Krishnan"
git config --global user.email "vijaykrishnan27@gmail.com"

git config --global --list (It will display the list of current global configuration settings)
user.name=Vijay Krishnan
user.email=vijaykrishnan27@gmail.com
init.defaultbranch=master


It created the simple text file within user directory i.e .gitconfig

cat ~/.gitconfig
[user]
        name = Vijay Krishnan
        email = vijaykrishnan27@gmail.com
[init]
        defaultBranch = master

5. Creating project from scratch

i. Know your current directory <pwd>
ii. Navigate to the folder where you will create git project
cd <path to the directory>

iii. git init git-demo
It will create sub-folder named <git-demo> after the projects folder

iv. ls (list the folder names)

v. cd git-demo
Now we are in working folder of git repository

vi. ls -a
It will show .git directory
It will manage all the different files  relevant to git source control

6. Start with existing project
i. Know your current directory <pwd>
ii. Navigate to the folder where you have existing project created
cd <path to the directory>

iii. git init
Initialized the git repository

7. How to open Notepad++ from gitbash

"C:\Program Files (x86)\Notepad++\notepad++.exe"
Edit Enviornment variable
Add new
Add in system variable - Variable Name: notepad++ & variable value: "C:\Program Files (x86)\Notepad++\notepad++.exe"

Edit Path and add New entry : C:\Program Files (x86)\Notepad++

Exit and reopen gitbash

8. How to use notepad++ as text editor?

i. cd Desktop/Learnings/Git/projects/git-demo
ii. notepad++ README.md
iii. Edit the content in README.md, save and exit
iv. git status (status of tracked and un-tracked files)

This is the working directory
Not added to staging area or the index

On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)



v. Add the file README.md to staging area
git add <fileName>
git add README.md

vi. git status
File is added to staging area and the changes are ready to get committed

vii. git commit - m <Message>
git commit -m "Initial commit"


viii. git status
On branch master
nothing to commit, working tree clean

9. Working on locally - working directory

i. git status
nothing to commit, clean working directory

ii. Edit the README.md text file

iii. git status
Modified file
non staged file

iv. adding new changes to the staging area
git add README.md

v.  git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

vi. git commit
git commit -m "Adding Git learnings"
[master d4b0a23] Adding Git learnings
 1 file changed, 7 insertions(+), 1 deletion(-)

inline commit messages

vii. git status
On branch master
nothing to commit, working tree clean

### Website contents
Created new file index.html