# GitHub Pages Setup Guide

This document provides instructions for enabling GitHub Pages for the AI Story Studio demo.

## Manual Setup Required

Since GitHub Pages configuration requires repository settings changes that cannot be automated through code, follow these steps:

### Step 1: Enable GitHub Pages
1. Go to your repository settings: `https://github.com/kalosha959-wq/github-mcp-server/settings`
2. Scroll down to the "Pages" section in the left sidebar
3. Under "Source", select "GitHub Actions"
4. The workflow in `.github/workflows/pages.yml` will automatically deploy the site

### Step 2: Access Your Demo
Once GitHub Pages is enabled and the workflow runs successfully, your AI Story Studio demo will be available at:

- **Main Demo**: `https://kalosha959-wq.github.io/github-mcp-server/ai-story-studio-combined.html`
- **Index Page**: `https://kalosha959-wq.github.io/github-mcp-server/`

### Step 3: Verify Deployment
- Check the Actions tab to see the deployment workflow status
- The first deployment may take 2-5 minutes to become available
- Subsequent updates will deploy automatically when changes are pushed to the main/master branch

## Files Created

1. **`ai-story-studio-combined.html`** - The main demo application
2. **`.github/workflows/pages.yml`** - GitHub Pages deployment workflow
3. **Updated `README.md`** - Documentation with demo links

## Troubleshooting

If the site doesn't load:
1. Check that GitHub Pages is enabled in repository settings
2. Verify the Actions workflow completed successfully
3. Ensure the source is set to "GitHub Actions" (not branch-based deployment)
4. Wait a few minutes for DNS propagation

## Repository Structure

After implementation, your repository structure includes:

```
github-mcp-server/
├── ai-story-studio-combined.html     # Main demo application
├── .github/workflows/pages.yml       # GitHub Pages deployment
├── README.md                         # Updated with demo links
└── ... (existing MCP server files)
```

The demo showcases GitHub MCP Server integration capabilities while maintaining the repository's primary purpose as a Go-based MCP server.