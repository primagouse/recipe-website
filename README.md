# recipe-website

This is my first website. I am using it to learn how to use git and github to start with. I will keep my notes in this file.

git status: checks status of directory

git add .: adds all files (untracked and modified files when I check status) to staging area - this means files are being tracked by git

git commit -m "message" -m "description": commits files to local repository - this means files are being saved to the local repository

git push: pushes files to remote repository - this means files are being saved to the remote repository once I have added them to the staging area and committed them to the local repository. I do this when I am ready to share my changes with others.

git log --oneline: shows the commit history with shortened commit IDs

git mv recipe.html index.html: renames recipe.html to index.html
have not used these yet:

git diff: shows the changes between what has been staged and what is in the local repository
----
git checkout <commit-id> <filename>: reverts specific file to version from that commit

git reset --hard <commit-id>: reverts entire repository to that commit (warning: this will delete all changes after that commit!)

git branch <branch-name>: creates a new branch

git checkout <branch-name>: switches to that branch

git merge <branch-name>: merges the specified branch into the current branch

-----


Explanation of workflow:

After saving your changes, you'll need to use git add again before committing. Even though the file is already being tracked, any new modifications need to be staged before they can be committed.
The workflow is:
Make changes
Save changes
git add recipe.html (or git add . for all changes)
4. git commit -m "your message"
This is because Git uses a staging area (also called the index) as an intermediate step between your working directory and the repository. Each time you modify a tracked file, you need to stage those new changes using git add before you can commit them.
You can think of it like taking a photo - even if you've photographed something before, you need to take a new photo to capture its current state. Similarly, git add takes a new "snapshot" of the file's current state to prepare it for committing.


