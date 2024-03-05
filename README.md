# git_tutorial
Git Learning for beginners. Get the Git installation file here

# Configure
Using gitbash:
- specify our name

```
git config --global user.name "John Doe"
git congig --global user.email "johndoe@gmail.com
```

- Default branch name
- What for?

```
git config --global init.default branch main
```

# Asking for help

```
git config -h
```

# Turning this into git repository

Create a new repository:

```
 git init
```

Check the status of the repository
```
git status
```

> [!NOTE]  
> As for now the files are untracked. Any changes the git will not do anything.

## How do we track a file?
```
git add [filename]
```

- ignore certain files: using .gitignore
- then put the condition which file you do not want to show
- privacy or unwanted files

## How do we track all files?
```
git add --all
```

# how to commit?
```
git commit -m "Messages"
```

To see the changes for the commit:
```
git diff
```

Stages of files in the git:
1. Working files - edits to the files
2. Staging - ready state before deploying to the github
3. Commit - deploy the codes

# how do we return back to the staging process
```
git restore --staged [filename]
```

# Bypass the staging steps
```
git commit -a -m "message"
```

# delete files through git
```
git rm "filename"
git restore "filename"
```

# renaming the file
```
git mv "old name" "new name"
git log
git commit -m "message" --amend
git help log
```

# Create a new brach 
```
git branch BRANCHNAME
git branch - to see how many branches we have
git switch -c BRANCHNAME - we create and we switch to a new branch called BRANCHNAME
```

# how to merge branch back to main
```
git merge -m "Message" (branch name that we want to merge with main)
```

# How to delete branch
```
git branch -d OLDBRANCH
```

# After doing any changes to your code
- actually do this to push your local repo to the remote repository
```
git add .
git commit -m "Your commit message here"
git push origin <branch-name>
```

# When you are ready, this is the step to push code from local to remote repository

```
git init
git add .
git commit -m "Your commit message here"
git push origin main
git remote add origin <repository_URL>
git push -u origin main
```




