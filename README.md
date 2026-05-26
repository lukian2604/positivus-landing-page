# Positivus Landing Page

🔗 **Live Site:** [lukian2604.github.io/positivus-landing-page](https://lukian2604.github.io/positivus-landing-page/)

## About

Positivus is a responsive landing page for a digital marketing agency. The design features a modern light/dark aesthetic with a green accent color and clean typographic hierarchy — built with HTML, SCSS (compiled to CSS), and no JavaScript frameworks.

## Sections

| Section | Description |
|---|---|
| **Header** | Logo, navigation menu, "Request a quote" button, mobile hamburger overlay |
| **Hero** | Headline, description, CTA button, and decorative SVG background |
| **Partners** | Horizontal logo strip — Amazon, Dribbble, HubSpot, Notion, Netflix, Zoom |
| **Services** | 6-card grid, each with icon, title, and "Learn more" link |
| **Case Studies** | 3-column panel with highlighted results and "Learn more" links |
| **Process** | Numbered accordion-style steps for the agency workflow |
| **Team** | 6-member grid with name, role, bio, and LinkedIn link |
| **Testimonials** | Review slider with star rating, quote, author, and pagination dots |
| **Contact Us** | Left-form / right-illustration layout with radio group and text fields |
| **Footer** | Logo, nav links, social icons (Facebook, LinkedIn, Twitter), newsletter subscribe form |

## Tech Stack

| Technology | Details |
|---|---|
| HTML5 | Semantic markup, single `index.html` |
| CSS3 / SCSS | Custom properties, Flexbox, Grid, mobile-first media queries |
| Fonts | Space Grotesk Regular & Medium — self-hosted `.woff2` |
| Icons & Images | SVG assets only (no external icon libraries) |

## Project Structure

```
positivus-landing-page/
├── index.html
├── fonts/
│   ├── SpaceGrotesk-Regular.woff2
│   └── SpaceGrotesk-Medium.woff2
├── images/
│   ├── logo.svg
│   ├── logo-light.svg
│   ├── hero-bg.svg
│   ├── banner-bg.svg
│   ├── contact-us-bg.svg
│   ├── icons/
│   │   ├── arrow-left.svg
│   │   ├── arrow-right.svg
│   │   ├── arrow-top-right 1.svg
│   │   ├── facebook.svg
│   │   ├── linkedin.svg
│   │   ├── star.svg
│   │   └── twitter.svg
│   ├── partners/          # 6 partner logos
│   ├── services/          # 6 service icons
│   └── team/              # 6 team member portraits
└── styles/
    ├── styles.css          # compiled output (ready to use)
    ├── styles.scss         # SCSS entry point
    ├── _fonts.scss
    ├── _globals.scss
    ├── _media.scss
    ├── _mixins.scss
    ├── _normalize.scss
    ├── _utils.scss
    ├── _variables.scss
    └── blocks/             # one file per component
        ├── _header.scss
        ├── _hero.scss
        ├── _services.scss
        ├── _studies.scss
        ├── _process.scss
        ├── _team.scss
        ├── _reviews.scss
        ├── _contact-us.scss
        ├── _footer.scss
        └── ...
```

## Getting Started

No build step required — the compiled `styles.css` is included. Open `index.html` directly in a browser or serve with any static file server:

```bash
# VS Code Live Server, or:
npx serve .
```

To edit styles, compile SCSS after changes:

```bash
# Install sass once
npm install -g sass

# Watch for changes
sass --watch styles/styles.scss styles/styles.css
```

## Deployment

Deployed via **GitHub Pages** from the `main` branch root. Push to `main` and the live site updates automatically.
