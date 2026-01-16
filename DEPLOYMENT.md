# How to Publish Your Portfolio

Your portfolio is ready to go live! Here are the easiest ways to publish it so everyone can access it.

## Option 1: Vercel (Recommended - Easiest & Free)

Vercel is the easiest and most popular option for React/Vite apps.

### Steps:

1. **Create a Vercel account** (if you don't have one):
   - Go to https://vercel.com
   - Sign up with GitHub, GitLab, or email (free)

2. **Install Vercel CLI** (optional, but easier):
   ```bash
   npm install -g vercel
   ```

3. **Deploy from terminal**:
   ```bash
   cd /Users/ziconghuang/portfolio-showcase
   vercel
   ```
   - Follow the prompts
   - It will ask you to login (first time only)
   - Press Enter to use default settings
   - Your site will be live in seconds!

4. **Or deploy via GitHub** (recommended for updates):
   - Create a GitHub repository
   - Push your code to GitHub
   - Go to vercel.com and click "New Project"
   - Import your GitHub repository
   - Vercel will automatically deploy and update on every push!

**Your site will get a URL like:** `https://portfolio-showcase-xxxxx.vercel.app`

---

## Option 2: Netlify (Also Easy & Free)

### Steps:

1. **Go to https://netlify.com** and sign up (free)

2. **Drag & Drop Method** (easiest):
   - Build your project: `npm run build`
   - Go to https://app.netlify.com/drop
   - Drag the entire `dist` folder onto the page
   - Your site is live instantly!

3. **Or use Netlify CLI**:
   ```bash
   npm install -g netlify-cli
   cd /Users/ziconghuang/portfolio-showcase
   netlify deploy
   ```

**Your site will get a URL like:** `https://random-name-123456.netlify.app`

---

## Option 3: GitHub Pages

### Steps:

1. **Install gh-pages package**:
   ```bash
   npm install --save-dev gh-pages
   ```

2. **Update package.json**:
   Add these lines to `package.json`:
   ```json
   "homepage": "https://yourusername.github.io/portfolio-showcase",
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```

3. **Deploy**:
   ```bash
   npm run deploy
   ```

---

## Quick Deploy Commands

### For Vercel (Fastest):
```bash
npm install -g vercel
cd /Users/ziconghuang/portfolio-showcase
vercel
```

### For Netlify (Drag & Drop):
1. Run: `npm run build`
2. Go to: https://app.netlify.com/drop
3. Drag the `dist` folder

---

## Custom Domain (Optional)

Both Vercel and Netlify allow you to add a custom domain for free:
- Vercel: Go to Project Settings → Domains
- Netlify: Go to Site Settings → Domain Management

---

## Important Notes

- Your `dist` folder contains the built website (already created)
- All your images and PDFs in the `public` folder are included
- The site is static and will load fast
- Updates: Just rebuild and redeploy

---

## Need Help?

- **Vercel Docs**: https://vercel.com/docs
- **Netlify Docs**: https://docs.netlify.com

**Recommended: Use Vercel - it's the fastest and easiest!**
