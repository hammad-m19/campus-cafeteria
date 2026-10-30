# Campus Bites - University Cafeteria Website

A warm, modern, and fully responsive website for **Campus Bites**, a fictional university cafeteria. Built with plain HTML5 and CSS3 only, featuring rich CSS animations, a glassmorphism-style header, and a mobile-first design.

## Pages

| # | Page | File | Stylesheet |
|---|------|------|------------|
| 1 | Home | `src/index.html` | `styles/style.css` |
| 2 | Menu | `src/menu.html` | `styles/style.css` |
| 3 | Daily Specials and Deals | `src/deals.html` | `styles/style.css` |
| 4 | How to Order | `src/order.html` | `styles/style.css` |
| 5 | Feedback and Contact | `src/feedback.html` | `styles/style.css` |
| 6 | About Us | `src/about.html` | `styles/style.css` |
| 7 | Gallery | `src/gallery.html` | `styles/style.css` |
| 8 | FAQ, Hours and Location | `src/faq.html` | `styles/style.css` |

All pages share the unified stylesheet `styles/style.css` containing design tokens, layout, header/footer, animations, and page-specific styles.

## Folder Structure

```
campus-cafeteria/
  .gitignore
  README.md
  images/
    bbq.jpg
    biryani.jpg
    burger.jpg
    chai.jpg
    foodfair.jpg
    gulabjamun.jpg
    juices.jpg
    lassi.jpg
    morning.jpg
    patio.jpg
    pizza.jpg
    seating.jpg
  src/
    about.html
    deals.html
    faq.html
    feedback.html
    gallery.html
    index.html
    menu.html
    order.html
  styles/
    style.css
```

## How to Run

No build tools or servers are needed. Simply open `src/index.html` in any modern browser:

```bash
open src/index.html
```

Or right-click any HTML file and choose "Open with" your preferred browser.

## Stylesheet Organization

All styles are unified in `styles/style.css`, organized into clear sections:

- Section 1: Design Tokens & CSS Reset
- Section 2: Global Layout, Header, Navigation, Footer, Buttons
- Section 3: Home Page (`index.html`)
- Section 4: Menu Page (`menu.html`)
- Section 5: Deals Page (`deals.html`)
- Section 6: Order Page (`order.html`)
- Section 7: Feedback Page (`feedback.html`)
- Section 8: About Page (`about.html`)
- Section 9: Gallery Page (`gallery.html`)
- Section 10: FAQ Page (`faq.html`)
- Section 11: Global Animations
- Section 12: Reduced Motion

## Branching Workflow

| Branch | Purpose |
|--------|---------|
| `main` | Production-ready releases only |
| `develop` | Integration branch for all features |
| `release/v1.0` | Release candidate for version 1.0 |
| `feature/<page-name>` | One branch per page, for example `feature/menu` |

### Workflow

1. Create your feature branch from `develop`: `git checkout -b feature/<page-name> develop`
2. Work on your assigned page and CSS section.
3. Push your feature branch and open a pull request into `develop`.
4. After review, merge into `develop`.
5. When all pages are complete, create `release/v1.0` from `develop`.
6. Final testing on the release branch, then merge into `main` and tag `v1.0`.

## Tech Stack

- HTML5 (semantic markup)
- CSS3 (custom properties, animations, grid, flexbox)
- Google Fonts (Poppins and Inter)
- No JavaScript, no frameworks, no build tools

## Design

- **Palette**: Orange #FF6B35, Chocolate #2B1B17, Cream #FFF6E9, Amber #FFB703, Green #2A9D8F
- **Typography**: Poppins (headings), Inter (body)
- **Features**: CSS-only hamburger menu, glassmorphism header, scroll-driven animations, CSS accordion, animated floating labels, star rating, masonry gallery with filter chips
