# Git Collaboration Practices

## Working Directory vs Staging vs History
* **Working Directory:** The actual local workspace directory on your machine where you are creating, editing, and deleting files. Changes here are untracked until staged.
* **Staging Area (Index):** A landing zone where files are prepared and marked to be included in the next snapshot commit. It allows you to select exactly what changes to group together.
* **Commit History:** The permanent record of safely snapshot records stored inside the `.git` directory. Once committed, changes are cryptographically tracked and retrievable.

## Branching Rules
* **Protect Main:** Never develop or commit code directly to the `main` branch. 
* **Feature Isolation:** Create short-lived, uniquely named feature branches (e.g., `feature/login-ui`) for every ticket or structural task.
* **Keep Updated:** Frequently pull updates from the remote `main` branch into your feature branch to prevent large merge conflicts later.

## Pull Request Expectations
* **Atomic Commits:** Keep your commit messages descriptive, small, and isolated to one clear logical change.
* **Peer Reviews:** All code branches must pass a code review by at least one other engineer before being merged into the master history.
* **Green Builds:** Code must successfully pass all automated GitHub Actions verification pipeline checks before the Pull Request is approved.