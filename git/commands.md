# 🚀 Git Notes (Beginner → DevOps Level)

## 📌 What is Git?
Git is a distributed version control system used to track changes in code and collaborate with teams.

---

## 🧱 Basic Git Workflow

1. Initialize repository  
2. Add files  
3. Commit changes  
4. Push to remote  
5. Pull updates  

---

## ⚙️ Git Commands with Explanation

### 🔹 Initialize Repository
git init  
➡️ Creates a `.git` folder and starts tracking your project

---

### 🔹 Check Status
git status  
➡️ Shows modified, staged, and untracked files

---

### 🔹 Add Files (Staging)
git add .  
➡️ Adds all files to staging area

git add filename  
➡️ Adds a specific file

---

### 🔹 Commit Changes
git commit -m "your message"  
➡️ Saves a snapshot of your code

---

### 🔹 Set Main Branch (First Time)
git branch -M main  
➡️ Renames default branch to `main`

---

### 🔹 Connect to Remote Repository
git remote add origin git@github.com:username/repo-name.git  
➡️ Links local repo to GitHub

---

### 🔹 Push Code (First Time)
git push -u origin main  
➡️ Uploads code and sets upstream branch

---

### 🔹 Push Changes (Daily Use)
git push  
➡️ Sends latest commits to remote

---

### 🔹 Pull Latest Changes
git pull origin main  
➡️ Downloads latest code from remote

---

## 🌿 Branching (Important)

### Create New Branch
git checkout -b feature-branch  

➡️ Used for new features or changes

---

### Switch Branch
git checkout main  

---

### Merge Branch
git merge feature-branch  

➡️ Combines changes into main branch

---

## 📜 View History
git log  
➡️ Shows commit history

---

## 🧹 Undo Staging
git reset  
➡️ Removes files from staging area

---

## 🔁 Real Daily Workflow

git pull  
git add .  
git commit -m "your message"  
git push  

---

## ⚠️ Common Errors

### ❌ Push rejected
git pull --rebase origin main  
git push  

---

### ❌ Authentication error
➡️ Use SSH instead of HTTPS  
➡️ GitHub does not support password login

---

## 💡 Pro Tips

- Always pull before pushing
- Use meaningful commit messages
- Use branches for features
- Use SSH for authentication
- Keep commits small and clean

---

## 🎯 Summary

| Command | Purpose |
|--------|--------|
| git init | Start repo |
| git add | Stage changes |
| git commit | Save changes |
| git push | Upload code |
| git pull | Get latest code |

---

## 🚀 Goal

This Git knowledge is essential for:
- CI/CD pipelines
- Collaboration
- DevOps workflows