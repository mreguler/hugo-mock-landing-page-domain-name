# README for `hugo-mock-landing-page-autodeployed`
## Overview

This repository hosts a Hugo website for Homework 2, Part II, featuring automated deployment via GitHub Actions. Changes pushed to the main branch automatically update the live site.

## Deployment Workflow

- **Setup.** Checks out the main branch and fetches submodules.
- **Hugo setup.** Installs Hugo using `peaceiris/actions-hugo`.
- **Build.** Compiles the site with `hugo`, incorporating options for drafts, garbage collection, and minification.
- **Deploy.** Uses `peaceiris/actions-gh-pages` to deploy the built site to the `gh-pages` branch.

## Configuration
- Adjust baseURL in `config.toml` to match the GitHub Pages URL.
- Personalize the site by editing content and settings.

## Usage Instructions

To make changes to the website:
1. Clone the repository and make the desired modifications locally.
2. Commit and push the changes to the main branch.
3. The GitHub Actions workflow will automatically trigger, building and deploying the updated site to GitHub Pages.
