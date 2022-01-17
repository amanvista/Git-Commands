Git Commands
============
### GIT Remove
*  git remote add origin git@github.com:amanvista/Movie-Watchlist.git
*  git remote set-url origin git@github.com:amanvista/Movie-Watchlist.git
*  git push -u origin master
### deleting accidently deleted file
* git gc --prune=now --aggressive : removing all files greater than 100 MB
* git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch mern.mp4' --prune-empty --tag-name-filter cat -- --all
### Git Checkout
* git checkout -- .
### Creating RSA key in MAC
* ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
* eval "$(ssh-agent -s)"
* cd .ssh
* cat id_rsa.pub

### Setup Email and Username
* git config --global user.email "amanvista@gmail.com"
* git config --global user.name "Aman Bisht"




### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init .` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git checkout <commit hash code/branch name> `| checkout to particular hash | 
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |

### Ignore Version Control

| Command | Description |
| ------- | ----------- |
| `.gitignore` | Ignore files |
