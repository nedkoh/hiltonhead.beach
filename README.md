# Stone's Throw from the Beach

A beautiful, beachy vacation rental website for a Hilton Head Island property. Built with Jekyll for easy hosting on GitHub Pages.

## Features

- Responsive design optimized for mobile, tablet, and desktop
- Ocean-inspired color palette with sandy accents
- Smooth animations and hover effects
- SEO optimized with meta tags and structured data
- Fast loading with optimized images
- Contact information and booking integration

## Quick Start

### Prerequisites

- Ruby 3.1+ (tested with Ruby 4.0)
- Bundler (`gem install bundler`)

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/hiltonhead.git
   cd hiltonhead
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the development server**
   ```bash
   bundle exec jekyll serve
   ```

4. **View the site**
   Open http://localhost:4000 in your browser

### Live Reload (optional)

For automatic browser refresh on file changes:
```bash
bundle exec jekyll serve --livereload
```

## Deploying to GitHub Pages

### Option 1: GitHub Actions (Recommended)

The repository includes a GitHub Actions workflow that automatically builds and deploys the site.

1. Push your code to GitHub
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

2. Enable GitHub Pages
   - Go to your repository **Settings**
   - Navigate to **Pages** in the sidebar
   - Under "Build and deployment", set Source to **GitHub Actions**

3. The site will automatically deploy on every push to `main`

Your site will be available at: `https://YOUR_USERNAME.github.io/YOUR_REPO/`

### Option 2: Deploy from Branch

1. Build the site locally:
   ```bash
   bundle exec jekyll build
   ```

2. The built site is in the `_site` directory

3. Configure GitHub Pages to serve from the `gh-pages` branch or `docs` folder

## Project Structure

```
hiltonhead/
├── _config.yml          # Jekyll configuration and site settings
├── _layouts/
│   └── default.html     # Base HTML template
├── assets/
│   └── css/
│       └── style.css    # Main stylesheet
├── index.html           # Homepage content
├── Gemfile              # Ruby dependencies
├── .gitignore           # Git ignore rules
└── .github/
    └── workflows/
        └── jekyll.yml   # GitHub Actions deployment
```

## Customization

### Site Settings

Edit `_config.yml` to update:

```yaml
title: "Your Property Name"
description: "Your property description for SEO"

property:
  name: "Property Name"
  location: "City, State"
  guests: 5
  bedrooms: 2
  bathrooms: 1.5

contact:
  email: "your@email.com"
  phone: "123.456.7890"
  booking_url: "https://your-booking-url.com"
```

### Colors

The color palette is defined as CSS variables in `assets/css/style.css`:

```css
:root {
  --ocean-deep: #1a5f7a;      /* Primary blue */
  --ocean-light: #57a0c1;     /* Secondary blue */
  --coral: #ff7f6e;           /* Accent color */
  --sand-light: #f4e4d4;      /* Background tan */
  /* ... more colors */
}
```

### Images

Replace the Unsplash placeholder images with your own property photos:

1. Add images to `assets/images/`
2. Update image `src` attributes in `index.html`

For best results:
- Hero image: 1920x1080px minimum
- Gallery images: 800x600px
- About section: 600x400px

### Content

Edit `index.html` to update:
- Property description
- Amenities list
- Location details
- Testimonials

## SEO Features

The site includes:
- Meta description and keywords
- Open Graph tags for social sharing
- Semantic HTML structure
- Fast load times
- Mobile-friendly responsive design

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome for Android)

## License

This project is open source and available for personal and commercial use.

## Contact

For questions about booking or the property:
- Email: nedkoh@gmail.com
- Phone: 404.374.6726
- Book: [Houfy Listing](https://www.houfy.com/lodging/stones-throw-from-the-beach/79850)
