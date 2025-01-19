## Git Hidden Folder

There is a hidden folder called `.git`which tells you that our project is a git repo.

If we wanted to create a git repo in a new project we' create the fodler and then initialize that repo using `git init`




## Cloning

We can clone three ways: 
- HTTPS
- SSH
- Github CLI

Since we are using Github Codespaces we'll a create a temporary directory in our workspace

```sh
mkdir /workspaces/tmp
cd /workspaces/tmp
```

### HTTPS

```sh
git clone https://github.com/carlosvsccnp/Github-Examples.git
```



## Commits

When we want to commit code we can write git commit which will open the commit edit message in the editor of choice.

```sh
git commit
```

Set the global editor

´´´sh
git config --global core-editor emacs
´´´

## Branches


## Remotes


## Stashing


## Merging

## git add

When we want to stage changes that will be included in the commit, we can use the `.`to add all possible files.

```sh
git add Readme.md
git add .
```

## git reset

Reset allows you to move Staged changes to be unstaged.

This is usefull when you want to revert all files not te commited.

```sh
git add .
git reset
````

> git reset will revert a `git add .`

## git status

Git status shows you what files will or will not be comited

```sh
git status
```

## Git config file

The gitconfig file is what stores your global configuration for git such as email, name, editor and more

Showing the content of our .gitconfig file
```sh
git config --list
```

```sh
git config --list --show-origin
```