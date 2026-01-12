# How to Deploy to GitHub Pages

## Step 1: Create a New Repository

1. Go to https://github.com/new
2. Name it `vanguard-ui-guidelines` (or any name you prefer)
3. Set to **Public** (required for free GitHub Pages) or **Private** (requires GitHub Pro)
4. Click **Create repository**

## Step 2: Upload Files

### Option A: Using GitHub Web Interface (Easiest)

1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop all files from this folder:
   - `index.html`
   - `README.md`
   - `.nojekyll`
3. Add commit message: "Initial commit - UI Guidelines v2.0"
4. Click **Commit changes**

### Option B: Using Git Command Line

```bash
cd vanguard-ui-guidelines
git init
git add .
git commit -m "Initial commit - UI Guidelines v2.0"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/vanguard-ui-guidelines.git
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (tab at the top)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**

## Step 4: Access Your Site

After a few minutes, your site will be live at:

```
https://YOUR_USERNAME.github.io/vanguard-ui-guidelines/
```

## Updating the Guidelines

To update the guidelines later:

1. Edit `index.html` locally or on GitHub
2. Commit and push changes
3. GitHub Pages will automatically redeploy (usually within 1-2 minutes)

## Custom Domain (Optional)

To use a custom domain like `ui.vanguard.co.nz`:

1. Go to Settings → Pages
2. Under "Custom domain", enter your domain
3. Add a CNAME record in your DNS pointing to `YOUR_USERNAME.github.io`
4. Wait for DNS propagation (can take up to 24 hours)

## Troubleshooting

- **Site not appearing?** Check Settings → Pages for any error messages
- **404 error?** Make sure your file is named `index.html` (lowercase)
- **Styles not loading?** Clear your browser cache or try incognito mode
