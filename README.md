# Git Branching and Conflict Resolution

## 1. Introduction to Git Branching (5 minutes)

### Concepts to Cover:
- **Why use branches?**
  - To isolate features or bug fixes.
  - To enable collaboration without disrupting the main codebase.
- **Types of branches:**
  - `main`: The default branch for production-ready code.
  - `feature`: Used to develop specific features.
  - `hotfix`: Used to quickly patch bugs in production.

### Commands Introduced:
- `git branch`: View existing branches.
- `git checkout -b`: Create and switch to a new branch.

---

## 2. Creating and Working with Branches (10 minutes)

### Live Demonstration:

#### Create a new branch for a feature:
```bash
git checkout -b feature/update-file
```

#### Make changes in `file.txt`:
```bash
echo "Adding a new line in feature branch" >> file.txt
cat file.txt
```

#### Commit the changes:
```bash
git add file.txt
git commit -m "Updated file in feature branch"
```

#### Switch back to the `main` branch:
```bash
git checkout main
```

#### Modify `file.txt` in the `main` branch:
```bash
echo "Adding another line in main branch" >> file.txt
git add file.txt
git commit -m "Updated file in main branch"
```

---

### Notes:
- Use branches to keep your work organized and avoid conflicts.
- Always commit your changes to avoid losing progress.
- Test your changes before merging back into `main`.

This process ensures smooth collaboration and a clean codebase.
