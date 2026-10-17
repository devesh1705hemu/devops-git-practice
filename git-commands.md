
# Git Commands Cheat Sheet

## 1. Git Merge

| Command | Use |
|---|---|
| `git switch main` | Switch to the main branch. |
| `git switch -c feature-login` | Create and switch to a new feature branch. |
| `git merge feature-login` | Merge the feature branch into the current branch. |
| `git merge --no-ff feature-login` | Merge while creating a merge commit, even when fast-forward is possible. |
| `git merge --squash feature-profile` | Combine feature branch changes into the working tree without creating a merge commit. |
| `git merge --abort` | Abort an in-progress merge and return to the pre-merge state. |
| `git status` | Check the current repository state and conflicts. |
| `git log --oneline --graph --all` | View commit history as a graph across branches. |
>>>>>>> 42dbccc (modified files)

## 2. Git Rebase

| Command | Use |
|---|---|
| `git rebase main` | Replay the current branch commits on top of main. |
| `git rebase --continue` | Continue the rebase after resolving conflicts and staging changes. |
| `git rebase --abort` | Cancel the rebase and return to the original branch state. |
| `git rebase --skip` | Skip the current commit during a rebase. |
| `git log --oneline --graph --all` | Compare commit history across branches. |

## 3. Squash and Commit History

| Command | Use |
|---|---|
| `git merge --squash feature-profile` | Combine all changes from a feature branch into one pending change set. |
| `git commit -m "Add user profile feature"` | Save staged changes as a commit with a message. |
| `git merge --no-ff feature-settings` | Preserve a separate merge commit for the feature branch. |
| `git log --oneline` | Display a compact commit history. |
| `git log --oneline --graph --all` | Visualize branches and merge history. |

## 4. Git Stash

| Command | Use |
|---|---|
| `git stash` | Temporarily save tracked-file changes and clean the working tree. |
| `git stash push -m "WIP: dashboard"` | Save changes with a descriptive stash message. |
| `git stash push -u -m "WIP: dashboard"` | Stash tracked and untracked files with a message. |
| `git stash list` | List all saved stashes. |
| `git stash pop` | Apply the latest stash and remove it from the stash list if successful. |
| `git stash apply` | Apply the latest stash while keeping it in the stash list. |
| `git stash apply 'stash@{1}'` | Apply a specific stash without removing it. |
| `git stash drop 'stash@{1}'` | Delete a specific stash entry. |
| `git stash clear` | Delete all stash entries. |
| `git stash show -p` | Display the changes saved in the latest stash. |

## 5. Git Cherry-Pick

| Command | Use |
|---|---|
| `git cherry-pick <commit-hash>` | Apply a specific commit to the current branch. |
| `git cherry-pick --continue` | Continue cherry-picking after resolving conflicts and staging changes. |
| `git cherry-pick --abort` | Cancel the current cherry-pick operation. |
| `git cherry-pick --skip` | Skip the current commit during cherry-picking. |
| `git show <commit-hash>` | Inspect the details and changes of a specific commit. |
| `git log --oneline -5` | Display the five most recent commits. |

## 6. Conflict Resolution and Inspection

| Command | Use |
|---|---|
| `git status` | Identify conflicted files and the current operation. |
| `git diff` | View unstaged changes and conflict-related differences. |
| `git diff --staged` | Review changes staged for the next commit. |
| `git add <filename>` | Stage a resolved file after fixing conflicts. |
| `git commit -m "Resolve merge conflict"` | Commit the staged resolution when Git requires a manual commit. |
| `git switch <branch-name>` | Switch to an existing branch. |
| `git branch` | List local branches and identify the current branch. |

## Important Notes

- Run `git merge <branch-name>` from the branch that should receive the changes.
- Rebase rewrites commit history. Avoid rebasing commits that others already depend on.
- Use `git stash apply` when you want to keep the stash available.
- Use `git stash pop` when you want to apply the stash and remove it if successful.
- Cherry-pick is useful for moving a specific fix or commit between branches.
- Always run `git status` after resolving conflicts to verify the repository state.

