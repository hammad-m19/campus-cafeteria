# Campus Bites - University Cafeteria Website

A warm, modern, and fully responsive website for **Campus Bites**, a fictional university cafeteria. Built with plain HTML5 and CSS3 only, featuring rich CSS animations, a glassmorphism-style header, and a mobile-first design.

## Pages and Owners

| # | Page | File | Stylesheet | Owner |
|---|------|------|------------|-------|
| 1 | Home | `src/index.html` | `styles/index.css` | **Team Lead** |
| 2 | Menu | `src/menu.html` | `styles/menu.css` | Member 1 |
| 3 | Daily Specials and Deals | `src/deals.html` | `styles/deals.css` | Member 2 |
| 4 | How to Order | `src/order.html` | `styles/order.css` | Member 3 |
| 5 | Feedback and Contact | `src/feedback.html` | `styles/feedback.css` | Member 4 |
| 6 | About Us | `src/about.html` | `styles/about.css` | Member 5 |
| 7 | Gallery | `src/gallery.html` | `styles/gallery.css` | Member 6 |
| 8 | FAQ, Hours and Location | `src/faq.html` | `styles/faq.css` | Member 7 |
| - | Shared Global Styles | - | `styles/global.css` | **Team Lead** |

Each page has its own dedicated `.css` file in `styles/`, and all pages share `styles/global.css` for layout, tokens, typography, and animations. The unified bundle is also maintained in `styles/style.css`.

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
    about.css
    deals.css
    faq.css
    feedback.css
    gallery.css
    global.css
    index.css
    menu.css
    order.css
    style.css
```

## How to Run

No build tools or servers are needed. Simply open `src/index.html` in any modern browser:

```bash
open src/index.html
```

Or right-click any HTML file and choose "Open with" your preferred browser.

## Stylesheet Organization

Styles are modularized so each team member can work in their own file without merge conflicts:

- `global.css`: Design tokens, CSS reset, header, navigation, footer, button styles, keyframes, and reduced motion.
- `index.css`: Home hero, floating badges, steaming coffee cup, feature cards, and preview strip.
- `menu.css`: Category jump bar, menu item cards, dietary badges, and price styling.
- `deals.css`: Infinite marquee ticker, featured Daily Special, and combo cards with savings calculation.
- `order.css`: Step-by-step ordering timeline, peak hours CSS bar chart, and pickup rules.
- `feedback.css`: Floating-label inputs, star rating radio row, and contact cards.
- `about.css`: Story section, vertical timeline, mission values, and kitchen team staff cards.
- `gallery.css`: Filter chips, masonry grid, image zooming, and hover caption slide-up.
- `faq.css`: Animated accordion items, weekly opening hours, and campus map.

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
