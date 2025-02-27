# GitHub Setup Instructions for NexusPi

This guide will walk you through setting up a GitHub repository for your NexusPi project and deploying the web components to GitHub Pages.

## 1. Create a GitHub Repository

1. Log in to your GitHub account at [github.com](https://github.com).
2. Click the "+" icon in the top right corner and select "New repository".
3. Name your repository `nexuspi` (all lowercase is recommended for GitHub Pages).
4. Add a description: "iOS marketplace app using Pi Network cryptocurrency and CloudKit"
5. Choose "Public" visibility (required for free GitHub Pages).
6. Initialize with a README (we'll replace it later).
7. Click "Create repository".

## 2. Set Up Git on Your Computer

If you haven't already set up Git on your machine:

```bash
# Install Git if needed (macOS)
brew install git

# Configure Git with your identity
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Generate SSH key if you don't have one
ssh-keygen -t ed25519 -C "your.email@example.com"

# Add SSH key to GitHub account (copy the output)
cat ~/.ssh/id_ed25519.pub
```

Add this public key to your GitHub account in Settings → SSH and GPG keys.

## 3. Clone and Push Your Project

```bash
# Create a local Git repository (in your project directory)
cd /path/to/NexusPi
git init

# Add your GitHub repository as a remote
git remote add origin git@github.com:your-username/nexuspi.git

# Add all files
git add .

# Commit the files
git commit -m "Initial commit"

# Push to GitHub
git push -u origin main
```

## 4. Configure GitHub Pages

1. Go to your repository on GitHub.
2. Click on "Settings" tab.
3. Scroll down to "GitHub Pages" section.
4. Under "Source", select "main" branch and the root folder.
5. Click "Save".

GitHub will provide you with a URL like `https://your-username.github.io/nexuspi/`.

## 5. Update URLs in Your App

Once GitHub Pages is set up, update the URLs in your app:

1. Open `NexusPi/NexusPi/NexusPiApp.swift`.
2. Replace all placeholder URLs with your actual GitHub Pages URL.
3. Commit and push the changes:

```bash
git add NexusPi/NexusPi/NexusPiApp.swift
git commit -m "Update URLs to GitHub Pages"
git push
```

## 6. Verify Your Web Setup

1. Visit your GitHub Pages URL: `https://your-username.github.io/nexuspi/`
2. Check that the index page loads correctly.
3. Verify that the privacy policy is accessible at `https://your-username.github.io/nexuspi/policies/privacy-policy.html`
4. Verify that the terms of service is accessible at `https://your-username.github.io/nexuspi/policies/terms-of-service.html`

## 7. Set Up Pi Network Domain Validation

1. Update the `.well-known/assetlinks.json` file with the correct fingerprint from Pi Network.
2. Commit and push the changes:

```bash
git add NexusPi-Web/.well-known/assetlinks.json
git commit -m "Update assetlinks.json for Pi Network validation"
git push
```

## 8. Configure Pi Network Developer Settings

1. Log in to the [Pi Network Developer Portal](https://developers.minepi.com/).
2. Update your app's development URL to point to your GitHub Pages URL.
3. Set the privacy policy URL to `https://your-username.github.io/nexuspi/policies/privacy-policy.html`.
4. Complete domain validation following Pi Network's instructions.
5. Test your app in the Pi Network sandbox.

## 9. Regular Code Updates

When making changes to your code:

```bash
# Pull latest changes if working with collaborators
git pull

# Add and commit your changes
git add .
git commit -m "Descriptive message about your changes"

# Push to GitHub
git push
```

## 10. Create Branches for New Features (Recommended)

For new features or significant changes:

```bash
# Create and switch to a new branch
git checkout -b feature-name

# Work on your changes, then add and commit
git add .
git commit -m "Add new feature X"

# Push the branch to GitHub
git push -u origin feature-name
```

Then create a Pull Request on GitHub to merge your changes into the main branch. 