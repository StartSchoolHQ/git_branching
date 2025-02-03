# Git Branching and Conflict Resolution

## 1. Introduction to Git Branching
there is some information here that could be useful

### Concepts to Cover:
- **What are branches?**
  - Git branches are a pointer to a snapshot of your changes.
- **Why use branches?**
  - To isolate features or bug fixes.
  - To enable collaboration without disrupting the main codebase.
- **Some types of branches:**
  - `main || master`: The default branch for production-ready code.
  - `feature`: Used to develop specific features.
  - `hotfix`: Used to quickly patch bugs in production.

### Commands Introduced:
- `git branch`: View existing branches.
- `git branch <branch_name>`: Create a new branch (without switching to it)
- `git checkout -b <branch_name>`: Create and switch to a new branch
- `git branch -d <branch_name>`: Delete a specified branch
- `git add`:  Add a change in the working directory to the staging area (without it, no git commit would ever do anything)
- `git commit`: 

---

## 2. Creating and Working with Branches

### Live Demonstration:

#### Create a new branch for a feature:
```
git checkout -b feature/update-file
```

#### Make changes in `file.txt`:
```
echo "Adding a new line in feature branch" >> file.txt
cat file.txt
```

#### Commit the changes:
```
git add file.txt
git commit -m "Updated file in feature branch"
```

#### Switch back to the `master` branch:
```bash
git checkout main
```

#### Modify `file.txt` in the `master` branch:
```bash
echo "Adding another line in master branch" >> file.txt
git add file.txt
git commit -m "Updated file in master branch"
```

---

### Notes:
- Use branches to keep your work organized and avoid conflicts.
- Always commit your changes to avoid losing progress.
- Test your changes before merging back into `main`.

This process ensures smooth collaboration and a clean codebase.
