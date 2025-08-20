# Github

### GitHub Setup & Credential Management

When working with GitHub across multiple projects or accounts, it’s important to configure credentials properly.  
Git provides a **Credential Helper** to store and manage your login details securely, so you don’t have to enter them every time.

---

#### 🔑 Git Credential Helper

You can store credentials at either **project level** or **global level**:

### 1. Project-specific (only for the current repository)
```bash
git config credential.helper store
```

### 2. Global (applies to all repositories on your machine)
```bash
git config --global credential.helper store
```

### 👤 Configuring Git User
```bash
git config user.name
git config user.email
```
