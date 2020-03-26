# Practice repository to start learning git

## Commands used

- git init: Create a new git repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history of all project commits
- git show: Show a single commit
- git diff: Show the difference between commits, the working directory, and
  the staging area.
- git checkout: Check out branch (Update HEAD and apply changes to working
  directory)
- git branch: List branches
- git branch -c: Create a branch
- git merge: Merge changes from different branches
- git checkout: check out a branch, update HEAD
- git checkout -b create a new branch, then check it out
- git stash: Stash changes from working directory
- git stash list: List stashes
- git stash pop: Apply stashed changes to working directory
- git remote add <remote> <url>: Add a new <remote> at <url>
- git remote -v: List remote repositories
- git push -u <remote> <branch>: Push <branch> to <remote>, and set default upstream for <branch>
- git fetch: Fetch changes from remote repository

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a
branch, we say we're "on" that branch. When we make a commit
while we're on a branch, the branch is updated to ref(er) to the
new commit .

## What's HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit...
more on that later). Git commands like 'status', 'log', and 'branch'
use HEAD. 'git checkout' updates HEAD to ref(er) to a different branch.

## Commit messages

git commit -m "<message>"

- first line should be clear accurate, and concise
- use proper spelling
- don't end with a '.'

For more advice, see https://chris.beams.io/posts/git-commit/

## Merging

Merging means to bring changes from one branch into another

- A fast forward merge happens when the target branch was branched from the current one,
  and there are no new changes to the current branch since then
- An automatic merge happens when the two histories have diverged but git is able to
  reconcile them into one set of changes. This creates a new commit on the current branch.
