# 🚀 GitHub Setup & Deployment Guide
## Data Communication Assignment Portfolio

This guide provides step-by-step instructions to push your project to GitHub and make it viewable online.

---

## Prerequisites

### 1. Install Git
- **Windows**: Download from https://git-scm.com/download/win
- **Mac**: Install via Homebrew: `brew install git`
- **Linux**: `sudo apt-get install git` (Ubuntu/Debian)

### 2. Create GitHub Account
- Visit https://github.com/signup
- Complete registration and verify email

### 3. Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

---

## Step-by-Step GitHub Push Instructions

### Step 1: Initialize Git Repository (First Time Only)

Navigate to your project folder and run:
```bash
cd /path/to/data-communication-assignment
git init
```

### Step 2: Add All Files

```bash
git add .
```

This stages all files (index.html, README.md, .gitignore) for commit.

### Step 3: Create Initial Commit

```bash
git commit -m "Initial commit: Data Communication Assignment Portfolio

- Complete professional portfolio website
- 7 content sections with comprehensive information
- Telegraph system diagram with SVG
- Embedded YouTube video for educational content
- Responsive design for all devices
- Multiple external and internal links
- Ready for GitHub and online deployment"
```

### Step 4: Create Repository on GitHub

1. Go to https://github.com/new
2. Enter **Repository name**: `data-communication-assignment`
3. Add **Description**: 
   ```
   A comprehensive Data Communication assignment portfolio featuring 
   concepts, history, technologies, and real-world applications
   ```
4. Choose **Public** (for assignment submission)
5. Click **Create repository**

### Step 5: Add Remote and Push

Copy the commands from GitHub (should look like this):

```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/data-communication-assignment.git
git push -u origin main
```

**Replace YOUR-USERNAME with your actual GitHub username**

Example:
```bash
git branch -M main
git remote add origin https://github.com/john-doe/data-communication-assignment.git
git push -u origin main
```

### Step 6: Verify on GitHub

1. Go to https://github.com/your-username/data-communication-assignment
2. You should see all your files (index.html, README.md, .gitignore)
3. The README.md will display as the repository description

---

## Making Updates & Additional Commits

### After Making Changes

```bash
# Check what files changed
git status

# Stage specific files
git add index.html README.md

# Or stage everything
git add .

# Commit with descriptive message
git commit -m "Update: Added personal student information and links"

# Push to GitHub
git push origin main
```

### Useful Git Commands

```bash
# View commit history
git log --oneline

# Check current status
git status

# View differences
git diff index.html

# Undo last commit (keep changes)
git reset --soft HEAD~1

# View remote information
git remote -v
```

---

## Enable GitHub Pages (View Online)

### Option 1: Quick Setup (Recommended)

1. Go to your repository: https://github.com/your-username/data-communication-assignment
2. Click **Settings** (top right)
3. Scroll down to **"Pages"** section (left sidebar)
4. Under **"Source"**: Select **Deploy from a branch**
5. Select branch: **main**
6. Select folder: **/ (root)**
7. Click **Save**
8. Wait 1-2 minutes for deployment
9. Your site will be at: `https://your-username.github.io/data-communication-assignment/`

### Option 2: Using GitHub Actions

1. Create `.github/workflows/pages.yml`
2. GitHub will automatically build and deploy on each push

---

## Sharing Your Project

### Share the Repository Link
```
https://github.com/your-username/data-communication-assignment
```

### Share the Live Website Link
```
https://your-username.github.io/data-communication-assignment/
```

**Example with username "jane-smith":**
- Repository: `https://github.com/jane-smith/data-communication-assignment`
- Live Site: `https://jane-smith.github.io/data-communication-assignment/`

---

## Common Git Issues & Solutions

### Issue: "fatal: not a git repository"
**Solution**: You're not in the right folder. Navigate to your project:
```bash
cd path/to/data-communication-assignment
```

