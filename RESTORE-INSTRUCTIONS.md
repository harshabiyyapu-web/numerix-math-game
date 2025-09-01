# 🔄 BACKUP & RESTORE INSTRUCTIONS

## Current Stable Version: v1.0-stable

Your working Numerix game has been backed up in multiple ways. Use any of these methods to restore if needed.

---

## 📦 BACKUP METHODS

### Method 1: Git Tag (Recommended)
- **Tag Created**: `v1.0-stable`
- **Location**: Both local and GitHub repository
- **Contains**: Complete working version with Airtable integration

### Method 2: Backup File
- **File**: `index-backup-v1.0.html`
- **Location**: Same directory as your main game
- **Contains**: Exact copy of working version

---

## 🔄 HOW TO RESTORE

### Option A: Using Git Tag (Full Restore)
```bash
# Go to your project directory
cd "/Users/harshabiyyapu/Desktop/Github Cursor/Matriks jakruthi"

# Restore to the stable version
git checkout v1.0-stable

# Create a new branch from the stable version (optional)
git checkout -b restored-stable

# Push the restored version to GitHub
git push origin main --force
```

### Option B: Using Backup File (Simple Restore)
```bash
# Go to your project directory
cd "/Users/harshabiyyapu/Desktop/Github Cursor/Matriks jakruthi"

# Copy backup over current file
cp index-backup-v1.0.html index.html

# Commit and push
git add index.html
git commit -m "Restore to stable v1.0 version"
git push
```

### Option C: Manual Restore
1. Open `index-backup-v1.0.html` in any text editor
2. Copy all the content
3. Paste it into `index.html`
4. Save and push to GitHub

---

## ✅ STABLE VERSION FEATURES

Your backed-up version includes:
- ✅ Working Airtable integration (saves name/email to D1 table)
- ✅ Autoplay background music
- ✅ Three difficulty levels with proper question types
- ✅ Visual difficulty selection with feedback
- ✅ Leaderboard system
- ✅ WhatsApp sharing
- ✅ Multi-level progression (3 levels)
- ✅ Timer system (120 seconds per level)
- ✅ Scoring system (+10 correct, -2 wrong)

---

## 🎯 WHEN TO USE RESTORE

Use restore if:
- New changes break the game
- You want to go back to the working version
- Experiments don't work out
- You need the stable version quickly

---

## 💡 DEVELOPMENT TIP

After making experimental changes:
1. Test thoroughly
2. If you like the changes, create a new backup:
   ```bash
   git tag -a v2.0-experimental -m "New experimental version"
   git push origin v2.0-experimental
   ```
3. If you don't like them, use restore instructions above

---

**Your stable version is safely backed up! Feel free to experiment now! 🚀**
