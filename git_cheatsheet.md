# GIT Cheat Sheet

```bash
# Init folder as git repository
git init

# Init folder as remote git repository
git init . --bare

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

# Change remote directory URL
git remote set-url origin remote_url

# Create new branch
git branch new_branch_name

# Delete branch
git branch -d branch_to_delete
git branch -D branch_to_delete

# List local branches
git branch

# List available branches
git branch -r

# Fetch remote branch to local branch
git fetch origin dev_remote_branch

# Set HEAD to a previous commit providing its commit hash
git checkout commit_hash

# Replace a commit message
git commit --amend -m "New commit message"

# Create branch named "develop" and switch to this branch
git rebase -b develop

# Switch branch
git switch branch_to_switch_to

# Merge branch B into branch A including commit messages
git merge branch_b

# Merge and stop at commit message to edit
git merge branch_b --no-ff

# Merge and don't commit any message, just add files
git merge branch_b --squash


```