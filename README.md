# Brat Studio Website

A professional, Rockstar Games-inspired website for Brat Studio showcasing the upcoming Isle of Man Racing Adventure game.

## Features

- **Modern Design**: Inspired by Rockstar Games with dark, cinematic aesthetics
- **Responsive**: Fully responsive design that works on all devices
- **Modern CSS**: Utilizes the latest CSS features including nesting, container queries, and scroll-driven animations
- **Smooth Animations**: Interactive elements with smooth transitions and scroll effects
- **Game Showcase**: Highlights the unique multi-genre game combining racing, sailing, and exploration

## Modern CSS Features Used

### 1. **CSS Nesting** (2023+)
CSS nesting allows you to write more organized and maintainable stylesheets by nesting selectors:

```css
.nav-link {
    color: var(--light-text);
    
    &::after {
        content: '';
        /* nested pseudo-element */
    }
    
    &:hover {
        color: var(--primary-color);
    }
}
```

### 2. **Container Queries** (2023+)
Container queries allow elements to adapt based on their container's size, not just the viewport:

```css
@container (max-width: 768px) {
    .about-content {
        grid-template-columns: 1fr;
    }
}
```

### 3. **Scroll-Driven Animations** (2024+)
Modern CSS animations that respond to scroll position:

```css
@supports (animation-timeline: scroll()) {
    .feature-box {
        animation: fadeInUp linear;
        animation-timeline: view();
        animation-range: entry 0% entry 50%;
    }
}
```

### 4. **CSS Custom Properties (Variables)**
Used throughout for consistent theming and easy customization:

```css
:root {
    --primary-color: #ff0000;
    --secondary-color: #ff6b00;
    /* ... */
}
```

### 5. **Modern Color Functions**
Using gradients and color functions for dynamic styling:

```css
background: var(--gradient-primary);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
```

### 6. **Math Functions**
Using `clamp()` for responsive typography:

```css
font-size: clamp(3rem, 8vw, 8rem);
```

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge) with latest updates
- CSS Nesting: Supported in Chrome 112+, Firefox 117+, Safari 16.5+
- Container Queries: Supported in Chrome 105+, Firefox 110+, Safari 16.0+
- Scroll-driven animations: Supported in Chrome 115+, with fallbacks for older browsers

## File Structure

```
Brat_Studio_Website/
├── index.html      # Main HTML structure
├── styles.css      # All styling with modern CSS features
├── script.js       # JavaScript for interactivity
└── README.md       # This file
```

## Getting Started

1. Open `index.html` in a modern web browser
2. No build process required - it's pure HTML, CSS, and JavaScript
3. Customize colors and content in `styles.css` and `index.html`

## Customization

### Changing Colors
Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #ff0000;    /* Change to your brand color */
    --secondary-color: #ff6b00;  /* Secondary accent color */
    /* ... */
}
```

### Adding Content
Edit sections in `index.html` to add your own content, images, or videos.

## Game Concept

The website showcases a unique game combining:
- **Racing**: Forza-style racing on the Isle of Man
- **Isle of Man TT**: Authentic TT race experience
- **Sailing**: Sea of Thieves-inspired treasure hunting
- **Exploration**: Open-world adventure on the Isle of Man

## License

© 2024 Brat Studio. All rights reserved.

