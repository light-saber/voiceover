# GitHub Upload Instructions

Follow these steps to upload your VoiceOver project to GitHub:

## 1️⃣ Create a New Repository on GitHub

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** icon in the top right → **"New repository"**
3. Repository name: `voiceover` (or your preferred name)
4. Description: `🎙️ A beautiful mobile-first PWA for voice notes with speech recognition`
5. Choose **Public** (or Private if you prefer)
6. **DO NOT** initialize with README, .gitignore, or license (we already have these)
7. Click **"Create repository"**

## 2️⃣ Push Your Code to GitHub

After creating the repository, run these commands in your terminal:

```bash
# Navigate to your project directory
cd /Users/sachin/Documents/Projects/voiceover

# Add all files to git
git add .

# Commit your files
git commit -m "Initial commit: VoiceOver PWA with speech recognition"

# Add your GitHub repository as remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/voiceover.git

# Push to GitHub
git push -u origin main
```

## 3️⃣ Enable GitHub Pages (Optional)

To host your app for free:

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under "Source", select **main** branch
4. Click **Save**
5. Your app will be live at: `https://YOUR_USERNAME.github.io/voiceover/`

## 4️⃣ Future Updates

When you make changes to your project:

```bash
# Check what files changed
git status

# Add changed files
git add .

# Commit with a descriptive message
git commit -m "Add new feature: XYZ"

# Push to GitHub
git push
```

## 🎯 Quick Commands Reference

| Command | Purpose |
|---------|---------|
| `git status` | Check what files have changed |
| `git add .` | Stage all changes |
| `git add filename` | Stage specific file |
| `git commit -m "message"` | Commit staged changes |
| `git push` | Upload commits to GitHub |
| `git pull` | Download changes from GitHub |
| `git log` | View commit history |

## 🔗 Useful Links

- [GitHub Desktop](https://desktop.github.com/) - GUI alternative to command line
- [GitHub Docs](https://docs.github.com/) - Official documentation
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) - Quick reference

---

**Note**: Replace `YOUR_USERNAME` with your actual GitHub username in all commands!
