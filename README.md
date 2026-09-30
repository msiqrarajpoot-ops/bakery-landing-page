# Golden Crumb Bakery — Landing Page

A responsive, single-page landing site for a bakery, built with plain HTML, CSS and JavaScript. No build step, no dependencies — open it and it works.

## Features

- **Sticky navigation** with animated underline links and a mobile hamburger menu
- **Hero section** with floating bread art, stats and dual call-to-action buttons
- **Features row** highlighting what makes the bakery special
- **Today's Menu** — six product cards with prices
- **Our Story** section with a checklist of highlights
- **Testimonials** on a contrasting dark band
- **Visit Us** panel with address, hours and a newsletter signup form
- **Scroll-reveal animations** via `IntersectionObserver`
- Fully responsive (desktop → tablet → mobile), respects `prefers-reduced-motion`

## Getting started

Clone the repository and open `index.html` in your browser:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
start index.html    # Windows
```

Or serve it locally:

```bash
npx serve .
# or
python -m http.server 8000
```

Then visit http://localhost:8000.

## Project structure

```
.
├── index.html   # Page markup and content
├── styles.css   # All styling, design tokens and responsive rules
├── script.js    # Menu toggle, scroll reveal, form handling
└── README.md
```

## Customisation

Design tokens live at the top of `styles.css` in the `:root` block — change `--brand`, `--bg`, fonts or radii to retheme the whole page:

```css
:root {
  --brand: #b3541e;   /* primary accent */
  --bg: #fdf8f1;      /* page background */
  --radius: 18px;     /* card corner radius */
}
```

Menu items, prices, opening hours and contact details are all plain markup in `index.html`.

## Browser support

Modern evergreen browsers (Chrome, Firefox, Edge, Safari). Uses `backdrop-filter`, CSS Grid and `IntersectionObserver`, all with graceful fallbacks.

## License

Free to use for your own projects.
