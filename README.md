# 🌱 NCU Saga Wiki

NCU Saga Wiki is a digital knowledge base that serves as a central repository for information, notes, and documentation. Built using Quartz, it transforms Markdown files into an interconnected and searchable website.

Live Site: https://ncuwiki.com (currently pointing to old site)

---
# For Developers:

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v20 or v22+)
- [npm](https://www.npmjs.com/) (v9.3.1+)

### Local Development

1. Clone this repository
   ```bash
   git clone https://github.com/ncuwiki/ncuwiki.git
   cd ncuwiki
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npx quartz build --serve
   ```

4. Visit `http://localhost:8080` in your browser

### Adding Content

1. Add Markdown files to the content directory
2. Use standard Markdown syntax
3. Create links between notes using `[[wiki-style links]]`
4. Add frontmatter to the top of your files for metadata:
   ```markdown
   ---
   title: My Note Title
   tags:
     - example
     - documentation
   ---

   Note content goes here...
   ```

## 📝 Editing Content

1. Create or edit Markdown files in the content directory
2. Commit and push your changes to the `v4` branch
3. The GitHub Actions workflow will automatically build and deploy your changes

## 🔄 Deployment

This wiki is automatically deployed to GitHub Pages using GitHub Actions. Any changes pushed to the `v4` branch will trigger a new build and deployment.

The deployment workflow:
1. Checks out the repository
2. Sets up Node.js
3. Installs dependencies
4. Builds the Quartz site
5. Deploys to GitHub Pages

## 🛠️ Configuration

The site configuration is managed in `quartz.config.ts`. You can customize:

- Site title and metadata
- Theme colors and typography
- Plugins and extensions
- Navigation and layout

## 📚 Resources

- [Quartz Documentation](https://quartz.jzhao.xyz/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
