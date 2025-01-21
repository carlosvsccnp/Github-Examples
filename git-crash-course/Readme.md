## Git Hidden Folder

There is a hidden folder called `.git`which tells you that our project is a git repo.

If we wanted to create a git repo in a new project we' create the fodler and then initialize that repo using `git init`

```sh
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
# makes changes to readme.md
git commit -m "add readme file"

```


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

```sh
git config --global core-editor emacs
```

Make a commit and commit message withouth opening and editor

```sh
git commit -m "commit message"
```

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

To find out where the file is located
```sh
git config --list --show-origin
```

When you first install Git on a machine you are suppose to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

## Log

To show show your recent git commits to the git tree

```sh
git log
```

## Push

When we want to push a repo to our remote origin

```
git push
```
