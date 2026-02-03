# Deployment Guide

## Step-by-Step GitHub Pages Deployment

### Method 1: GitHub Web Interface (Easiest)

1. **Create a new repository on GitHub**
   - Go to [github.com](https://github.com) and sign in
   - Click the "+" icon in the top right
   - Select "New repository"
   - Name it `link-to-mp4` (or any name you prefer)
   - Make it **Public**
   - **Do not** initialize with README, .gitignore, or license
   - Click "Create repository"

2. **Upload your files**
   - On your new repository page, click "uploading an existing file"
   - Drag and drop these files:
     - `index.html`
     - `README.md`
     - `.gitignore`
   - Scroll down and click "Commit changes"

3. **Enable GitHub Pages**
   - Click on "Settings" (top menu)
   - Scroll down and click "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Under "Branch", select `main` and `/ (root)`
   - Click "Save"

4. **Access your app**
   - Wait 1-2 minutes for deployment
   - Your app will be live at: `https://yourusername.github.io/link-to-mp4`
   - GitHub will show you the URL at the top of the Pages settings

### Method 2: Command Line (For Developers)

```bash
# Navigate to where you want the project
cd ~/Desktop

# Create a new directory
mkdir link-to-mp4
cd link-to-mp4

# Copy your files here (index.html, README.md, .gitignore)
# Then initialize git

git init
git add .
git commit -m "Initial commit: Link to MP4 downloader"

# Add your GitHub repository as remote
# Replace 'yourusername' with your actual GitHub username
git remote add origin https://github.com/yourusername/link-to-mp4.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then follow step 3 from Method 1 to enable GitHub Pages.

### Method 3: GitHub Desktop (GUI)

1. Download and install [GitHub Desktop](https://desktop.github.com)
2. Create a new repository locally
3. Add your files (`index.html`, `README.md`, `.gitignore`)
4. Commit and publish to GitHub
5. Follow step 3 from Method 1 to enable Pages

## Verifying Deployment

After enabling GitHub Pages:

1. Go to your repository's "Actions" tab
2. You should see a workflow called "pages build and deployment"
3. Wait for the green checkmark
4. Visit your URL: `https://yourusername.github.io/link-to-mp4`

## Troubleshooting

**404 Error after deployment?**
- Make sure the file is named exactly `index.html` (lowercase)
- Wait a few minutes - deployments can take 1-5 minutes
- Check that GitHub Pages is enabled in Settings → Pages

**Changes not appearing?**
- GitHub Pages can cache for a few minutes
- Try hard refresh: `Cmd/Ctrl + Shift + R`
- Check the Actions tab to see if deployment completed

**Repository is private?**
- GitHub Pages requires a public repository on the free tier
- Make your repository public in Settings → General → Danger Zone

## Updating Your Deployed App

### Via GitHub Web Interface:
1. Go to your repository
2. Click on `index.html`
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for redeployment

### Via Git Command Line:
```bash
# Make changes to index.html locally
# Then:

git add index.html
git commit -m "Update design"
git push origin main
```

## Custom Domain (Optional)

To use your own domain:

1. Go to Settings → Pages
2. Under "Custom domain", enter your domain
3. Configure DNS with your domain provider:
   - Add a CNAME record pointing to `yourusername.github.io`
4. Wait for DNS propagation (can take up to 24 hours)

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)
