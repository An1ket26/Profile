# GitHub Pages Deployment Guide

## Option 1: Using GitHub Web Interface (Easiest)

1. **Create Repository**
   - Go to github.com/new
   - Repository name: `<your-username>.github.io`
   - Description: "My Resume & Portfolio Website"
   - Select "Public"
   - Click "Create repository"

2. **Upload Files**
   - Click "Add file" → "Upload files"
   - Upload all files:
     - index.html
     - style.css
     - script.js
     - profile.jpg
     - README.md
   - Click "Commit changes"

3. **Enable GitHub Pages** (Usually automatic for `.github.io` repos)
   - Go to Settings → Pages
   - Ensure "main" branch is selected
   - Your site will be live at: `https://<your-username>.github.io`

---

## Option 2: Using Git Command Line (More Control)

### Prerequisites
- Install Git: https://git-scm.com/download

### Steps

1. **Initialize Git Repository**
   ```bash
   cd c:\Users\Aniket\Desktop\profile
   git init
   git config user.email "01aniket26@gmail.com"
   git config user.name "Aniket"
   ```

2. **Create Repository on GitHub**
   - Go to https://github.com/new
   - Name: `<your-username>.github.io`
   - Make it Public
   - Click "Create repository"
   - Copy the HTTPS URL

3. **Add Remote and Push**
   ```bash
   git add .
   git commit -m "Initial commit: Add portfolio website"
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git branch -M main
   git push -u origin main
   ```

4. **Your site is live!**
   - Access: `https://<your-username>.github.io`
   - It may take 1-2 minutes to deploy

---

## Option 3: Using GitHub Desktop (GUI)

1. Download GitHub Desktop: https://desktop.github.com/
2. Sign in with your GitHub account
3. File → New Repository
4. Fill in:
   - Name: `<your-username>.github.io`
   - Local path: `c:\Users\Aniket\Desktop\profile`
5. Click "Create Repository"
6. Copy files into the folder
7. Publish to GitHub (top right)
8. Visit `https://<your-username>.github.io`

---

## Updating Your Portfolio

### With Git Command Line
```bash
cd c:\Users\Aniket\Desktop\profile
git add .
git commit -m "Update: Add new project/skills"
git push
```

### With GitHub Web
1. Open your repository
2. Click on file to edit
3. Click pencil icon to edit
4. Make changes
5. Commit directly to main

---

## Custom Domain (Optional)

To use your own domain (like aniket.com):

1. Go to repository Settings → Pages
2. Under "Custom domain", enter your domain
3. Update your domain DNS settings:
   - Add CNAME record pointing to `<your-username>.github.io`
   - Or add A records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

---

## Troubleshooting

### Site not loading
- Check repository is Public
- Wait 2-3 minutes for first deployment
- Ensure file is named `index.html`
- Check GitHub Pages is enabled in Settings

### Changes not showing
- Do a hard refresh: Ctrl+Shift+R
- Wait a few minutes for GitHub to rebuild
- Check commit was pushed successfully

### Photo not showing
- Ensure `profile.jpg` is in the same folder as `index.html`
- Check file name matches in HTML (case-sensitive on GitHub)
- Use relative path: `profile.jpg`

---

## Next Steps

1. ✅ Set up GitHub repository
2. ✅ Push your portfolio code
3. 📸 Add your professional photo
4. 🔗 Update all links and content
5. 📝 Share your portfolio link!

---

**Your portfolio will be accessible at: `https://<your-username>.github.io`**

Example: If your GitHub username is "aniket26", your site will be at:
`https://aniket26.github.io`
