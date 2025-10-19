# 🌱 Complete Git & GitHub Workflow Guide

This guide explains everything — from working locally to pushing your code to GitHub, creating branches, and collaborating with others.  

---

## 🧩 1. What is Git?

Git is a **Version Control System (VCS)** — it helps you track changes in your code over time.

- You can save checkpoints (commits)
- Revert to older versions
- Work with others on the same project without overwriting their work

When you initialize Git in a folder, a hidden `.git` folder is created that stores all commit history, branches, and metadata.

```bash
git init


The folder structure- 
my_project/
│
├── demo.py
└── .git/   ← hidden folder that stores all version control info


fron local to git
create a project and initialize the git
mkdir demo-project
cd demo-project
git init


add files and commit changes
echo 'print("Hello World")' > demo.py
git add demo.py
git commit -m "Initial commit"

connect git to github
git remote add origin https://github.com/<your-username>/demo-project.git
git branch -M main
git push -u origin main


branching
git checkout main
git pull origin main               # ensure latest version
git checkout -b feature/add-age    # create and switch to new branch


create a pull request


