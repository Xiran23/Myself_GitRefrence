
# GIT REFRENCE FOR MYSELF 

## Basic Git Commands and Concepts

### Configuring Git

Set your user name and email:

```bash
git config --global user.name "URSELF_NAME"
git config --global user.email "URSELF#4@gmail.com"

```

View your user name and email:

```bash
git config --global user.name
git config --global user.email

```

### Initializing a Repository

Initialize a new Git repository:

```bash
git init

```

### Basic File Operations

List files, including hidden ones:

```bash
ls -lart

```

Check the status of your repository:

```bash
git status

```

### Staging and Committing Changes

Stage a specific file:

```bash
git add <file_name>

```

Stage all changes:

```bash
git add -A

```

Commit staged changes with a message:

```bash
git commit -m "commit message"

```

Commit all changes at once (staging and committing):

```bash
git commit -a -m "commit message"

```

### Checking Status and Logs

Show the commit logs:

```bash
git log

```

Show the last 5 commits with patches:

```bash
git log -p -5

```

### Viewing Differences

View differences between working directory and staging area:

```bash
git diff

```

View differences between staging area and the last commit:

```bash
git diff --staged

```

### Recovering Files

Recover a specific file:

```bash
git checkout <file_name>

```

Forcefully recover all files:

```bash
git checkout -f

```

### Removing Files

Remove a file from the working directory and staging area:

```bash
git rm <file_name>

```

Remove a file only from the staging area:

```bash
git rm --cached <file_name>

```

### Ignoring Files

Create a `.gitignore` file:

```bash
touch .gitignore

```

Add files or patterns to ignore:

```
log.txt
/mylog
*.log
*.html
*.cpp
foldername/

```

### Working with Branches

Create a new branch:

```bash
git branch <branch_name>

```

Check out (switch to) a branch:

```bash
git checkout <branch_name>

```

Create and switch to a new branch:

```bash
git checkout -b <branch_name>

```

### Merging Branches

Merge changes from another branch into the current branch:

```bash
git merge <branch_name>

```

Typical workflow for merging:

1. Make changes and commit on `feature1` branch:
    
    ```bash
    git add -A
    git commit -m "commit message"
    
    ```
    
2. Switch back to the master branch:
    
    ```bash
    git checkout master
    
    ```
    
3. Merge `feature1` branch into `master`:
    
    ```bash
    git merge feature1
    
    ```
    

This summary covers the essential Git commands and workflows for managing a Git repository. 

