# Git Commands Cheat Sheet

## Git Terminology

Here are some key terms to understand Git commands better:

- **Repository (Repo)**: A directory where your project's code and version history are stored. It's the core of Git's functionality.
- **Commit**: A snapshot of your project's current state. Think of it as saving your progress.
- **Branch**: A pointer to a series of commits. Used to develop features or work on fixes separately from the main codebase.
- **Staging Area (Index)**: A preparatory area where changes are placed before committing. It helps you organize what gets committed.
- **Working Directory**: The local directory where your project files reside. Changes made here can be staged or committed.
- **Remote Repository**: A repository hosted on a server (like GitHub, GitLab, or Bitbucket) that allows collaboration with others.
- **Clone**: Copying a remote repository to your local machine.
- **Pull**: Fetching changes from a remote repository and merging them into your local branch.
- **Push**: Sending your local changes to a remote repository.
- **Merge**: Combining changes from one branch into another.
- **Rebase**: Reapplying commits on top of another branch's history, often used to clean up commit history.
- **Tag**: A marker for a specific commit, usually used for releases.
- **Stash**: A way to save changes temporarily without committing them.
- **Reset**: Undoing changes by moving the current branch to a different commit.
- **Revert**: Creating a new commit to undo changes made by a specific previous commit.
- **Checkout**: Switching between branches or specific commits.
- **HEAD**: The current commit or branch that you are working on.
- **Upstream/Origin**: A reference to a remote repository (commonly named `origin`).
- **Conflict**: Happens when Git cannot automatically resolve differences between branches during a merge or rebase.
- **Fast-Forward Merge**: A merge that simply moves the branch pointer because no additional commits exist on the target branch.
- **Detached HEAD**: A state where HEAD points to a specific commit instead of a branch.

Use this glossary to enhance your understanding of Git commands and workflows.

## Basics
- `git init` - Initialize a new Git repository.
- `git clone <repo-url>` - Clone a repository into a new directory.
- `git status` - Display the status of the working directory and staging area.
- `git add <file>` - Add a file to the staging area.
- `git add .` - Add all files to the staging area.
- `git commit -m "<message>"` - Commit staged changes with a message.
- `git log` - Show commit logs.
- `git show <commit>` - Display detailed information about a specific commit.
- `git diff` - Show changes between working directory and staging area.
- `git diff --staged` - Show changes between staging area and last commit.
- `git branch` - List all branches in the repository.
- `git branch <branch-name>` - Create a new branch.
- `git checkout <branch-name>` - Switch to a specific branch.
- `git checkout -b <branch-name>` - Create and switch to a new branch.
- `git merge <branch-name>` - Merge a branch into the current branch.

## Remote Repositories
- `git remote add <name> <url>` - Add a remote repository.
- `git remote -v` - List remote repositories.
- `git fetch` - Download objects and refs from a remote repository.
- `git pull` - Fetch and integrate changes from a remote repository into the current branch.
- `git push` - Upload local changes to a remote repository.
- `git push -u origin <branch-name>` - Push a branch and set upstream tracking.
- `git remote remove <name>` - Remove a remote repository.

## Undoing Changes
- `git restore <file>` - Restore a file from the last commit.
- `git restore --staged <file>` - Unstage a file.
- `git reset <commit>` - Reset the current branch to a specific commit.
- `git reset --soft <commit>` - Reset to a commit, keeping changes staged.
- `git reset --hard <commit>` - Reset to a commit and discard all changes.
- `git revert <commit>` - Create a new commit to undo changes from a specific commit.

## Stashing
- `git stash` - Save changes temporarily without committing.
- `git stash list` - List all stashes.
- `git stash apply <stash-id>` - Apply a specific stash.
- `git stash drop <stash-id>` - Remove a specific stash.
- `git stash clear` - Remove all stashes.

## Tagging
- `git tag <tag-name>` - Create a lightweight tag.
- `git tag -a <tag-name> -m "<message>"` - Create an annotated tag.
- `git push origin <tag-name>` - Push a tag to the remote repository.
- `git tag -d <tag-name>` - Delete a tag locally.
- `git push origin --delete <tag-name>` - Delete a tag from the remote repository.

## Advanced Commands
- `git cherry-pick <commit>` - Apply changes from a specific commit to the current branch.
- `git rebase <branch-name>` - Reapply commits on top of another branch.
- `git reflog` - Show the history of HEAD changes.
- `git bisect` - Use binary search to find the commit that introduced a bug.
- `git submodule add <repo-url>` - Add a submodule to the repository.
- `git submodule update --init` - Initialize and update submodules.
- `git blame <file>` - Show who made changes to each line in a file.
- `git archive --format=zip --output=<filename.zip> HEAD` - Create a zip archive of the repository.

## Cleaning
- `git clean -n` - Show files that would be removed by `git clean`.
- `git clean -f` - Remove untracked files from the working directory.
- `git clean -fd` - Remove untracked files and directories.

## Collaboration
- `git fetch --prune` - Remove remote-tracking branches that no longer exist.
- `git merge --no-ff <branch-name>` - Merge with a non-fast-forward merge.
- `git pull --rebase` - Fetch changes and reapply commits on top of them.
- `git push --force` - Force push changes to a remote repository.
- `git push --force-with-lease` - Force push only if no one else has pushed.

## Aliases
- `git config --global alias.<alias-name> <command>` - Create a custom alias for a Git command.
- `git config --list` - List all configured Git settings.
- `git config --global user.name "<name>"` - Set the global username.
- `git config --global user.email "<email>"` - Set the global email.

## Miscellaneous
- `git grep "<pattern>"` - Search for a string in the repository.
- `git shortlog -s -n` - Show contributors sorted by the number of commits.
- `git rev-parse HEAD` - Get the hash of the latest commit.
- `git diff-tree --no-commit-id --name-only -r <commit>` - Show files changed in a specific commit.


## Author

Created and maintained by [Albin Aji](https://github.com/albin6).

- GitHub: [Albin Aji](https://github.com/albin6)
- Email: albinpariyarathu@gmail.com
