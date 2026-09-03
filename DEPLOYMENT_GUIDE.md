# GitHub Pages & Profile Deployment Guide

This package contains everything needed to launch your live **interactive portfolio website** and your **GitHub Profile README**.

---

## 🚀 Option 1: Deploy to `elvintsang.github.io` (Recommended)

This creates your personal root domain portfolio at `https://elvintsang.github.io`.

### Step 1: Create the repository on GitHub
1. Go to [GitHub New Repository](https://github.com/new).
2. Name the repository exactly:
   ```
   elvintsang.github.io
   ```
3. Set visibility to **Public**.
4. Click **Create repository**.

### Step 2: Push the `portfolio` files
Run these commands from your terminal:

```bash
cd "/Users/elvintsang/Documents/SKYLOFT App/portfolio"

# Initialize git if needed
git init
git add .
git commit -m "feat: ship interactive portfolio and live SkyLoft web app"

# Link to your new repository and push
git branch -M main
git remote add origin https://github.com/elvintsang/elvintsang.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub: `https://github.com/elvintsang/elvintsang.github.io/settings/pages`.
2. Under **Build and deployment** > **Source**, ensure **Deploy from a branch** is selected.
3. Select **Branch: main**, folder: `/ (root)`, and click **Save**.
4. In ~60 seconds, your site will be live at:
   👉 **`https://elvintsang.github.io`**

---

## 📄 Setup Your GitHub Profile README (`github.com/elvintsang`)

To display your featured projects directly on your GitHub user profile:

1. Create a new public repository on GitHub named exactly your username:
   ```
   elvintsang
   ```
   *(GitHub displays a special banner: "You found a secret! elvintsang/elvintsang is a special repository...")*
2. Check the box **"Add a README file"** (or push an empty repo).
3. Copy the contents of [`portfolio/PROFILE_README.md`](./PROFILE_README.md) into the `README.md` of that repository.
4. Commit and push.

Whenever an employer visits `https://github.com/elvintsang`, they will see your high-impact profile, dynamic architecture diagram, stats badges, and direct links to test your live app!

---

## 🔍 What Employers Will Experience

1. **Interactive iPhone Simulator**: They can directly click, scroll, and test the real SkyLoft app without installing anything.
2. **Onboarding & RecSys Feed**: They can complete the 3 questions and see instant personalized apartment recommendations with net-effective pricing and transit estimates.
3. **Application State Machine**: They can test the unit hold flow and KYC document upload interface.
4. **Deep Technical Breakdown**: Below the simulator, they can inspect tabs explaining React Native Web, Python Flask architecture, scoring math, and data mining parsers.
