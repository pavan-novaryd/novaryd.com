# NovaRyd Landing Page

A responsive, single-page marketing website for NovaRyd – Clean Public Transport Service featuring electric auto-rickshaws in Mumbai.

## Features

- Fully responsive design that works on all devices
- Built with vanilla HTML and Tailwind CSS (via CDN)
- Zero build steps required - runs directly from the file system
- Optimized for performance and accessibility (WCAG AA compliant)
- Smooth scroll navigation and modern UI components

## Project Structure

```
/
├── index.html          # Single-page website with all content
├── assets/             # Directory for images and favicons
│   ├── novaryd-logo.svg
│   ├── electric-rickshaw.jpg
│   ├── app-screenshot.png
│   ├── favicon-16x16.png
│   ├── favicon-32x32.png
│   ├── apple-touch-icon.png
│   └── site.webmanifest
└── README.md           # This file
```

## Local Development

### Prerequisites

- A modern web browser
- (Optional) A simple local web server

### Running Locally

**Option 1: Direct file opening**

Simply open the `index.html` file in your web browser:

```
double-click index.html
```

**Option 2: Using a local web server (recommended)**

For a more production-like environment, you can use a simple HTTP server. If you have Python installed:

```powershell
# Using Python 3
python -m http.server

# Then open http://localhost:8000 in your browser
```

Or if you have Node.js installed:

```powershell
# Install a simple server globally (if you haven't already)
npm install -g serve

# Run the server
serve .

# Then open the URL shown in the terminal (typically http://localhost:5000)
```

## Deployment with GitHub Pages

This site is designed to be deployed directly to GitHub Pages without any build steps.

### Manual Deployment

1. Push your changes to the `main` branch of your GitHub repository
2. Go to your repository on GitHub
3. Navigate to Settings > Pages
4. Under "Source", select "Deploy from a branch"
5. Select the `main` branch and the root folder (`/`)
6. Click Save

### Automated Deployment with GitHub Actions

This repository includes a GitHub Actions workflow file (`.github/workflows/deploy.yml`) that automatically deploys the site to GitHub Pages whenever changes are pushed to the `main` branch.

The workflow file is already set up and no additional configuration is needed.

## Adding Images

To add the required images:

1. Create the `/assets` directory if it doesn't exist
2. Add your image files to the `/assets` directory
3. Make sure the filenames match those referenced in the HTML:
   - `novaryd-logo.svg`
   - `novaryd-logo-white.svg` (for the footer)
   - `electric-rickshaw.jpg`
   - `app-screenshot.png`
   - Favicon files

## Customization

- **Colors**: The primary color is NovaRyd green (#16A34A) with neutral-100 backgrounds and slate-800 text
- **Fonts**: The site uses Poppins from Google Fonts
- **Content**: Edit the HTML directly to update content, pricing, or features

## License

© 2025 NovaRyd Private Ltd. All rights reserved.