### Issue: "Permission denied" when pushing
**Solution**: Set up SSH key or use HTTPS with personal access token:
```bash
git remote set-url origin https://YOUR-TOKEN@github.com/your-username/data-communication-assignment.git
```

### Issue: "Branch is behind origin/main"
**Solution**: Pull latest changes first:
```bash
git pull origin main
git push origin main
```

### Issue: Forgot to add remote
**Solution**: Add it now:
```bash
git remote add origin https://github.com/your-username/data-communication-assignment.git
git push -u origin main
```

---

## Customization Checklist Before Final Push

- [ ] Update student name (in header and profile)
- [ ] Update student ID (in profile section)
- [ ] Add personal bio
- [ ] Replace avatar image URL with personal photo
- [ ] Update assignment link to actual assignment document
- [ ] Update Turnitin link with your course code
- [ ] Verify all external links are correct
- [ ] Test navigation - all links should work
- [ ] Test YouTube video plays correctly
- [ ] Check responsiveness on mobile device
- [ ] Review all spelling and grammar
- [ ] Commit all changes to Git
- [ ] Push to GitHub

---

## Advanced Git Tips

### Viewing Your Commits
```bash
git log --graph --oneline --all
```

### Creating Branches (for development)
```bash
git checkout -b feature/add-more-content
# Make changes
git add .
git commit -m "Add new section on 5G networks"
git push origin feature/add-more-content
```

### Reverting Changes
```bash
git checkout -- index.html  # Undo changes to specific file
git reset HEAD~1            # Undo last commit
```

---

## One Million Coders Integration

After completing this assignment, consider:

1. **Visit**: https://www.onemillioncodes.com
2. **Sign Up**: For web development program
3. **Build Portfolio**: Add projects to your GitHub
4. **Learn More**: HTML, CSS, JavaScript, React, and more
5. **Get Certified**: Earn certificates upon course completion

### Share Your Achievement

After pushing to GitHub, you can share:
- Link to your portfolio
- Screenshot of GitHub repo
- Live website link
- GitHub contributions graph

---

## Final Submission Checklist

### What to Submit

1. **GitHub Repository Link**
   - Example: https://github.com/your-username/data-communication-assignment

2. **Live Website Link** (if using GitHub Pages)
   - Example: https://your-username.github.io/data-communication-assignment/

3. **Assignment Details**
   - Student Name: _______________
   - Student ID: _______________
   - Repository URL: _______________
   - Live Site URL: _______________

### Documentation to Include

- ✅ README.md (provided)
- ✅ index.html (main website)
- ✅ .gitignore (provided)
- ✅ All required sections and links
- ✅ Telegraph diagram
- ✅ Embedded video
- ✅ Profile information

---

## Troubleshooting

### My GitHub Pages site is showing 404
- Wait 2-3 minutes for deployment
- Check repository name is correct in URL
- Verify Pages is enabled in repository Settings
- Ensure index.html is in root directory

### My changes aren't showing on the live site
- Verify you pushed to GitHub: `git push origin main`
- Clear browser cache (Ctrl+Shift+Del)
- Check deployment status in Settings → Pages
- Wait a minute for GitHub to rebuild

### I need to update my personal information
1. Edit index.html locally
2. Test changes in browser
3. Git add, commit, and push
4. Changes will appear in a few seconds

---

## Support Resources

- **GitHub Docs**: https://docs.github.com
- **Git Tutorials**: https://git-scm.com/doc
- **GitHub Pages Help**: https://docs.github.com/en/pages
- **One Million Coders**: https://www.onemillioncodes.com

---

## Next Steps After Assignment Submission

1. ✅ Keep your GitHub repository updated
2. ✅ Add more projects to your portfolio
3. ✅ Continue learning at One Million Coders
4. ✅ Build 5-10 projects for your portfolio
5. ✅ Start contributing to open-source projects
6. ✅ Network with other developers on GitHub

---

**Good luck with your Data Communication assignment!**

For questions about Git/GitHub, visit: https://github.com/support
For web development courses, visit: https://www.onemillioncodes.com

