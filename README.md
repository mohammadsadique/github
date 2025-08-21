# 🚀 Github

🔑 Git Credential Helper
---

#### GitHub Setup & Credential Management

When working with GitHub across multiple projects or accounts, it’s important to configure credentials properly.  
Git provides a **Credential Helper** to store and manage your login details securely, so you don’t have to enter them every time.

You can store credentials at either **project level** or **global level**:

#### 1. Project-specific (only for the current repository)
```bash
git config credential.helper store
```

#### 2. Global (applies to all repositories on your machine)
```bash
git config --global credential.helper store
```

#### 👤 Configuring Git User
```bash
git config user.name
```
```bash
git config user.email
```

---
Fetch All Branch From Server
---
When you need to work on a branch that exists on the remote repository but not yet in your local system, you must first fetch it from the server. Once fetched, you can check it out locally and start working.

#### 1️⃣ Fetch all remote branches
This command updates your local repository with the latest references from the remote without merging them into your local branches:
```bash
git fetch --all
```

#### 2️⃣ List available remote branches
After fetching, you can list all branches that exist on the remote:
```bash
git branch -r
```

#### 3️⃣ Check out a remote branch locally
To work on a remote branch (example: `fix-capture-image`), first create a local branch that tracks it:
```bash
git checkout -b fix-capture-image origin/fix-capture-image
```

🔹 fix-capture-image → name of your new local branch

🔹 origin/develop → remote branch you are tracking

💡 After this, your local branch will stay connected to the remote branch, so you can pull the latest changes or push your updates directly.

![App Screenshot](https://raw.githubusercontent.com/mohammadsadique/github/refs/heads/main/fetch-all-branch.png)





---
---
---


# Git Document  
The simplest way to learn Git 🚀  

## 1. Install Git  
Download and install Git from the official site:  
👉 [Git Download](https://git-scm.com/downloads)  

After installation, right-click you will see:  
- **Git GUI Here**  
- **Git Bash Here**  

Click **Git Bash Here** to open the terminal and check the version:  

```bash
git --version
```

## 2. First-Time Setup
Before using Git, configure your name and email.

**Add Your Name**
```bash
git config user.name "yourname"          # Specific Project  
git config --global user.name "yourname" # All Projects  
```

**Add Your Email**
```bash
git config user.email "example@example.com"          # Specific Project  
git config --global user.email "example@example.com" # All Projects  
```

## 3. Initialize Git Repository
Navigate to your project folder and initialize Git:
```bash
git init
```

## 4. Git Workflow (4 Steps)
  1. Untracked File
  2. Staged Area
  3. Commit Files
  4. Status

### Step 1: Untracked File
When you create a new file, Git marks it as untracked. Check untracked files:
```bash
git status
```

### Step 2: Staged Area
Add files to the staging area.
```bash
git add index.html   # Single file  
git add -A           # All files  
git add .            # New + Modified files (not deleted)  
git add -u           # Modified + Deleted files (not new)  
```

### Step 3: Commit Files
Commit saves your work in Git history.
```bash
git commit           # Opens editor to write commit message  
git commit -m "Your message here"  
git commit -a -m "Commit all tracked changes with message"
```
💡 In the editor, type your message, then press: 
Esc + :wq + Enter to save and exit.

### Step 4: Status
Check the current state of your repository:
```bash
git status
```



---








