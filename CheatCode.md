GitHub / Git Complete Cheat Sheet

Initial Setup

git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
git config --list

Create Repository

git init
git clone https://github.com/user/repo.git

Check Status

git status
git status -s

Add Files

git add file.txt
git add .
git add -A
git add *.py

Commit

git commit -m "Initial commit"
git commit -am "Update code"
git commit --amend

View History

git log
git log --oneline
git log --graph
git log --all --decorate --oneline
git show

Branches

git branch
git branch new-feature
git switch new-feature
git switch -c new-feature
git checkout new-feature
git checkout -b new-feature
git branch -d new-feature
git branch -D new-feature

Merge

git merge feature-branch
git merge --no-ff feature-branch

Rebase

git rebase main
git rebase -i HEAD~5

Remote Repositories

git remote -v
git remote add origin https://github.com/user/repo.git
git remote remove origin
git remote rename origin upstream

Push

git push
git push origin main
git push -u origin main
git push --force
git push --force-with-lease

Pull & Fetch

git fetch
git fetch --all
git pull
git pull origin main

Stash

git stash
git stash save "work"
git stash list
git stash apply
git stash pop
git stash drop
git stash clear

Undo Changes

Unstage file

git restore --staged file.txt

Discard changes

git restore file.txt

Reset commit

git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1

Revert commit

git revert COMMIT_ID

Compare Changes

git diff
git diff --staged
git diff branch1 branch2

Tags

git tag
git tag v1.0
git tag -a v1.0 -m "Release"
git push origin v1.0
git push origin --tags

Delete Files

git rm file.txt
git rm -r folder/

Rename Files

git mv old.txt new.txt

Git Ignore

touch .gitignore

Example:

venv/
__pycache__/
.env
*.log
*.pyc
node_modules/

Clean Untracked Files

git clean -n
git clean -f
git clean -fd

Inspect Repository

git ls-files
git blame file.py
git shortlog

Cherry Pick

git cherry-pick COMMIT_ID

Work with Specific Commit

git checkout COMMIT_ID
git switch -

GitHub Authentication

gh auth login

GitHub CLI

gh repo create
gh repo clone user/repo
gh repo view
gh repo delete
gh pr create
gh pr list
gh pr view
gh issue create
gh issue list
gh release create v1.0

Common Daily Workflow

git pull
git checkout -b feature
# code changes
git add .
git commit -m "Added feature"
git push -u origin feature

Emergency Commands

git reflog

Recover deleted commit:

git reflog
git reset --hard COMMIT_ID

One-Liners

Clone and enter:

git clone URL && cd repo

Create repo and first commit:

git init
git add .
git commit -m "Initial commit"

Push existing project:

git remote add origin URL
git branch -M main
git push -u origin main
