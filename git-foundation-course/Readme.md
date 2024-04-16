## 1. GitCrashCourse

### a. COMMIT
### b. BRANCHES
### c. REMOTES
### d. STASHING
### e. MERGING
### f. CLONING
### g. GITHIDDEN FOLDER
### h. Reset
### i. ADD
### j. GITCONFIG

GitHidden Folder
There is a hidden folder called `.git` which tells you that your project is a git Project.

If we want to create a git repo in a new folder we'd create the folder and initalize that repo using `git init`

```
mkdir /workspaces/temp/new-project
cd /workspaces/temp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
# Make changes to readme.md
git commit -a -m "add readme file"
```

since we are using GitHub Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspaces/temp
cd /workspaces/temp
```

1. Cloning:
We can clone in 3 ways: HTTPs, SSH, Github CLI

### HTTPs
```sh
git clone https://github.com/RohanK1804/GitFoundation.git
cd GitFoundation
```

> You'll need to Genrate a Personal Access Token(PAT)

https://github.com/settings/tokens

You will need the PAT as your password when you Login
-Give it access to contents for commits


### SSH


## Add
When we want to stage changes that will be included in the commit
We can use the . to add all the possible files.
```
git add Readme.md
git add .
```

## Reset
Reset allows you to move staged changes to be unstaged
this is usefull when you want to revert all files not to be commited 

```
git add .
git reset
```

> git reset will reverse a git add .

## Status
Git Status show you what files will or will not be commited.

```
git status
```

## Commit
when we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.
```sh
git commit
```
to set the global editor 
```
git config --global core.editor emacs
```

## Gitconfig File
The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

showing the contents of our .gitconfig file
``` sh
git config --list 
```

When you first install Git on a machine you are suppose to set up your name & email

```sh
git config --global user.name  "Rohan.Kharatmol"
git config --global user.email "kharatmol180@example.com"
```


### My Refrence
Git Add All :
```sh
git add .
```
Git Reset (Resets all file to untracked)
```sh
git reset
````
