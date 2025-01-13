# Portfolio Website Update Guide

## Table of Contents
- [Basic Setup](#basic-setup)
- [File Structure](#file-structure)
- [How to Update Content](#how-to-update-content)
- [How to Push Changes](#how-to-push-changes)

## Basic Setup

1. Clone the repository:
```bash
git clone https://github.com/SophieXueZhang/SophieXueZhang.github.io.git
cd SophieXueZhang.github.io
```

2. Make sure you're on the `gh-pages` branch:
```bash
git checkout gh-pages
```

## File Structure

- `index.html` - Main content of the website
- `styles/main.css` - All styling and design
- `js/main.js` - JavaScript functionality
- `requirements.md` - Project overview and features

## How to Update Content

### 1. Updating Text Content

To update text content (like About section, Services, etc.):
1. Open `index.html`
2. Find the relevant section using the comments (e.g. `<!-- About Section -->`)
3. Modify the text within the HTML tags
4. Save the file

Example sections in `index.html`:
- Hero section: Look for `<header class="hero">`
- About section: Look for `<section class="about">`
- Services: Look for `<section class="services">`
- Portfolio: Look for `<section class="portfolio">`
- Blog: Look for `<section class="blog">`

### 2. Updating Portfolio Projects

To update portfolio projects:
1. In `index.html`, find the `<section class="portfolio">` section
2. Each project is within a `<div class="portfolio-item">` element
3. Update:
   - Image: Change the `src` attribute in `<img src="...">`
   - Title: Modify text in `<h3>` tags
   - Description: Update text in `<p>` tags

### 3. Updating Contact Form

The contact form uses Formspree. To update:
1. Find the form section: `<section id="contact">`
2. The form action contains your Formspree ID: `action="https://formspree.io/f/xzzzyzvl"`
3. To change where emails are sent, update your Formspree settings at formspree.io

### 4. Updating Styles

To modify the design:
1. Open `styles/main.css`
2. Find the relevant section using comments
3. Common properties to change:
   - Colors: Look for `:root` variables at the top
   - Spacing: Modify `padding` and `margin` values
   - Font sizes: Change `font-size` properties

## How to Push Changes

After making updates:

1. Stage your changes:
```bash
git add .
```

2. Commit your changes:
```bash
git commit -m "Description of your updates"
```

3. Push to GitHub:
```bash
git push origin gh-pages
```

4. Wait 2-3 minutes for GitHub Pages to rebuild
5. Clear your browser cache or open in incognito mode
6. Visit https://sophiexuezhang.github.io to see changes

## Tips

- Always backup your changes before making major updates
- Test changes locally before pushing
- Use browser developer tools (F12) to preview style changes
- Keep image sizes reasonable for fast loading
- Maintain consistent styling across sections

## Need Help?

If you need to make more complex changes or run into issues:
1. Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
2. Review the [requirements.md](requirements.md) file for project structure
3. Consider using GitHub's interface for small text changes    
