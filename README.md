# Modern Static Portfolio

A clean, responsive, single-page portfolio built with **semantic HTML**, **Tailwind CSS (CDN)**, and lightweight **vanilla JavaScript**.

## Overview

This project is a one-file static portfolio (`index.html`) that includes:

- Fixed top navigation with mobile menu toggle
- Hero section with gradient background
- Horizontal carousel/slider with drag support and desktop arrows
- Responsive gallery card grid
- Contact form UI
- Footer with partner placeholders

## Tech Stack

- HTML5
- Tailwind CSS via CDN (`https://cdn.tailwindcss.com`)
- Vanilla JavaScript (inline script)

## Project Structure

```text
static-profolio-main/
├── index.html
└── README.md
```

## Run Locally

Since this is a static page, no build step is required.

1. Open `index.html` directly in your browser.
2. For better local development behavior (recommended), run it through a lightweight local server (for example with VS Code Live Server).

## Features in `index.html`

### Navigation

- Sticky dark navbar
- Mobile hamburger menu (`#menu-btn`) toggles menu visibility (`#menu`)
- Auto-closes mobile menu when a nav link is clicked

### Carousel

- Container: `#slider`
- Buttons: `#prev-btn`, `#next-btn` (desktop only)
- Drag-to-scroll support with mouse interactions

### Gallery

- Responsive 1/2/3 column card layout
- Placeholder image blocks and project metadata labels

### Contact Form

- Form ID: `#contact-form`
- Includes required fields for name, email, and message
- Current submit behavior prevents default and shows an alert

> Note: The form is UI-only right now. To collect real submissions, connect it to a backend endpoint or form service.

## Customization Guide

You can quickly personalize by editing:

- **Branding**: `MyLogo`, page title, hero text
- **Colors**: Tailwind utility classes across sections
- **Content**: Gallery card titles/descriptions and partner names
- **Footer**: Copyright line currently shows `2026 My Website`

## Accessibility Notes

- Uses semantic sections (`nav`, `header`, `section`, `footer`)
- Mobile menu toggle includes `aria-label`
- Consider adding:
  - Better keyboard support for carousel dragging
  - Focus-visible styles for interactive elements
  - Form submission success/error live regions

## Next Improvements (Optional)

- Replace placeholders with real images and `alt` text
- Add touch gesture enhancements for mobile slider
- Integrate a backend for contact form submissions
- Move inline JavaScript into a separate `script.js` file for maintainability
