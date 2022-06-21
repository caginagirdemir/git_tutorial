# Git Tutorial

## Sections

<details>
  <summary> Setup </summary>
  
## Setup

Set the name and email that will be attached to your commits and tags.
```
$> git config --global user.name  "Cagin Agirdemir"
$> git config --global user.email "caginagirdemir@gmail.com"
```
  
</details>  

<details>
  <summary> Start a Project </summary>

## Start a Project

Create a local repo
```
$> git init
```
or
Download a remote repo
```
$> git clone <url>
```

</details>  
  
<details>
  <summary> Make a Change </summary>
  
## Make a Change

Add a file to staging (sahneye koyma)

```
$> git add <file>
$> git add .
```

Commit all staged giles to git

```
$> git commit -m "commit message"
```

Add all changes made to tracked files & commit

```
$> git commit -am "commit message"
```
  
</details>  

<details>
  <summary> Basic Concepts </summary>

## Basic Concepts

**main**\: default development branch
  
**origin**\: default upstream repo
  
**HEAD**\: current branch
  
**HEAD\^**\: parent of HEAD
  
**HEAD\~4**\: great\-great grandparent of HEAD
  
</details> 
  
<details>
  <summary> Branches </summary>

## Branches

List all local branches. Add -r flag to show all remote branches. -a flag for all branches.

```
$> git branch
```

Create a new branch

```
$> git branch <new-branch>
```

Switch to a branch & update the working directory

```
$> git checkout <branch>
```

Create a new branch and switch to it

```
$> git checkout -b <new-branch>
```

Delete a merged branch

```
$> git checkout -d <branch>
```

Delete a branch, whether merged or not

```
$> git checkout -D <branch>
```

Add a tag to current commit (often used for new version releases)

```
$> git tag <tag-name>
```
  
</details> 
  
<details>
  <summary> Merging </summary>

## Merging (combine branches with  history)

Merge branch a into branch b.

```
$> git checkout b
$> git merge a
```
  
</details> 
  
<details>
  <summary> Rebasing </summary>

## Rebasing (combine branches wihtout history)

Rebase feature branch onto main (to incorporate new changes made to main). Prevents unnecessary merge commits into feature, keeping history clean

```
$> git checkout feature
$> git merge main
```
  
</details> 
  

  
<details>
  <summary> Undo Things </summary>

## Undoing Things

Move (&/or rename) a file & stage move

```
$> git mv <existing_path> <new_path>
```

Remove a file from working directory & staging area, then stage the removal

```
$> git rm <file>
```

Create a new commit, reverting the changes from a specified commit

```
$> git revert <commit_ID>
```

Go back to a previous commit & delete all commits ahead of it (revert is safer). 

```
$> git reset <commit_ID>
```
  
</details> 
  
<details>
  <summary> Review your Repo </summary>
  
## Review your Repo

List new or modified files not yer committed


```
$> git status
```
  
List commit history, with respective IDs
  
```
$> git log --oneline
```
  
Show changes to unstaged files. For changes to staged files, add --cached option
  
```
$> git diif
```
  
Show changes between two commits
  
```
$> git diff commit_1ID commit2_ID
```
  
</details> 
  
<details>
  <summary> Synchronizing </summary>

## Synchronizing
  
Add a remote repo
  
```
$> git remote add <alias> <url>
``` 

View all remote connections. Add -v flag to view urks.

```
$> git remote 
``` 
  
Remove a connection
 
```
$> git remote remove <alias>
``` 
  
Rename a connection
  
```
$> git remote rename <old> <new>
``` 
  
Fetch all branches from remote repo (no merge)
  
```
$> git fetch <alias>
``` 

Fetch a specific branch
  
```
$> git fetch <alias> <branch>
``` 
  
Fetch the remote repo's copy of the current branch, then merge (fetch + merge)

```
$> git pull
``` 
Move (rebase) your local changes onto the top of new changes made to the remote repo (for clean, linear history)

```
$> git pull --rebase <alieas>
``` 
  
Upload local content to remote repo
  
```
$> git push
``` 
  
Upload to a branch (can then pull request)
  
```
$> git push <alias> <branch>
``` 

</details> 
