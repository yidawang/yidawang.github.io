# Personal Website

A minimal Jekyll-based personal website that deploys directly to GitHub Pages without needing to copy generated files to a separate repository.

## Features

- Clean, responsive design
- SEO optimization with meta tags and sitemap
- Social media integration
- GitHub Actions deployment
- Mobile-friendly layout
- Direct GitHub Pages deployment

## Quick Start

1. **Use this template** or clone this repository
2. **Edit `_config.yml`** with your personal information
3. **Customize content** in `about.md` and other pages
4. **Update social links** in `_config.yml`
5. **Push to GitHub** and enable Pages in repository settings

## Local Development

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Build site
bundle exec jekyll build
```

## Deployment

This site uses GitHub Actions to automatically build and deploy to GitHub Pages when you push to the main branch.

### Setup GitHub Pages

1. Go to your repository settings
2. Navigate to Pages section
3. Set Source to "GitHub Actions"
4. Push to your main branch to trigger deployment

## File Structure

```
├── _layouts/          # Page templates
├── .github/workflows/ # GitHub Actions
├── assets/css/       # Stylesheets
├── _config.yml       # Site configuration
├── index.md          # Homepage
├── about.md          # About page
├── contact.md        # Contact page
└── Gemfile           # Ruby dependencies
```

## Customization

- **Personal info**: Edit `_config.yml` with your name, title, description
- **Navigation**: Update `navigation` section in `_config.yml`
- **Social links**: Update `social` section in `_config.yml`
- **Styling**: Modify `assets/css/style.css`
- **Content**: Edit markdown files for each page
- **About page**: Add your professional background and experience

## Dependencies

- Jekyll 4.3+
- GitHub Pages compatible gems
- jekyll-seo-tag
- jekyll-feed
- jekyll-sitemap