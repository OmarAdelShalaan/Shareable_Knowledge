# Git

### What is Git?
Git is a distributed **version control system**. It tracks changes in your project files, so you can:
- Revert to previous states of the project.
- Collaborate with others without conflicts.
- Branch and work on different features simultaneously.
- Merge branches back into the main project seamlessly.

### Basic Git Workflow
- **Modify Files:** You change or create files in your project directory.
- **Stage Changes:** You add the changes to the staging area to tell Git to keep track of these specific changes.
- **Commit Changes:** You save a snapshot of the staged changes, making them part of your Git history.
- **Push Changes:** You send your committed changes to a remote repository (e.g., GitHub, GitLab, etc.).

### Git Stages

![git_Stages](./)

### Install Git
- **Windows**
```link
```
- **Linux**
```bash
$ sudo apt install git
```

## Git Commands

### Git Help & Manual
```bash
$ git help
# OR
$ man git
```

### Creating a Git Repository

```bash
$ git init
```
This creates a hidden **.git** directory inside the folder, and Git will start tracking changes from here.

### Cloning a Repository

```bash
$ git clone https://github.com/username/repository.git
```
to download an existing repository from GitHub or another Git server


### Checking the Status

```bash
$ git status
```
see which files have changed and which files are staged for a commit

### Adding Changes to the Staging Area

```bash
$ git add <file-name>       # Add specific file
$ git add .                 # Add all changes in the current directory
```
make changes to files, you need to add them to the staging area

### Committing Changes

```bash
$ git commit -m "Your commit message: It's important to write clear commit messages explaining what the changes are."

```
After adding files to the staging area, commit them to record the changes in Git

### Viewing the Commit History

```bash
$ git log
```
see all the commits made to the repository

### Pushing Changes to a Remote Repository

```bash
$ git push origin main   # Push to the main branch of the remote
# OR
$ git push
```
After committing changes, push them to a remote repository (like GitHub)


### Pulling Changes from a Remote Repository

```bash
$ git pull origin main   # Pull from the main branch of the remote
# OR
$ git pull
```
to pull the latest changes from a remote repository

### Branching and Merging

- **Branching** allows creating separate lines of development, so you can work on new features **without** affecting the main project.

```bash
$ git branch   <branch-name>      # Create a new branch
$ git checkout -b <branch-name>   # Create a new branch branch
# -B is given, <new_branch> is created if it doesn’t exist; otherwise, it is reset.
```
- **Checkout Branch** to change Branch
```bash
$ git checkout <branch-name> # Switch to that branch
```

- **Merging** brings changes from one branch into another (usually the main branch)

```bash
$ git checkout main           # Switch to the main branch
$ git merge <branch-name>     # Merge your branch into main
```

- **Delete  branch**
```bash
$ git branch -d <branch-name>  # Only deletes if the branch has been merged
$ git branch -D <branch-name>  # Force delete even if not merged
```

### Stashing Changes
- If you’re in the middle of some work and want to switch branches but aren’t ready to commit your changes, you can temporarily stash your changes
```bash
$ git stash
```
- To bring those changes back later
```bash
$ git pop
```
 
### Undoing Changes
- To undo changes before committing (but keep them unstaged)
```bash
$ git restore <file>
```
- To reset the entire working directory
```bash
$ git reset --hard
```


## Git Collaboration

### Forking and Pull Requests (on GitHub)

**Forking allows you to copy someone else's repository to your GitHub account.**
- You can make changes to this copy and then submit a pull request to suggest your changes to the original repository.

**Resolving Merge Conflicts**

- When working on a shared project, you might run into merge conflicts, where Git can’t automatically merge two changes. You’ll need to manually resolve these conflicts in your code files. 

## Git Aliases
Aliases are shortcuts for Git commands that you can define in your .gitconfig file to save time.

```bash
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.cm "commit -m"
$ git config --global alias.st status
```

## General Token
### On GitHub:
1. Go to your GitHub Personal Access Token settings.
Click on "Generate new token".
2. Select the appropriate scopes (permissions) depending on what you need (e.g., repository access, workflow, Gist, etc.).
3. Generate the token and copy it. You won’t be able to see it again after navigating away from this page.


### Use HTTPS and the Token as Password

```bash
$ git remote set-url origin https://<YOUR_GITHUB_USERNAME>:<YOUR_PERSONAL_ACCESS_TOKEN>@github.com/<USERNAME>/<REPO>.git
```
