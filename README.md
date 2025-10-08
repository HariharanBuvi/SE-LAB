# 🧪 Git Lab Experiment – Exploring Git Commands

**Author:** Hariharan R  
**Course:** Software Engineering Lab  
**IDE Used:** Visual Studio Code  
**Version Control System:** Git & GitHub  
**Date:** October 2025  

---

## 🎯 AIM
To explore and practice real-world **Git and GitHub** workflows — including repository creation, staging, committing, branching, pushing, merging, resolving conflicts, and contributing via forks and pull requests.

---

## 📘 OBJECTIVES
- Understand Git as a distributed version control system.  
- Learn to initialize, stage, and commit changes locally.  
- Practice creating and switching between branches.  
- Push and pull code between local and remote repositories.  
- Resolve merge conflicts manually.  
- Create and merge pull requests in GitHub.  
- Fork repositories and contribute to open-source projects.

---

## 🗂️ PROJECT OVERVIEW
This experiment uses a simple interactive web page named **`index.html`** that displays  
`<h1>Hello from Hariharan!</h1>` and other content demonstrating Git workflow.  
Each modification to the file represents a **Git commit or feature branch update**.

---

## 🧠 THEORY

**Git** is a distributed version control system used to track changes in source code during software development.  
**GitHub** is a cloud-based hosting service for Git repositories that allows collaboration and contribution.  

Key Git areas:
- **Working Directory** → Your local files  
- **Staging Area** → Prepared files for commit  
- **Repository** → Permanent history of commits  

---

## ⚙️ PROCEDURE & COMMANDS

### 🧩 Step 1: Initialize a Repository
Open VS Code and the project folder, then run:
```bash
git init
````

This creates a local Git repository in your folder.

---

### 🧩 Step 2: Configure User Information

```bash
git config --global user.name "Hariharan"
git config --global user.email "your_email@example.com"
git config --list
```

This identifies your commits.

---

### 🧩 Step 3: Add and Commit Files

Create the main file:

```bash
echo "<h1>Hello from Hariharan!</h1>" > index.html
git status
git add index.html
git commit -m "Initial commit - added index.html"
```

To view commit history:

```bash
git log --oneline
```

---

### 🧩 Step 4: Connect to GitHub

1. Create a new GitHub repository named **git-lab**.
2. Copy the repository’s HTTPS link.
3. Connect and push:

```bash
git remote add origin https://github.com/your-username/git-lab.git
git branch -M main
git push -u origin main
```

---

### 🧩 Step 5: Create and Work on a New Branch

```bash
git checkout -b feature-hariharan
```

Modify your `index.html` (add new section or style)
Then:

```bash
git add .
git commit -m "Added new feature section"
git push origin feature-hariharan
```

---

### 🧩 Step 6: Create a Pull Request

1. Go to your GitHub repository.
2. Click **Compare & Pull Request** → add details → submit.
3. After review, **merge** it into `main`.

---

### 🧩 Step 7: Handle Merge Conflicts

If a teammate edited the same section:

```bash
git pull origin main
```

Conflicts appear like this:

```
<<<<<<< HEAD
Your code
=======
Other code
>>>>>>> main
```

Fix manually → save →

```bash
git add .
git commit -m "Resolved merge conflict"
git push origin feature-hariharan
```

Then merge again on GitHub.

---

### 🧩 Step 8: Merge Branches Locally

```bash
git checkout main
git merge feature-hariharan
git push origin main
```

---

### 🧩 Step 9: Fork and Contribute

1. Go to another repo → Click **Fork**
2. Clone your fork:

   ```bash
   git clone https://github.com/your-username/original-repo.git
   ```
3. Make a small edit → Commit & push:

   ```bash
   git add .
   git commit -m "Added footer/comment"
   git push origin main
   ```
4. Create a **Pull Request** to merge back to the original repo.

---

## 🔧 ADDITIONAL GIT COMMANDS

| Command                                | Purpose                             |
| -------------------------------------- | ----------------------------------- |
| `git status`                           | Show changed files and branch info  |
| `git diff`                             | Show unstaged differences           |
| `git restore <file>`                   | Undo changes before committing      |
| `git branch -a`                        | List all branches                   |
| `git merge <branch>`                   | Merge specified branch into current |
| `git log --graph --oneline --decorate` | Show visual commit tree             |
| `git stash` / `git stash pop`          | Temporarily save and restore work   |
| `git tag v1.0`                         | Mark version milestone              |
| `git push origin --tags`               | Push all tags to GitHub             |

---

## 📁 FOLDER STRUCTURE

```
git-lab/
│
├── index.html
├── README.md
└── .git/ (auto-created by git)
```

---

## 📸 SCREENSHOTS TO INCLUDE (for lab record)

1. Output of `git init`
2. Output of `git add .` and `git commit -m`
3. Push to GitHub (screenshot of repo page)
4. Branch creation and merge
5. Merge conflict and resolution
6. Pull Request screenshot
7. Fork and contribution page

---

## 💻 SAMPLE OUTPUT (from index.html)

```
Hello from Hariharan! 👋
Welcome to my Git Lab Experiment Project.
Git Features Practiced:
- git init
- git add .
- git commit -m "message"
- git push
- git pull
- git merge
- git checkout -b branch
```

---

## ✅ RESULT

Thus, the Git experiment was successfully executed using VS Code and GitHub.
All major Git commands were practiced — including initialization, staging, committing, pushing, branching, merging, resolving conflicts, and contributing via forks.

---

## 🏁 CONCLUSION

Through this experiment, we learned:

* How Git maintains version history efficiently
* How collaboration happens using GitHub
* How to fix merge conflicts and manage branches effectively
* How developers work together in real-world projects

---

## 🧩 REFERENCES

* [Official Git Documentation](https://git-scm.com/doc)
* [GitHub Guides](https://guides.github.com)
* [Pro Git Book](https://git-scm.com/book/en/v2)

---

> *“Commit your progress, merge your ideas, and push your limits.”* 💻✨
> — *Hariharan R*

```

---

✅ **How to use it:**
1. Create a new file in VS Code → name it `README.md`  
2. Paste the above content  
3. Save it → it will appear formatted perfectly on your GitHub repo page.  

Would you like me to also generate a **Word version (`README.docx`)** with screenshots placeholders (for submission to college)?
```
