# Practice repository to start learning git

## Commands used

- git init: Create a repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history of all project commits
- git checkout: Check out branch (Update HEAD and apply changes to working
  directory)
- git merge: Merge changes from different branches

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
