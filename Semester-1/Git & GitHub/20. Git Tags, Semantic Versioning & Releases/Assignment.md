
# Assignment – Git Tags, Sematic Versioning & Releases

### Day 20

---

## Objective
By completing this assignment, you will learn how to:
- Create Lightweight and Annotated tags
- Use tags for versioning
- Push tags to GitHub
- Create GitHub Releases
- Understand the difference between personal and professional use of tags

---

## Part A: Solo Work (Lightweight Tags)

1. Create a new repository or use your existing practice repository.
2. Make at least **3 commits** on the `main` branch.
3. Create **Lightweight tags** on these commits as personal bookmarks.  
   Example names:
   - `bookmark-setup`
   - `bookmark-structure`
   - `temp-trial`

4. Run the following command and take a screenshot:
   ```bash
   git tag
   ```

---

## Part B: Collaborative Style (Annotated Tags)

Now imagine 2-3 developers have joined your project. From now on, use only **Annotated tags**.

### Steps:

1. Create three branches:
   ```bash
   git branch feature/major-update
   git branch feature/minor-update
   git branch bugfix/login-issue
   ```

2. **Major Update (v1.0.0)**
   - Switch to `feature/major-update`
   - Make **3 commits** (example: Authentication, Home Page, Payment Gateway)
   - Merge the branch into `main` using `--no-ff`
   - Create an **Annotated tag** on the merge commit:
     ```bash
     git tag -a v1.0.0 -m "First stable release - Auth, Home Page & Payment Gateway"
     ```

3. **Minor Update (v1.1.0)**
   - Switch to `feature/minor-update`
   - Make **2 commits** (example: Dark Mode feature)
   - Merge into `main`
   - Create Annotated tag:
     ```bash
     git tag -a v1.1.0 -m "Minor release - Added Dark Mode"
     ```

4. **Bug Fix (v1.1.1)**
   - Switch to `bugfix/login-issue`
   - Make **1 commit** (example: Fixed login redirect)
   - Merge into `main`
   - Create Annotated tag:
     ```bash
     git tag -a v1.1.1 -m "Patch release - Fixed login redirect issue"
     ```

---

## Part C: Push to GitHub

1. Push the `main` branch:
   ```bash
   git push origin main
   ```

2. Push all the annotated tags:
   ```bash
   git push origin v1.0.0
   git push origin v1.1.0
   git push origin v1.1.1
   ```

   **OR**

   ```bash
   git push origin --tags
   ```

---

## Part D: Create GitHub Releases

1. Go to your repository on GitHub.
2. Click on **Releases** → **Draft a new release**.
3. Create releases for the following tags:

   | Tag     | Release Title                        |
   |---------|--------------------------------------|
   | v1.0.0  | v1.0.0 – First Stable Release        |
   | v1.1.0  | v1.1.0 – Dark Mode Added             |
   | v1.1.1  | v1.1.1 – Login Bug Fix               |

4. Add a short description for each release.

---

## Submission Requirements

Submit the following:

1. Screenshot of `git tag` command (showing all tags)
2. Screenshot of `git show v1.0.0`
3. Screenshot of `git log --oneline --decorate --graph --all`
4. Link to your GitHub repository
5. Screenshots of the three GitHub Releases you created

---

## Evaluation Criteria

| Criteria                              | Marks |
|---------------------------------------|-------|
| Lightweight tags created correctly    | 10    |
| Annotated tags created correctly      | 20    |
| Proper Semantic Versioning used       | 15    |
| Tags pushed to GitHub                 | 15    |
| GitHub Releases created               | 20    |
| Screenshots + Repository link         | 20    |
| **Total**                             | 100   |

---

**Note:**  
- Use only **Annotated tags** for versions `v1.0.0`, `v1.1.0`, and `v1.1.1`.
- Make sure your commit messages are clear and meaningful.

---

### Deadline - 13th September, 2026
