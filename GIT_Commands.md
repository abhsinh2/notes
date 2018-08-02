# Configuration

```
git config --global user.name "<NAME>"
git config --global user.email "<EMAIL>"
git config --global core.autocrlf input
```
  
# Initialize a Directory

```
git init topology
git remote add <BRANCH> <REMOTE_URL>
git status
git add .
git commit -m "intial commit"
```
  
# Useful Commands
git log

git branch

git pull --rebase

git checkout feature/test1

# Merge 

git checkout <SOURCE_BRANCH>
git pull origin <TARGET_BRANCH>
git commit
git push origin HEAD

# Reset

git fetch origin

git reset --hard origin/master

git reset <commit_id>

# Clone Specific Branch

git clone --branch <BRANCH> --depth 150 <GIT_REMOTE_URL> <DIRECTORY_NAME>
