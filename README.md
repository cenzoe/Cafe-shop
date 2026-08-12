# Brew & Bean — Coffee Shop Landing Page

A simple, modern, fully responsive landing page for a small coffee shop, built with plain HTML, CSS, and JavaScript (no frameworks).

## Getting Started

No installation or build step required.

1. Download `index.html`.
2. Double-click it, or open it in any web browser (Chrome, Firefox, Safari, Edge).
3. That's it — the page works immediately, including fonts, images, animations, and the mobile menu.

Optional: to preview it like a real hosted site, run a local server from the project folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

## Project Structure

```
brew-bean/
└── index.html   (all HTML, CSS, and JavaScript in one file)
```

Everything — styles and scripts — lives inside `index.html` so the whole site is a single, portable file.

## Sections

| Section | Description |
|---|---|
| Navbar | Logo, nav links, "Order Now" button, mobile hamburger menu |
| Hero | Headline, subtext, "View Menu" / "Order Now" buttons, coffee cup image |
| Popular Menu | 4 product cards — Cappuccino, Caffè Latte, Americano, Mocha |
| About Us | Story + photo + quick stats |
| Why Choose Us | 3 feature cards (Fresh Coffee, Quality Beans, Cozy Atmosphere) |
| CTA | "Your perfect coffee is waiting" call-to-action banner |
| Contact | Address, hours, phone, email, and a map placeholder |
| Footer | Logo, description, social icons, copyright |

## Customizing

- **Colors & fonts** — all defined as CSS variables at the top of the `<style>` block (`:root { ... }`) in `index.html`. Change `--cream`, `--brown-dark`, `--coffee`, etc. to re-theme the whole site.
- **Text content** — edit directly inside the relevant `<section>` tags.
- **Menu items / prices** — each item is a `.menu-card` block in the `#menu` section.
- **Images** — currently pulled from Unsplash via direct URLs (`<img src="https://images.unsplash.com/...">`). Swap these `src` attributes for your own photos, or point them to local files (e.g. `images/hero-cup.jpg`) if you'd rather host images yourself.
- **Map** — the Contact section uses a placeholder `<div class="map-placeholder">`. Replace it with a real embed, e.g.:
  ```html
  <iframe src="https://www.google.com/maps/embed?..." width="100%" height="340" style="border:0; border-radius:18px;" loading="lazy"></iframe>
  ```
- **Social links** — update the `href="#"` attributes in the footer's `.socials` block.

## Features

- Fully responsive (desktop, tablet, mobile)
- Smooth scrolling navigation
- Mobile hamburger menu
- Scroll-reveal animations (fade + rise) via `IntersectionObserver`
- Hover animations on buttons and cards
- Respects `prefers-reduced-motion` for accessibility
- Semantic HTML (`header`, `nav`, `main`, `section`, `footer`)

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). No polyfills needed.

## License

Free to use and modify for personal or commercial projects.
