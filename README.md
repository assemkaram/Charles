# Charles

A static, single-page business website with a hero section, feature cards, an About section, services, a team section, and a footer. It is built with plain HTML and CSS and has no build step or dependencies beyond a Font Awesome icon stylesheet.

**Live site:** https://assemkaram.github.io/Charles/

## Features

- Sticky-style header with address and email info and a "Get a Quote" button
- Full-width hero with background image and call-to-action
- Four feature cards: Consumer Insights, Emerging Ideas, Thought Leadership, and Marketing Goals
- About section with Vision, Mission, and Goal icons
- Services grid with six cards and "Learn more" links
- Team section with four member cards
- Footer with contact details, social links, and copyright
- Responsive layout for tablets and phones

## Project structure

```
Charles/
├── index.html    # Page structure and content
├── style.css     # All styles, including responsive breakpoints
└── imges/        # Images used by the page (logo, icons, backgrounds, team photos)
```

## Getting started

No installation is needed.

1. Clone or download the repository:
   ```bash
   git clone https://github.com/assemkaram/Charles.git
   ```
2. Open `index.html` in a web browser.

Keep `index.html`, `style.css`, and the `imges/` folder in the same directory. The HTML links to the stylesheet and loads images using relative paths, so the page will look broken if any of them are moved.

## Responsive design

`style.css` uses these breakpoints:

| Screen width | Layout changes |
| --- | --- |
| Up to 1024px | Feature cards and services move to 2 columns; About section gets tighter spacing |
| Up to 768px | Header and navigation stack vertically; About section stacks; team grid moves to 2 columns; footer stacks |
| Up to 480px | Feature cards and services move to 1 column; spacing and font sizes are reduced |

Text sizes use `clamp()` so headings scale smoothly between breakpoints.

## Customization

- **Text and contact details:** edit `index.html`. The address and email appear in the header, the footer, and the contact line in the services section.
- **Colors and layout:** edit `style.css`. Feature card colors are set by the `.d1` to `.d4` classes.
- **Images:** replace files in `imges/`, keeping the same filenames or updating the `src` attributes in `index.html`.


## Deployment

The site is published with GitHub Pages from the `main` branch. Any push to `main` updates the live site after a short delay.
