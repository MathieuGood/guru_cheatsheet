# GIT Cheat Sheet

```bash
# Init folder as git repository
git init

# Set config
git config --global user.name "MathieuGood"
git config --global user.email "bon.mathieu@gmail.com"

# Display config
git config -l

# Add files
git add script.py
git add *

# Add all files, including deleted files
git add --all
# Or
git add -A

# Set remote repository URL
git remote add origin https://github.com/Microsoft/windows.git

git push origin master


# Check log
git log

# Check log for a specific file
git log -- specific_file.html
git log --online

# See remote directory URL
git remote -v
git remote show origin

# Create new branch
git branch new_branch_name

# List local branches
git branch

# List remote branches
git branch -r

# Fetch remote branch to local branch
git fetch origin dev_remote_branch

# Set HEAD to a previous commit proviging its commit hash
git checkout commit_hash

# Replace a commit message
git commit --amend -m "New commit message"

# Create branch named "develop" and switch to this branch
git rebase -b develop

# Switch branch
git switch branch_to_switch_to



```
