# Philia (φιλία) - Learning Experience Designers Team Website

## 🚀 Deployment Guide

### Prerequisites
- GitHub account
- Vercel account (free tier works)

### Step 1: Initialize Git Repository
```bash
git init
git add .
git commit -m "Initial commit of Philia team website"
```

### Step 2: Create GitHub Repository
1. Go to GitHub and create a new repository named "philia-website"
2. Make it public or private as preferred
3. Don't initialize with README or .gitignore

### Step 3: Connect and Push to GitHub
```bash
git remote add origin https://github.com/YOUR-USERNAME/philia-website.git
git branch -M main
git push -u origin main
```

### Step 4: Deploy to Vercel
1. Sign in to [Vercel](https://vercel.com)
2. Click "New Project" → "Import Git Repository"
3. Select your "philia-website" repository
4. Click "Deploy" (Vercel will automatically detect the static site configuration)

### 🔧 Development Setup
To run locally:
```bash
python3 -m http.server 8000
```
Then open: http://localhost:8000

## 🛠 File Structure
```
/
├── index.html       # Homepage
├── about.html       # About our team
├── team.html        # Team members
├── projects.html    # Project showcase
├── contact.html     # Contact form
├── 404.html         # Custom error page
├── vercel.json      # Deployment config
└── package.json     # Project metadata
```

## ✨ Customization Guide
1. **Team Members**: Edit `team.html` to update:
   - Profile photos (replace Pexels URLs)
   - Names, roles, and bios
   - Social media links

2. **Projects**: Edit `projects.html` to:
   - Add/remove project cards
   - Update project images and descriptions
   - Modify status badges

3. **Styling**: All pages use Tailwind CSS classes for:
   - Colors (primary: blue, secondary: green)
   - Responsive layouts
   - Interactive elements

## 📈 Post-Deployment
1. Set up custom domain in Vercel (optional)
2. Connect Google Analytics (add script to `<head>`)
3. Enable form submissions using Formspree (edit contact.html)

## 💡 Tips
- Update the hero image in `index.html` (currently using Pexels placeholder)
- Add real social media links in the footer
- Test all links before final deployment