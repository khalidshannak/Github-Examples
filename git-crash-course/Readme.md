## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo. 

If we wanted to create a git repo in a new project we create the folder and the initalize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
# makes changes to readme.md
git commit -m "add readme file"
```


## Cloning

we can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/khalidshannak/Github-Examples.git
cd Github-Examples
```

## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

Set the global core.editor
```
git config --global core.ediotr 
```

Make a commit and commit message without opening an editor
```sh
git commit -m "note"
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage change that will be included in the commit we can use the . to add all possible files. 
```
git add Readme.md
git add .
```

## Reset

Reset allow you to move staged changes to be unstaged.
This is useful when you revert all files not to be commited

```
git add .
git reset
```
> git reset will revert a git add . 


## status

Git status shows you what files will or will not be commited.

```
git status
```

## Gitconfig file

The gitconfig file is what stores your global configurations for git such as email, name. 

showing the contnets of our .gitconfig file
```
git config --list
```

## log

git log will show recent git commits to the git tree

## Push

When we want to push a repo to our remote origin

```
git push
```