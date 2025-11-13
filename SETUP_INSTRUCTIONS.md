# GitHub Pages Setup Instructions

Follow these steps to deploy your Cloud Computing study materials on GitHub Pages:

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Sign in to your account
3. Click the "New" button to create a new repository
4. Name your repository exactly as: `your-username.github.io` (replace `your-username` with your actual GitHub username)
5. Set the repository to "Public"
6. Do NOT initialize with a README, .gitignore, or license (we'll add our files separately)

## Step 2: Prepare Your Files

The files you need to upload to GitHub are already organized in the `github-pages` folder. These include:
- index.html (main landing page)
- All your study material HTML files
- README.md (repository documentation)
- CNAME (optional, for custom domains)

## Step 3: Upload Files to GitHub

### Option A: Using Git (Recommended)
1. Open Git Bash or your terminal in the `github-pages` folder
2. Initialize a git repository:
   ```
   git init
   ```
3. Add all files:
   ```
   git add .
   ```
4. Commit changes:
   ```
   git commit -m "Initial commit with Cloud Computing study materials"
   ```
5. Connect to your GitHub repository:
   ```
   git remote add origin https://github.com/your-username/your-username.github.io.git
   ```
6. Push to GitHub:
   ```
   git branch -M main
   git push -u origin main
   ```

### Option B: Upload via GitHub Web Interface
1. Go to your `your-username.github.io` repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop all files from the `github-pages` folder
4. Click "Commit changes"

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click the "Settings" tab
3. In the left sidebar, click "Pages"
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click "Save"
7. Wait a few minutes for GitHub to build your site

## Step 5: Access Your Site

Your site will be available at: `https://your-username.github.io`

## Optional: Custom Domain Setup

If you want to use a custom domain:

1. Purchase a domain (if you don't have one)
2. In your domain registrar, create a CNAME record pointing to `your-username.github.io`
3. In your GitHub repository, edit the CNAME file to contain just your domain name (e.g., `study.mycloudcourse.com`)
4. GitHub Pages will automatically use this after a few hours

## Troubleshooting

- **Site not loading**: Wait up to 10 minutes after enabling GitHub Pages for the initial build
- **Changes not showing**: Clear your browser cache or do a hard refresh (Ctrl+F5)
- **Files not appearing**: Ensure all files are in the root directory, not in a subfolder
- **404 errors**: Check that all filenames match exactly (case-sensitive)

## Additional Tips

- All files must be in the root directory for GitHub Pages to work correctly
- The `index.html` file serves as the main page of your site
- All links in the index.html file reference the correct filenames for navigation
- The site is fully responsive and will work on mobile devices
- You can customize the styling by editing the CSS in the index.html file

## Maintaining Your Site

To update your site:
1. Edit your files locally
2. Commit and push changes to the main branch
3. GitHub Pages will automatically rebuild your site