# 🚀 Module 02 - Git Setup and First Repository

---

# 🎯 Learning Objectives

After completing this module, you will be able to:

✅ Install Git

✅ Create a GitHub Account

✅ Configure Git

✅ Create Git Repositories

✅ Understand the `.git` folder

✅ Clone repositories

✅ Add files to Git

✅ Create commits

✅ Push code to GitHub

✅ View commit history

---

# 1️⃣ Git Download and Installation

## What is Git?

Git is a Distributed Version Control System that tracks changes in your code.

---

## Download Git

### Windows

https://git-scm.com/download/win

### Linux (Ubuntu)

```bash
sudo apt update
sudo apt install git -y
```

### Verify Installation

```bash
git --version
```

Example:

```bash
git version 2.49.0
```

---

# 2️⃣ GitHub Signup

## What is GitHub?

GitHub is a cloud platform used to store Git repositories and collaborate with other developers.

---

## Create an Account

1. Visit https://github.com
2. Click Sign Up
3. Enter:

* Email
* Username
* Password

4. Verify your email.

---

# 3️⃣ Git Configuration

Before using Git, we need to tell Git who we are.

---

## Configure Username

```bash
git config --global user.name "Yaswanth Sai"
```

---

## Configure Email

```bash
git config --global user.email "your-email@gmail.com"
```

---

## Check Configuration

```bash
git config --list
```

---

## Why is this required?

Whenever you create a commit, Git stores:

* Author Name
* Email
* Timestamp
* Commit Message

Every commit becomes part of the project's history.

---

# 4️⃣ Create Repository Using GitHub UI

## Step 1

Login to GitHub.

---

## Step 2

Click:

```text
New Repository
```

---

## Step 3

Enter:

| Field           | Example      |
| --------------- | ------------ |
| Repository Name | demo-project |
| Visibility      | Public       |
| README          | Optional     |

---

## Step 4

Click:

```text
Create Repository
```

---

# Repository Created 🎉

---

# 5️⃣ Create Repository Using CLI

Create a project folder.

```bash
mkdir demo-project
cd demo-project
```

Initialize Git.

```bash
git init
```

Output:

```text
Initialized empty Git repository
```

---

# What does `git init` do?

It creates a hidden folder called:

```text
.git
```

This folder converts a normal directory into a Git repository.

---

# 6️⃣ Understanding the `.git` Folder

View hidden files.

```bash
ls -la
```

You will see:

```text
.git
```

---

# Why is `.git` Important?

Everything Git knows about your project is stored inside this folder.

---

# `.git` Architecture

```text
.git
│
├── HEAD
├── config
├── objects
├── refs
├── hooks
├── logs
└── index
```

---

# Important Files

| File    | Purpose                  |
| ------- | ------------------------ |
| HEAD    | Current branch           |
| config  | Repository configuration |
| objects | Stores commits and files |
| refs    | Branch references        |
| index   | Staging area information |
| logs    | History of references    |

---

# Interview Question

### Can we delete the `.git` folder?

Yes.

But after deleting it:

❌ Commit history is lost.

❌ Branches disappear.

❌ Repository becomes a normal folder.

---

# 7️⃣ Git Clone

## What is Cloning?

Copying an existing repository from GitHub to your local machine.

---

## Syntax

```bash
git clone <repository-url>
```

Example:

```bash
git clone https://github.com/user/demo-project.git
```

---

# What happens internally?

```text
GitHub Repository
        │
        ▼
 Download Repository
        │
        ▼
 Create Local Copy
        │
        ▼
 Configure Remote Origin
```

---

# 8️⃣ Git Add

## Purpose

Moves changes from:

```text
Working Directory
        │
        ▼
    Staging Area
```

---

## Add Single File

```bash
git add file.txt
```

---

## Add All Files

```bash
git add .
```

---

# Why do we need `git add`?

Because Git allows us to choose exactly which files should be included in the next commit.

---

# Real-Life Analogy

```text
Working Directory = Kitchen

Staging Area = Plate

Commit = Serving Food
```

You first prepare food.

Then place it on the plate.

Then serve it.

---

# 9️⃣ Git Commit

## Purpose

Creates a permanent snapshot of your code.

---

## Syntax

```bash
git commit -m "Initial Commit"
```

---

# What is a Commit?

A commit is a checkpoint.

```text
Commit 1
Commit 2
Commit 3
```

You can return to any checkpoint later.

---

# Why is Commit Important?

Without commits:

❌ No history

❌ No rollback

❌ No collaboration

❌ No tracking

---

# Internally

```text
Working Directory
       │
git add
       ▼
Staging Area
       │
git commit
       ▼
Local Repository
```

---

# 🔟 Git Push

## Purpose

Uploads commits to GitHub.

---

## Syntax

```bash
git push origin main
```

---

# Internally

```text
Local Repository
       │
git push
       ▼
GitHub Repository
```

---

# What does `origin` mean?

```text
origin = Remote Repository Name
```

---

# What does `main` mean?

```text
main = Branch Name
```

---

# 1️⃣1️⃣ Git Log

## Purpose

Shows commit history.

---

## Command

```bash
git log
```

---

## One Line Format

```bash
git log --oneline
```

Example:

```text
8f35d2a Initial Commit
54e45ab Added README
97de78c Added Dockerfile
```

---

# Why is Git Log Important?

✅ Shows commit history

✅ Shows who made changes

✅ Shows timestamps

✅ Helps debugging

---

# Complete Workflow

```text
Create File
      │
      ▼
git add
      │
      ▼
Staging Area
      │
      ▼
git commit
      │
      ▼
Local Repository
      │
      ▼
git push
      │
      ▼
GitHub Repository
```

---

# Commands Covered in This Module

| Command       | Purpose               |
| ------------- | --------------------- |
| git --version | Verify installation   |
| git config    | Configure Git         |
| git init      | Initialize repository |
| git clone     | Copy repository       |
| git add       | Stage changes         |
| git commit    | Create snapshot       |
| git push      | Upload to GitHub      |
| git log       | View history          |

---

