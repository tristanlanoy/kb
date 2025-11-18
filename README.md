# kb - Personal Tech Knowledge Base

This repository contains my personal tech knowledge base, automatically published to GitHub Pages using MkDocs.

## 📚 View the Documentation

The knowledge base is automatically built and deployed to GitHub Pages. Visit the live site at:
- https://tristanlanoy.github.io/kb/

## 🚀 Features

- **Automated Deployment**: CI/CD pipeline automatically builds and deploys to GitHub Pages on every push to `main`
- **Beautiful UI**: Using Material for MkDocs theme with dark/light mode
- **Search**: Full-text search functionality
- **Markdown**: Write documentation in simple markdown format

## 📝 Local Development

To work on this knowledge base locally:

1. Install Python 3.x
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the development server:
   ```bash
   mkdocs serve
   ```
4. Open http://127.0.0.1:8000/ in your browser

## 📁 Structure

- `docs/` - Markdown documentation files
- `mkdocs.yml` - MkDocs configuration
- `.github/workflows/` - GitHub Actions CI/CD pipeline

## ✏️ Adding Content

1. Add or edit markdown files in the `docs/` directory
2. Commit and push to the `main` branch
3. GitHub Actions will automatically build and deploy the site

## 🛠️ Configuration

The MkDocs configuration is in `mkdocs.yml`. You can customize:
- Site name and description
- Theme settings
- Navigation structure
- Enabled plugins and extensions
