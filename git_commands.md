# 🛠️ Ultimate Git Commands Cheat Sheet

This cheat sheet includes all commands and variations discussed, organized by their role in the development workflow.


| Category | Command | Usage & Explanation |
| :--- | :--- | :--- |
| **Setup & Config** | `git init` | Initialize a new local repository. |
| | `git clone <url>` | Copy a remote repository to your local machine. |
| | `git config --global user.name "Name"` | Set your name for all commits. |
| | `git config --global user.email "email"` | Set your email for all commits. |
| **Workflow** | `git status` | Show changed, staged, or untracked files. |
| | `git add .` | Stage all current changes for the next commit. |
| | `git commit -m "msg"` | Save the staged snapshot to local history. |
| | `git commit --amend` | Modify the last commit (fix message or add files). |
| | `git cherry-pick <hash>` | Apply one specific commit from another branch to yours. |
| **Branching** | `git branch` | List all local branches. |
| | `git switch -c <name>` | Create a new branch and switch to it immediately. |
| | `git checkout -b <name>` | (Legacy) Create and switch to a new branch. |
| | `git merge <branch>` | Combine changes from another branch into your current one. |
| | `git rebase <branch>` | Move your current branch's commits on top of another branch. |
| **Multi-Tasking** | `git worktree add <path> <branch>` | Checkout multiple branches into separate folders simultaneously. |
| | `git worktree list / remove` | Manage and clean up active working trees. |
| **Releases** | `git tag -a <name> -m "msg"` | Mark a specific commit as a version/milestone. |
| | `git push origin --tags` | Upload all local tags to the remote server. |
| **Remote Sync** | `git remote -v` | Show the full URLs (fetch/push) of your remote connections. |
| | `git fetch` | Download updates from the server without merging them. |
| | `git pull` | Fetch and immediately merge changes from the server. |
| | `git push` | Upload your local commits to the remote repository. |
| **Inspection** | `git log --oneline` | View history as a compact, one-line-per-commit list. |
| | `git log --oneline --graph --all` | Visual "A DOG" log: show all branches and their merge history. |
| | `git stash show -p` | Peek inside the most recent stash to see the code diff. |
| | `git cat-file -p <hash>` | Inspect the raw content/metadata of any Git object. |
| **Stashing** | `git stash -m "msg"` | Save messy work with a label to clear your workspace. |
| | `git stash list` | List all your currently stashed changes. |
| | `git stash pop` | Apply the latest stash and delete it from the list. |
| | `git stash apply` | Apply the latest stash but keep it in the list. |
| **Conflicts** | `git checkout --ours <file>` | Resolve a conflict using your current branch's version. |
| | `git checkout --theirs <file>` | Resolve a conflict using the incoming branch's version. |
| **Debugging** | `git bisect` | Use binary search to find which commit introduced a bug. |
| **Recovery** | `git reflog` | The "Black Box" recorder; find any move you've made locally. |
| | `git reset --hard <hash>` | Wipe all local changes and force the branch to a specific commit. |

---
*Keep this file as a reference for your Git workflow!*