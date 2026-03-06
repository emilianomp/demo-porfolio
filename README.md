# DesignStudio - Creative Freelance Portfolio

**Developer:** Emiliano Mendoza Peña  
**Built with:** VSC + Blackbox AI  
**Live Demo:** [https://demo-profile-26.netlify.app/](https://demo-profile-26.netlify.app/)

A modern, responsive portfolio website for creative freelancers. Built with Bootstrap 5, featuring a clean design, multi-language support, and smooth animations.

![DesignStudio Portfolio](https://images.unsplash.com/photo-1522071820081-009f0129c71c?w=1200&h=600&fit=crop)

## Features

- **Responsive Design** - Looks great on desktop, tablet, and mobile devices
- **Multi-language Support** - English (default), Spanish, and Portuguese
- **Project Showcase** - Display your work with case study pages
- **Services Section** - Highlight your skills and services
- **Contact Form** - Built-in contact form with Bootstrap styling
- **Smooth Animations** - Subtle hover effects and transitions
- **SEO Friendly** - Proper semantic HTML structure

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom styling with CSS variables
- **Bootstrap 5.3** - CSS framework for responsive grid and components
- **Lucide Icons** - Lightweight icon library
- **Google Fonts** - Inter font family

## File Structure

```
demo-porfolio/
├── index.html                 # Main page (English)
├── project-detail.html        # Project case study template
├── README.md                  # This file
├── TODO.md                    # Project notes
├── assets/
│   └── css/
│       ├── style.css          # Shared styles (navigation, footer, forms)
│       ├── home.css           # Home page specific styles
│       └── project-detail.css # Project detail page styles
├── es/
│   └── index.html             # Spanish translation
└── pt/
    └── index.html              # Portuguese translation
```

## Customization

### Changing Colors

Edit the CSS variables in `assets/css/style.css`:

```css
:root {
    --bg-white: #FFFFFF;
    --text-black: #000000;
    --text-gray: #6B7280;
    --accent-teal: #14B8A6;        /* Primary accent color */
    --accent-teal-hover: #0D9488;  /* Hover state color */
    --border-teal-light: rgba(20, 184, 166, 0.2);
}
```

### Updating Content

1. **Main Content** - Edit `index.html`
2. **Spanish Version** - Edit `es/index.html`
3. **Portuguese Version** - Edit `pt/index.html`

### Adding New Projects

1. Copy `project-detail.html` to create a new project page
2. Update the project details (title, description, images, results)
3. Add a link to your new project in `index.html`

### Changing Images

Images are sourced from Unsplash. To use your own:
1. Add images to an `assets/images/` folder
2. Update the `src` attributes in the HTML files

## Multi-language Setup

The language switcher is already implemented in the navigation. To add more languages:

1. Create a new folder (e.g., `fr/`, `de/`)
2. Copy and translate the HTML files
3. Update the language switcher links in all HTML files:

```html
<div class="language-switcher">
    <a class="nav-link lang-link" href="../index.html">EN</a>
    <a class="nav-link lang-link" href="es/index.html">ES</a>
    <a class="nav-link lang-link" href="pt/index.html">PT</a>
    <!-- Add your language -->
    <a class="nav-link lang-link" href="fr/index.html">FR</a>
</div>
```

## How to Run

### Local Development

Simply open `index.html` in your browser, or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000`

### Deployment

This is a static website - deploy to any static hosting service:

- **Netlify** - Drag and drop the folder to Netlify
- **Vercel** - Connect your GitHub repository
- **GitHub Pages** - Enable in repository settings
- **Traditional Hosting** - Upload via FTP/SFTP

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

MIT License - Feel free to use this template for your own portfolio.

---

Built with ❤️ using Bootstrap 5

