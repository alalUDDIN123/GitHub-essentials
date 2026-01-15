
# 🚀 GitHub Complete Setup Guide (Windows Only)

---

## 1️⃣ What is **GitHub** & why all developers use it

### What GitHub is

* GitHub is a **cloud platform for hosting Git repositories**
* It helps developers:

  * Store code
  * Track changes
  * Collaborate with teams
* Built on **Git (version control system)**

### Why almost every developer uses GitHub

* ✅ Industry standard (startups → big companies)
* ✅ Team collaboration & code review
* ✅ Open-source learning
* ✅ Portfolio for jobs
* ✅ CI/CD automation
* ✅ Backup + history of code

👉 **If you are a developer and not on GitHub, you are invisible.**

---

## 2️⃣ Create & Set Up a GitHub Account

### Steps

1. Go to github.com
2. Sign up with:

   * Professional username
   * Valid email
3. Verify email
4. Complete profile:

   * Profile photo
   * Bio (tech stack)
   * Location (optional)

### Important Settings (Must Do)

* Enable **Two-Factor Authentication (2FA)**
* Set email privacy
* Later: add SSH key

---

## 3️⃣ Understand GitHub Interface (What to know)

### Key GitHub Features

* Repositories – store code
* Issues – bugs / tasks
* Pull Requests – code review & merge
* Actions – CI/CD automation
* Projects – task management
* Wiki – documentation
* Discussions – team/community talk

---

### Important Navigation Links

#### 🔹 Profile

* Contribution graph
* Repositories
* Pinned projects
* Your **developer identity**

#### 🔹 Settings

* Account & security
* SSH & GPG keys
* Permissions

#### 🔹 Create Repository

* Public / Private
* README.md
* .gitignore
* License

#### 🔹 Pull Requests

* Propose code changes
* Review & merge
* Core of team workflow

#### 🔹 Actions

* Automated build, test, deploy

#### 🔹 Collaborate

* Add contributors
* Permission control

#### 🔹 Projects

* Kanban-style task boards

---

## 4️⃣ Install Git on Windows (FIRST REQUIREMENT)

### Download & Install

* [Install Git for Windows](https://git-scm.com/install/windows)
* During install:

  * Use **Git from command line**
  * Use **default editor or VS Code**

### Verify

```bash
git --version
```

✅ If version appears → OK

---

## 5️⃣ Install GitHub CLI on Windows (VERY IMPORTANT)

### What is **GitHub CLI (`gh`)**

* Official GitHub command-line tool
* Used to manage:

  * Repos
  * Pull requests
  * Issues
  * Auth

---

### Installation (Recommended Way)

#### Option 1: Using Winget (Best)

Open **PowerShell (Admin)**:

```powershell
winget install --id GitHub.cli
```

#### Option 2: Using Chocolatey

```powershell
choco install gh
```

---

### Verify Installation

```bash
gh --version
```

✅ If version shows → installed correctly
❌ If `gh not found` → restart terminal / VS Code

---

## 6️⃣ Authenticate GitHub CLI (Login)

Now run:

```bash
gh auth login
```

### Choose options

* GitHub.com
* HTTPS or SSH (SSH recommended)
* Login via browser (easy)

Check status:

```bash
gh auth status
```

---

## 7️⃣ Connect GitHub with VS Code (Windows)

### Method 1: Automatic (Best)

* Open VS Code
* It detects `gh`
* GitHub integration works automatically

### Method 2: Manual

* Command Palette → `GitHub: Sign in`
* Uses CLI authentication

---

## 8️⃣ Core Git Commands (Must Know)

### Basic Commands

```bash
git init
git clone <repo-url>
git status
git add .
git commit -m "message"
git log
```

### Branching

```bash
git branch
git checkout -b new-branch
git merge
git rebase
```

### GitHub (Remote)

```bash
git remote -v
git push origin main
git pull origin main
```

### Collaboration

```bash
git fetch
git diff
git stash
```

---

## 9️⃣ Core GitHub CLI (`gh`) Commands

```bash
gh repo create
gh repo clone
gh pr create
gh pr list
gh issue create
gh auth status
```

---

## 🔟 Recommended Professional Setup (Windows)

### SSH Setup (One-Time)

```bash
ssh-keygen -t ed25519 -C "your_email"
gh ssh-key add ~/.ssh/id_ed25519.pub
```

✅ Benefits:

* No password prompts
* Secure
* Industry standard

---

## 🔚 Correct Order (IMPORTANT)

- 1️⃣ Install Git
- 2️⃣ Create GitHub account
- 3️⃣ Install GitHub CLI (`gh`)
- 4️⃣ `gh auth login`
- 5️⃣ Connect VS Code
- 6️⃣ Start pushing code 🚀

---
