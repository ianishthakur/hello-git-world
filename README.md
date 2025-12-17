# 🚀 Git Workshop - GDG Kathmandu × HECC

Welcome to the hands-on Git Workshop! In this session, you'll learn Git by actually creating and resolving merge conflicts.

---

## 📋 Workshop Overview

| Detail | Info |
|--------|------|
| **Event** | Git Live Demo Session |
| **Organizer** | GDG Kathmandu |
| **Venue** | Himalaya Electronics & Computer Club (HECC) |
| **Participants** | B.Tech Students |

---

## 🎯 What You'll Learn

- Clone a repository
- Create and switch branches
- Make changes and commit
- Push to remote repository
- Create Pull Requests
- **Understand and resolve merge conflicts!**

---

## 🛠️ Prerequisites

Make sure you have:

- [ ] Git installed on your system
- [ ] A GitHub account
- [ ] A code editor (VS Code recommended)

### Quick Git Installation Check

```bash
git --version
```

If not installed, download from: <https://git-scm.com/downloads>

---

## 📝 Step-by-Step Instructions

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/git-workshop.git
cd git-workshop
```

### Step 2: Create Your Branch

Create a branch with your name (use lowercase, no spaces):

```bash
git checkout -b your-name
```

**Example:**

```bash
git checkout -b ram-sharma
```

### Step 3: Open the HTML File

Open `index.html` in your code editor and find this section (around line 96):

```html
<!-- 🔥 CHANGE THIS LINE TO CREATE A CONFLICT! 🔥 -->
<span class="participant-name">Anish</span>
```

### Step 4: Change the Name

Replace `Anish` with **YOUR name**:

```html
<span class="participant-name">Ram Sharma</span>
```

### Step 5: Stage and Commit Your Changes

```bash
git add .
git commit -m "Added my name - Ram Sharma"
```

### Step 6: Push Your Branch

```bash
git push origin your-branch-name
```

**Example:**

```bash
git push origin ram-sharma
```

### Step 7: Create a Pull Request

1. Go to the repository on GitHub
2. Click "Compare & pull request"
3. Add a title: "Added my name - Your Name"
4. Click "Create pull request"

---

## 💥 Understanding Merge Conflicts

When multiple people change the **same line** of code, Git doesn't know which change to keep. This creates a **merge conflict**.

### What a Conflict Looks Like

```html
<<<<<<< HEAD
<span class="participant-name">Anish</span>
=======
<span class="participant-name">Ram Sharma</span>
>>>>>>> ram-sharma
```

### How to Read This

- `<<<<<<< HEAD` → The current content in main branch
- `=======` → Separator between conflicting changes  
- `>>>>>>> branch-name` → Your changes

### Resolving the Conflict

1. **Open the file** with the conflict
2. **Decide** which change to keep (or combine them)
3. **Remove** the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)
4. **Save** the file
5. **Stage and commit** the resolution:

```bash
git add .
git commit -m "Resolved merge conflict"
```

---

## 🔧 Useful Git Commands

| Command | Description |
|---------|-------------|
| `git status` | Check current status |
| `git branch` | List all branches |
| `git log --oneline` | View commit history |
| `git diff` | See unstaged changes |
| `git pull origin main` | Get latest changes from main |

---

## 🆘 Troubleshooting

### "Permission denied" error?

Make sure you're authenticated with GitHub:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### "Branch already exists" error?

Use a unique branch name:

```bash
git checkout -b firstname-lastname
```

### Can't push to origin?

You might need to set upstream:

```bash
git push -u origin your-branch-name
```

---

## 📚 Resources for Further Learning

- [Git Official Documentation](https://git-scm.com/doc)
- [GitHub Learning Lab](https://lab.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- [Oh Shit, Git!?!](https://ohshitgit.com/) - For when things go wrong!

---

## 🤝 Connect With Us

- **GDG Kathmandu**: [gdg.community.dev/gdg-kathmandu](https://gdg.community.dev/gdg-kathmandu)
- **HECC**: Himalaya Electronics & Computer Club

---

```html
<div align="center">
Made with ❤️ for B.Tech Students
Happy Learning! 🎉
</div>
```
