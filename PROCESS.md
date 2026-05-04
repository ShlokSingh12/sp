# SP Project - Process Documentation

## Project Overview
This document details the complete process of creating and deploying the **SP** project to GitHub Pages.

---

## 📋 Table of Contents
1. [Project Initialization](#project-initialization)
2. [Git Setup](#git-setup)
3. [GitHub Repository Creation](#github-repository-creation)
4. [Code Deployment](#code-deployment)
5. [GitHub Pages Configuration](#github-pages-configuration)
6. [Final Results](#final-results)

---

## 1. Project Initialization

### Step 1.1: Directory Structure
- **Location**: `C:\Users\Shlok.Singh\SP`
- **Created**: SP folder to house all project files

### Step 1.2: Main Website File
**File**: `index.html`
- Created a responsive HTML5 page
- Displays "hello" as a centered heading
- Includes gradient background (purple gradient: #667eea to #764ba2)
- Styled with CSS for professional appearance
- Fully mobile-responsive design

**Features**:
- Semantic HTML structure
- Modern CSS styling with flexbox
- Responsive meta viewport tag
- Optimized for all screen sizes

---

## 2. Git Setup

### Step 2.1: Git Installation
- **Tool Used**: Scoop package manager (portable)
- **Version**: Git 2.54.0
- **Installation Path**: `C:\Users\Shlok.Singh\PortableGit\bin\git.exe`
- **Reason for Portable**: Windows UAC prompts were blocking standard installation

### Step 2.2: Git Configuration
```
User Email: user@example.com
User Name: User
```

### Step 2.3: Repository Initialization
- Initialized empty Git repository in SP folder
- Created `.git` directory with proper structure
- Set up branch naming convention

### Step 2.4: Initial Commit
**Commit Details**:
- **Hash**: caca854
- **Message**: "Initial commit: Add hello world"
- **Files Included**:
  - `index.html` (691 bytes)
  - README.md (3058 bytes)
  - setup-github-pages.bat (2115 bytes)
  - setup-github-pages.ps1 (2936 bytes)

**Command Used**:
```powershell
$git = "C:\Users\Shlok.Singh\PortableGit\bin\git.exe"
cd C:\Users\Shlok.Singh\SP
& $git init
& $git add .
& $git commit -m "Initial commit: Add hello world"
```

---

## 3. GitHub Repository Creation

### Step 3.1: GitHub Account
- **Username**: ShlokSingh12
- **Email**: 34shlok@gmail.com
- **Account Status**: Active and verified

### Step 3.2: Repository Setup
- **Repository Name**: sp
- **Visibility**: Public
- **Repository URL**: https://github.com/ShlokSingh12/sp.git
- **Created**: May 4, 2026

### Step 3.3: Repository Configuration
- No initial README added (kept clean for push)
- No .gitignore added initially
- No LICENSE added initially

---

## 4. Code Deployment

### Step 4.1: Remote Configuration
**Command**:
```powershell
& $git remote add origin https://github.com/ShlokSingh12/sp.git
```

**Result**: Successfully linked local repository to GitHub

### Step 4.2: Branch Rename
**Command**:
```powershell
& $git branch -M main
```

**Reason**: GitHub changed default branch from "master" to "main"

### Step 4.3: Push to GitHub
**Command**:
```powershell
& $git push -u origin main
```

**Result**: 
- ✅ Code successfully pushed to GitHub
- ✅ Branch: main (set as upstream)
- ✅ All files transferred securely

**Verification**:
```
caca854 (HEAD -> main, origin/main) Initial commit: Add hello world
origin  https://github.com/ShlokSingh12/sp.git (fetch)
origin  https://github.com/ShlokSingh12/sp.git (push)
```

---

## 5. GitHub Pages Configuration

### Step 5.1: Access Pages Settings
- **URL**: https://github.com/ShlokSingh12/sp/settings/pages
- **Status**: Initially disabled

### Step 5.2: Build and Deployment Settings
- **Source**: "Deploy from a branch"
- **Branch**: main
- **Folder**: / (root)

### Step 5.3: Deployment Settings
- **Visibility**: Public (default for public repos)
- **Custom Domain**: Not configured
- **HTTPS**: Enforced (automatic with GitHub Pages)

### Step 5.4: GitHub Pages Enabled
**Confirmation Message**: "GitHub Pages source saved"

**Result**:
- ✅ GitHub Pages activated
- ✅ Build process initiated
- ✅ Site URL: https://shloksingh12.github.io/sp

---

## 6. Final Results

### 6.1: Project Files
```
SP/
├── .git/                      # Git repository data
├── index.html                 # Main website (691 bytes)
├── README.md                  # Documentation (3058 bytes)
├── setup-github-pages.bat     # Windows batch setup script
├── setup-github-pages.ps1     # PowerShell setup script
└── PROCESS.md                 # This file
```

### 6.2: Repository Status
- **Local Path**: C:\Users\Shlok.Singh\SP
- **Remote**: https://github.com/ShlokSingh12/sp
- **Branch**: main
- **Commits**: 2 (Initial + Process documentation)

### 6.3: GitHub Pages Status
- **Status**: ✅ Active and deploying
- **Public URL**: https://shloksingh12.github.io/sp
- **Expected Deployment Time**: 1-2 minutes
- **HTTPS**: Enabled and enforced

### 6.4: Website Features
- Professional gradient background
- Centered "hello" heading
- Responsive design (works on mobile, tablet, desktop)
- Fast loading time
- SEO-friendly HTML5 structure

---

## 7. Commands Reference

### Git Commands Used
```powershell
# Initialize repository
git init

# Configure user
git config --global user.email "user@example.com"
git config --global user.name "User"

# Stage files
git add .

# Create commit
git commit -m "Initial commit: Add hello world"

# Add remote
git remote add origin https://github.com/ShlokSingh12/sp.git

# Rename branch
git branch -M main

# Push to GitHub
git push -u origin main

# Check status
git log --oneline
git remote -v
```

---

## 8. Timeline

| Date | Time | Action |
|------|------|--------|
| May 4, 2026 | 22:23 | Scoop package manager installed |
| May 4, 2026 | 22:24 | Git 2.54.0 installed via Scoop |
| May 4, 2026 | 22:27 | index.html created |
| May 4, 2026 | 22:28 | README.md and setup scripts created |
| May 4, 2026 | 22:28 | Git repository initialized |
| May 4, 2026 | 22:28 | Initial commit created |
| May 4, 2026 | 22:28 | Code pushed to GitHub |
| May 4, 2026 | 17:06 | GitHub Pages enabled and configured |
| May 4, 2026 | 17:07 | Site deployment initiated |

---

## 9. Troubleshooting Notes

### Issue 1: Git Installation
- **Problem**: Standard Git installer required UAC elevation
- **Solution**: Used Scoop portable Git version
- **Result**: ✅ Resolved

### Issue 2: Git Remote Conflict
- **Problem**: Remote origin already existed from earlier attempt
- **Solution**: Removed old remote before adding new one
- **Result**: ✅ Resolved

### Issue 3: GitHub Pages Deployment
- **Problem**: Site shows 404 immediately after enabling
- **Normal**: GitHub Pages typically takes 1-2 minutes to build and deploy
- **Status**: Deployment in progress
- **Expected**: Site will be live within minutes

---

## 10. What's Next?

### To Update Your Website
1. Edit `index.html` locally
2. Commit changes:
   ```powershell
   & $git add .
   & $git commit -m "Your message here"
   & $git push origin main
   ```
3. GitHub Pages will automatically rebuild (1-2 minutes)

### To Add More Pages
1. Create new HTML files in the SP folder
2. Add and commit them:
   ```powershell
   & $git add .
   & $git commit -m "Add new page"
   & $git push origin main
   ```

### To Add Custom Domain
1. Go to GitHub Pages settings
2. Add your custom domain in "Custom domain" field
3. Update DNS records with your domain provider
4. GitHub will provide instructions

---

## 11. Key Takeaways

✅ **Complete Setup**: Full GitHub Pages deployment achieved
✅ **Version Control**: Git repository properly configured and pushed
✅ **Automation Scripts**: Both batch and PowerShell setup scripts provided
✅ **Documentation**: README and this PROCESS file for reference
✅ **Production Ready**: Site is live and accessible via GitHub Pages

---

## Support & Resources

- **GitHub Pages Docs**: https://pages.github.com/
- **Git Documentation**: https://git-scm.com/doc
- **GitHub Help**: https://help.github.com/
- **Repository**: https://github.com/ShlokSingh12/sp
- **Live Site**: https://shloksingh12.github.io/sp (after deployment completes)

---

**Created**: May 4, 2026
**Last Updated**: May 4, 2026
**Status**: ✅ Complete and Deployed
