# GitHub Push Instructions

## Option 1: Using Personal Access Token (Recommended)

1. **Create a GitHub Personal Access Token**:
   - Go to: https://github.com/settings/tokens
   - Click "Generate new token" → "Generate new token (classic)"
   - Select scopes: `repo` (full control)
   - Copy the token (save it - you won't see it again!)

2. **Create GitHub Repository**:
   - Go to: https://github.com/new
   - Repository name: `gregg-henwood-dev-portfolio` (or your preferred name)
   - Description: "Creative Technologist & Full-Stack Developer Portfolio"
   - Public or Private: Your choice
   - Do NOT initialize with README (we have one)
   - Click "Create repository"

3. **Push from your local folder**:
   ```powershell
   cd "D:\Dev Projects 2025\gregg-henwood-dev-portfolio"
   
   git remote add origin https://github.com/YOUR_USERNAME/gregg-henwood-dev-portfolio.git
   git branch -M main
   git push -u origin main
   ```
   When prompted for password, enter your Personal Access Token

## Option 2: Using SSH (if configured)

```powershell
git remote add origin git@github.com:YOUR_USERNAME/gregg-henwood-dev-portfolio.git
git branch -M main
git push -u origin main
```

## Option 3: GitHub Desktop (Easiest)

1. Open GitHub Desktop
2. File → Add Local Repository
3. Select: `D:\Dev Projects 2025\gregg-henwood-dev-portfolio`
4. Click "Publish repository"
5. Name & description populated
6. Choose "Public" or "Private"
7. Click "Publish"

## Next: Enable GitHub Pages

Once pushed:
1. Go to repo Settings
2. Scroll to "Pages"
3. Source: Select `main` branch, `/root` folder
4. Save
5. Your site will be live at: `https://YOUR_USERNAME.github.io/gregg-henwood-dev-portfolio`

(Or if you want it at `gregghenwood.github.io`, rename the repo to `gregghenwood.github.io`)

---

Let me know which option you'd like to use!
