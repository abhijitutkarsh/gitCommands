![image](https://github.com/user-attachments/assets/365bca4b-2505-4d75-8792-93cccf426385)# gitCommands


Setup and Configuration
git config: Configures Git settings.
git config --global user.name "Your Name": Sets the username.
git config --global user.email "you@example.com": Sets the email.
git config --list: Lists all Git configurations.
Basic Workflow Commands
git init: Initializes a new Git repository in the current directory.

git init: Creates an empty Git repository or reinitializes an existing one.
git clone: Clones a repository into a new directory.

git clone <repository_url>: Downloads the repository from the given URL.
git status: Shows the working tree status.

git status: Displays the current state of the working directory and staging area.
git add: Adds changes to the staging area.

git add <file_name>: Stages a specific file.
git add .: Stages all changes in the current directory.
git commit: Records changes to the repository.

git commit -m "Your commit message": Commits the staged changes with a message.
git commit -a -m "Your commit message": Commits all changes (staged and unstaged).
git push: Uploads local repository content to a remote repository.

git push origin <branch_name>: Pushes changes to the remote branch.
git push -u origin <branch_name>: Sets the upstream branch and pushes changes.
git pull: Fetches and merges changes from a remote repository to your local branch.

git pull origin <branch_name>: Pulls changes from the remote branch.
Branching and Merging
git branch: Lists, creates, or deletes branches.

git branch: Lists all local branches.
git branch <branch_name>: Creates a new branch.
git branch -d <branch_name>: Deletes a branch.
git checkout: Switches branches or restores working tree files.

git checkout <branch_name>: Switches to the specified branch.
git checkout -b <new_branch_name>: Creates and switches to a new branch.
git merge: Merges changes from one branch into another.

git merge <branch_name>: Merges the specified branch into the current branch.
Undoing Changes
git revert: Creates a new commit that undoes changes from a previous commit.

git revert <commit_hash>: Reverts a specific commit.
git reset: Resets the current HEAD to a specified state.

git reset <commit_hash>: Resets to the specified commit, keeping changes in the working directory.
git reset --hard <commit_hash>: Resets to the specified commit and discards all changes.
git stash: Temporarily stores changes in the working directory.

git stash: Stashes the current changes.
git stash pop: Applies the stashed changes and removes them from the stash list.
Viewing History
git log: Shows the commit history.

git log: Lists commits in the current branch.
git log --oneline: Displays the commit history in a simplified, single-line format.
git diff: Shows changes between commits, branches, or your working directory.

git diff: Displays changes in the working directory that are not yet staged.
git diff --staged: Shows changes between the staging area and the last commit.
Working with Remotes
git remote: Manages remote repository connections.

git remote -v: Lists all remotes with their URLs.
git remote add <name> <url>: Adds a new remote repository.
git fetch: Downloads objects and refs from another repository.

git fetch origin: Fetches updates from the remote repository.
Advanced Commands
git rebase: Reapplies commits on top of another base tip.

git rebase <branch_name>: Reapplies commits from one branch onto another.
git rebase -i <commit_hash>: Interactive rebase for squashing or editing commits.
git tag: Creates, lists, or deletes tags.

git tag: Lists all tags.
git tag <tag_name>: Creates a new tag.
git tag -d <tag_name>: Deletes a tag.
Collaboration Commands
git cherry-pick: Applies the changes from a specific commit.

git cherry-pick <commit_hash>: Applies the changes from the specified commit to the current branch.
git bisect: Helps find the commit that introduced a bug by binary search.

git bisect start: Begins the bisecting process.
git bisect good <commit_hash>: Marks a commit as "good."
git bisect bad <commit_hash>: Marks a commit as "bad."
Clean Up Commands
git clean: Removes untracked files from the working directory.
git clean -n: Shows which files would be removed.
git clean -f: Removes untracked files.
Miscellaneous
git blame: Shows what revision and author last modified each line of a file.

git blame <file_name>: Annotates each line in the file with the commit hash and author.
git archive: Creates a tar or zip file from the contents of a tree.

git archive --format=zip --output=<file.zip> HEAD: Archives the repository's current state.
