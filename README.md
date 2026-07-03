# 🚀 Git & GitHub Setup Guide (Windows)

This guide will help you install Git, configure your Git account, connect a local project to GitHub, and push your code.

---

# Step 1: Install Git

Download and install Git for Windows:

https://git-scm.com/install/windows

After installation, open **Git Bash**.

---

# Step 2: Configure Git

> If you already have an old Git configuration, remove it first.

Run the following commands:

```bash
git config --global --unset user.name
git config --global --unset user.email
```

Now set your Git username and email.

```bash
git config --global user.name "sanjaynakum089-hub"
git config --global user.email "sanjaynakum089@gmail.com"
```

---

# Step 3: Verify Git Configuration

Run:

```bash
git config --list
```

Make sure the output contains your correct:

- Username
- Email Address

You can also check individually:

```bash
git config --global user.name
git config --global user.email
```

---

# Step 4: Create a Project

Create a new project folder.

Example:

```
News_Website
```

Open the project in **Visual Studio Code**.

---

# Step 5: Initialize Git

Open the VS Code Terminal and run:

```bash
git init
```

---

# Step 6: Create a GitHub Repository

1. Login to GitHub.
2. Click the **New Repository** button.
3. Enter a repository name.

Example:

```
News-Website
```

4. Click **Create Repository**.

---

# Step 7: Connect Local Project to GitHub

Copy the command provided by GitHub.

It will look similar to:

```bash
git remote add origin https://github.com/USERNAME/News-Website.git
```

Paste it into your terminal.

To verify:

```bash
git remote -v
```

---

# Step 8: Add Your Files

Create, edit, or delete files inside your project.

---

# Step 9: Commit Your Changes

Stage all files:

```bash
git add .
```

Create a commit:

```bash
git commit -m "Initial commit"
```

---

# Step 10: Push to GitHub

Check your current branch:

```bash
git branch
```

If your branch is **main**, run:

```bash
git push -u origin main
```

If your branch is **master**, run:

```bash
git push -u origin master
```

---

# Daily Workflow

Whenever you make changes:

```bash
git add .
git commit -m "Describe your changes"
git push origin main
```

Repeat this process every time you update your project.

---

# Useful Git Commands

## Check Status

```bash
git status
```

## View Commit History

```bash
git log
```

## View Current Branch

```bash
git branch
```

## Check Remote Repository

```bash
git remote -v
```

## Pull Latest Changes

```bash
git pull origin main
```

---

# Common Git Workflow

```text
Create Project
      │
      ▼
git init
      │
      ▼
Create GitHub Repository
      │
      ▼
git remote add origin <repository-url>
      │
      ▼
Create / Edit Files
      │
      ▼
git add .
      │
      ▼
git commit -m "Commit message"
      │
      ▼
git push origin main
      │
      ▼
Repeat
```

---

# Notes

- Install Git only once.
- Configure your username and email only once.
- Always check your current branch before pushing.
- Commit frequently with meaningful commit messages.
- Push your code regularly to keep GitHub updated.

---

## Happy Coding! 🎉
