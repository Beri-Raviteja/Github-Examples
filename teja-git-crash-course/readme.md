## Git hidden folder
> There is a hidden folder called `.git` which tells you that our project is a git repo.
If we want to create a git repo in a new project we would create the folder and then initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
open Readme.md
git status
git add  Readme.md
# make changes to Readme.md
git commit -m "add readme file"
```


## Cloning

> we can clone in three ways. they are HTTPS, SSH, Github CLI

> Since we are using Github Codespaces we will create a temporary in our workspace


```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## HTTPS

```sh
git clone https://github.com/Beri-Raviteja/Github-Examples.git
cd Github-Examples
```

## Commits

> When we want to commit code we can write git commit whuch will open up the commit edit message in the editor of choice.

```sh
git commit
```
> set the global editor

```
git config --global core.editor emacs
```
make a commit and commit message without opening the editor
```sh
git commit -m "add another exclamation"

## Branches

## Remotes

## Stashing

## Merging

## Add
when we want to stage charges that will be in cluded in the commit
we can use the . to add all possible files.

```
git add Readme.md
git add .
```
## Git reset
Reset allows tou to staged changes to be unsdtaged.
This is useful when you want to revert all files to be not commited

```
git add .
git reset
```
>git reset will revert a git add .
## status
Git status shows you what files will or will not be committed

```
git status
```

## Gitconfig file
The gitconfig file is what stores your global configuration for git such as email, name, editor and more.

Thats showing the contents of our .gitconfig file
```
git config --list
```

When you first install Git on a machine you are suppose  to set up your name and email
```sh
git config --global user.name "john Due"
git config --global user.mail johndoe@example.com
```

## log
git log will show recent git commits to the git tree

## Push
When we want to push a repo to our remote origin

```
git push

```

