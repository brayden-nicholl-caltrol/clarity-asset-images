# GitHub Upload Instructions

A quick guide for uploading changes from a **OneDrive-synced folder** to a GitHub repository using PowerShell.

## 🔄 Upload Workflow

```text
┌─────────────────────────────┐
│  Edit or create files       │
│  in your OneDrive folder    │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│  Navigate to repository     │
│  folder in PowerShell       │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│  git add .                  │
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│  git commit -m "Description"│
└──────────────┬──────────────┘
               ↓
┌─────────────────────────────┐
│  git push                   │
└──────────────┬──────────────┘
               ↓
        ┌──────────────┐
        │   GitHub 🚀  │
        └──────────────┘
```

## 🛠️ PowerShell Commands

### 1. Navigate to the Repository

Open **PowerShell** and navigate to your OneDrive repository folder:

```powershell
cd "path\to\OneDrive\folder"
```

### 2. Check Your Changes

Before uploading anything, check which files have been added or modified:

```powershell
git status
```

### 3. Stage Your Changes

Add all new and modified files:

```powershell
git add .
```

### 4. Commit Your Changes

Create a commit with a short description of what you changed:

```powershell
git commit -m "Description"
```

For example:

```powershell
git commit -m "Add data processing script"
```

### 5. Push to GitHub

Upload your committed changes to GitHub:

```powershell
git push
```

## ✅ Complete Example

The entire process can be performed with:

```powershell
cd "C:\Users\YourName\OneDrive\Documents\MyProject"

git status
git add .
git commit -m "Add new files"
git push
```

> **Tip:** Run `git status` before committing to make sure you're only uploading the changes you intended.

---

### 📌 Quick Reference

| Command                   | Purpose                     |
| ------------------------- | --------------------------- |
| `cd "path"`               | Navigate to your repository |
| `git status`              | View changed/new files      |
| `git add .`               | Stage all changes           |
| `git commit -m "Message"` | Save changes to Git history |
| `git push`                | Upload commits to GitHub    |

**OneDrive** keeps your local files synchronized across your devices, while **Git** handles version control and synchronization with **GitHub**.
