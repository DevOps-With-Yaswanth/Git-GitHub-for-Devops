# 🚀 Git & GitHub Fundamentals

> Welcome to the world of Version Control Systems.
> Before learning Git commands, every DevOps Engineer must understand **why Git was created** and **what problems it solves**.

---

# 📚 Module 01 - Introduction to Git & GitHub

## 🎯 Learning Objectives

After completing this module, you will be able to:

✅ Understand Version Control Systems

✅ Understand problems without Version Control

✅ Differentiate Local, Centralized, and Distributed VCS

✅ Understand Git Architecture

✅ Understand Git Workflow

✅ Differentiate Git and GitHub

---

# 🤔 Why Do We Need Version Control?

Imagine you are working on a project called:

```text
project-final.zip
```

After making changes:

```text
project-final-final.zip
```

Again:

```text
project-final-final-v2.zip
```

Again:

```text
project-final-latest-final-v3.zip
```

After a few weeks:

```text
project-final-final-v2-latest-updated-new.zip
```

😂 Sounds familiar?

Without Version Control:

❌ Files get duplicated

❌ No history tracking

❌ Difficult collaboration

❌ Accidentally overwrite files

❌ Impossible to know who changed what

❌ Hard to restore previous versions

---

# 📖 What is Version Control?

A Version Control System (VCS) is a tool that tracks changes made to files over time.

It allows developers to:

* Save versions of code
* Track history
* Restore previous versions
* Collaborate with teams
* Manage software projects efficiently

---

## 🎯 Simple Example

### Version 1

```python
print("Hello")
```

### Version 2

```python
print("Hello World")
```

### Version 3

```python
print("Hello DevOps")
```

Instead of saving multiple files:

```text
app-v1.py
app-v2.py
app-v3.py
```

Git stores all changes efficiently and allows switching between versions anytime.

---

# 😟 Problems Without Version Control

| Problem              | Description                  |
| -------------------- | ---------------------------- |
| File Duplication     | Multiple copies of same file |
| No History           | Cannot track changes         |
| Collaboration Issues | Team members overwrite code  |
| Backup Problems      | Previous versions lost       |
| No Rollback          | Cannot restore old versions  |
| Manual Tracking      | Time consuming               |

---

# 🏗️ Types of Version Control Systems

There are three major types:

```text
Version Control Systems
│
├── Local VCS
├── Centralized VCS
└── Distributed VCS
```

---

# 1️⃣ Local Version Control System

All versions are stored on a single computer.

```text
+----------------+
| Developer PC   |
|                |
| Version 1      |
| Version 2      |
| Version 3      |
+----------------+
```

### Advantages

✅ Simple

### Disadvantages

❌ No collaboration

❌ No backup

❌ Single point of failure

---

# 2️⃣ Centralized Version Control System (CVCS)

A central server stores all code.

```text
              +-------------+
              | Central     |
              | Repository  |
              +-------------+
                    ▲
                    │
      ┌─────────────┼─────────────┐
      │             │             │
      ▼             ▼             ▼

 Developer A   Developer B   Developer C
```

### Examples

* SVN
* CVS

### Advantages

✅ Team collaboration

✅ Centralized management

### Disadvantages

❌ Server failure affects everyone

❌ Requires network connectivity

❌ Single point of failure

---

# 3️⃣ Distributed Version Control System (DVCS)

Every developer has a complete copy of the repository.

```text
            +----------------+
            | Remote Repo    |
            +----------------+
                 ▲      ▲
                 │      │
                 │      │
      ┌──────────┘      └──────────┐
      ▼                            ▼

+--------------+          +--------------+
| Developer A  |          | Developer B  |
| Full Copy    |          | Full Copy    |
+--------------+          +--------------+
```

### Examples

* Git
* Mercurial

### Advantages

✅ Fast

✅ Offline work

✅ Full backup available

✅ No single point of failure

✅ Better collaboration

---

# 🎉 What is Git?

Git is a Distributed Version Control System created by:

**Linus Torvalds**

Creator of Linux.

Git helps developers:

* Track changes
* Collaborate
* Manage versions
* Restore previous states
* Maintain project history

---

# 🏛️ Git Architecture

Git consists of three major areas:

```text
Working Directory
       │
       ▼
 Staging Area
       │
       ▼
 Local Repository
```

---

## Working Directory

This is where files are created and modified.

Example:

```text
app.py
index.html
Dockerfile
```

---

## Staging Area

Temporary area where changes are prepared before committing.

Think of it as:

```text
Draft Area
```

---

## Local Repository

Permanent storage of commits on your machine.

Every commit creates a checkpoint.

```text
Commit 1
Commit 2
Commit 3
```

---

# 🔄 Git Workflow

```text
Create File
     │
     ▼
Modify File
     │
     ▼
Stage Changes
     │
     ▼
Commit Changes
     │
     ▼
Push to Remote Repository
```

---

## Visual Workflow

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
       │
 git push
       ▼
 Remote Repository
```

---

# ⚔️ Git vs GitHub

Many beginners think both are same.

They are NOT.

| Feature             | Git                    | GitHub                |
| ------------------- | ---------------------- | --------------------- |
| Type                | Version Control System | Code Hosting Platform |
| Installation        | Installed Locally      | Web Platform          |
| Purpose             | Track Changes          | Store & Collaborate   |
| Works Offline       | Yes                    | No                    |
| Created By          | Linus Torvalds         | GitHub Company        |
| Repository Location | Local Machine          | Cloud                 |

---

## Easy Analogy

Think about:

```text
Git     = Microsoft Word

GitHub  = Google Drive
```

### Git

Creates and manages your work.

### GitHub

Stores and shares your work.

---

# 🎯 Real-World DevOps Usage

Git is used for:

* Source Code Management
* Infrastructure as Code
* CI/CD Pipelines
* Kubernetes Manifests
* Dockerfiles
* Terraform Code
* Automation Scripts

Every modern DevOps tool integrates with Git.

---

# 📝 Key Takeaways

✅ Git is a Distributed Version Control System

✅ Git tracks file changes

✅ Git stores project history

✅ Git enables collaboration

✅ Git works offline

✅ GitHub hosts Git repositories online

✅ Every DevOps Engineer must master Git

---

Happy Learning! 🎉
