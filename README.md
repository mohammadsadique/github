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





