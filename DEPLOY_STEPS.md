# Step-by-Step Deployment Guide

Follow these steps exactly to publish your portfolio.

---

## STEP 1: Initialize Git in Your Project

Open your terminal and run these commands:

```bash
cd /Users/ziconghuang/portfolio-showcase
git init
git add .
git commit -m "Initial commit - Portfolio website"
```

**What this does:** Sets up Git version control in your project folder.

---

## STEP 2: Create a GitHub Repository

1. **Go to GitHub.com** and log in
2. **Click the "+" icon** in the top right corner
3. **Click "New repository"**
4. **Fill in the details:**
   - Repository name: `portfolio-showcase` (or any name you like)
   - Description: "My AIGC Designer Portfolio"
   - Choose: **Public** (so Vercel can access it)
   - **DO NOT** check "Initialize with README" (we already have files)
5. **Click "Create repository"**

**You'll see a page with setup instructions - DON'T follow those yet!**

---

## STEP 3: Connect Your Local Project to GitHub

Go back to your terminal and run these commands (replace `YOUR_USERNAME` with your actual GitHub username):

```bash
cd /Users/ziconghuang/portfolio-showcase
git remote add origin https://github.com/YOUR_USERNAME/portfolio-showcase.git
git branch -M main
git push -u origin main
```

**Example:** If your GitHub username is `alexhuang`, the command would be:
```bash
git remote add origin https://github.com/alexhuang/portfolio-showcase.git
```

**What happens:**
- First command: Connects your local folder to GitHub
- Second command: Renames branch to "main"
- Third command: Uploads all your files to GitHub

**Note:** You'll be asked to enter your GitHub username and password (or use a Personal Access Token if you have 2FA enabled)

---

## STEP 4: Verify Files Are on GitHub

1. **Go back to your GitHub repository page** (refresh if needed)
2. **You should see all your files:**
   - `src/` folder
   - `public/` folder
   - `package.json`
   - `index.html`
   - etc.

**If you see all your files, you're ready for the next step!**

---

## STEP 5: Deploy to Vercel

1. **Go to https://vercel.com** and log in
2. **Click "Add New..." button** (or "New Project" if you see it)
3. **Click "Import Git Repository"**
4. **You'll see a list of your GitHub repositories**
5. **Find and click on `portfolio-showcase`** (or whatever you named it)
6. **Click "Import"**

---

## STEP 6: Configure Vercel Project Settings

On the "Configure Project" page:

1. **Project Name:** Keep it as `portfolio-showcase` (or change if you want)
2. **Framework Preset:** Should auto-detect as "Vite" - **leave it as is**
3. **Root Directory:** Leave as `./` (default)
4. **Build Command:** Should be `npm run build` - **leave it as is**
5. **Output Directory:** Should be `dist` - **leave it as is**
6. **Install Command:** Should be `npm install` - **leave it as is**

**Click "Deploy" button** (usually at the bottom)

---

## STEP 7: Wait for Deployment

You'll see a progress screen showing:
- "Installing dependencies..."
- "Building..."
- "Deploying..."

**This takes about 1-2 minutes.** Just wait!

---

## STEP 8: Your Site is Live! 🎉

When deployment finishes, you'll see:

1. **"Congratulations!" message**
2. **A URL like:** `https://portfolio-showcase-xxxxx.vercel.app`
3. **Click "Visit"** to see your live portfolio!

**Your portfolio is now accessible to everyone!**

---

## STEP 9: Share Your Portfolio

Copy your Vercel URL and share it:
- Put it in your email signature
- Add it to your LinkedIn profile
- Share it with potential clients/employers

**Example URL format:**
```
https://portfolio-showcase-xxxxx.vercel.app
```

---

## Future Updates (How to Update Your Site)

Whenever you make changes to your portfolio:

1. **Make your changes** in your code
2. **Commit and push to GitHub:**
   ```bash
   cd /Users/ziconghuang/portfolio-showcase
   git add .
   git commit -m "Updated portfolio"
   git push
   ```
3. **Vercel automatically redeploys** - your site updates in 1-2 minutes!

**No need to manually deploy again - it's automatic!**

---

## Troubleshooting

### If Git asks for credentials:
- Use your GitHub username
- For password, use a **Personal Access Token** (not your password)
- Create token: GitHub → Settings → Developer settings → Personal access tokens → Generate new token

### If Vercel can't find your repo:
- Make sure the repository is **Public** (not Private)
- Try refreshing the Vercel page

### If build fails:
- Check that all files are pushed to GitHub
- Make sure `package.json` is in the root folder

---

## Quick Command Reference

```bash
# Navigate to project
cd /Users/ziconghuang/portfolio-showcase

# Initialize Git (first time only)
git init
git add .
git commit -m "Initial commit"

# Connect to GitHub (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/portfolio-showcase.git
git branch -M main
git push -u origin main

# For future updates
git add .
git commit -m "Updated portfolio"
git push
```

---

**That's it! Your portfolio will be live in about 5 minutes! 🚀**
