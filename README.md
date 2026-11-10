# Vee Creations

A responsive, multi-page website concept originally developed for a client who was exploring a business focused on flowers, home décor, wall art, and gift hampers.

The client later changed their business direction, so the website was not taken forward as the final website for an operating business. The project has been preserved as a development and portfolio project.

**Live preview:** https://jeiso-n.github.io/vee-creations/

## Project overview

The website concept presents **Vee Creations** as a Kampala-based creative retail brand. Its original proposed catalogue includes:

- Fresh flowers, bouquets, and vases
- Decorative wall clocks and wall art
- Home and office décor
- Curated gift hampers for special occasions

The interface is organised into four pages:

| Page | Description |
| --- | --- |
| Home | Brand introduction, featured collections, and calls to action |
| Services | Overview of the proposed products and services |
| Reviews | Customer-review page layout |
| Contact | Contact and enquiry information |

> **Project status:** Archived concept / portfolio project. The brand details, business claims, contact information, product availability, statistics, and review content in the demonstration should not be treated as verified details of a currently operating business.

## Technology

The repository contains two implementations of the website:

### Published static website

The GitHub Pages deployment currently serves the standalone HTML implementation from the repository root.

- HTML5
- CSS3
- JavaScript
- Local image assets

It does not require a server-side application to display the published pages.

### React application source

The repository also preserves the React implementation and its development tooling:

- React 19
- TypeScript
- Vite
- TanStack Start and TanStack Router
- Tailwind CSS
- Radix UI components
- Lucide React icons

The React application is retained as source code; it is **not** the version currently published on GitHub Pages.

## Repository structure

```text
vee-creations/
├── images/                 # Images used by the published website
├── public/                 # Public assets for the React application
├── src/                    # React, TypeScript, routes and components
│   ├── assets/
│   ├── components/
│   ├── hooks/
│   ├── lib/
│   └── routes/
├── static-html/             # Preserved standalone HTML implementation
├── index.html               # Published home page
├── services.html            # Published services page
├── reviews.html             # Published reviews page
├── contact.html             # Published contact page
├── style.css                # Published website styles
├── package.json              # React application scripts and dependencies
└── README.md
```

## Run the published website locally

No Node.js installation is required to preview the standalone HTML pages. From the project root, run:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

You can also open `index.html` directly in a browser, although using a local HTTP server is recommended.

## Run the React application locally

Install a compatible Node.js version and npm, then run:

```bash
npm install
npm run dev
```

Vite will print the local development URL in the terminal.

Useful scripts:

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the development server |
| `npm run build` | Build the React application |
| `npm run preview` | Preview a production build |
| `npm run lint` | Run ESLint |

These commands apply to the React source, not the standalone HTML version currently deployed.

## GitHub Pages deployment

The published static site is hosted using GitHub Pages:

**https://jeiso-n.github.io/vee-creations/**

The deployment is configured in the repository's GitHub Pages settings. The published source is the **main branch, root folder**.

To publish updates to the live static website:

1. Update the root-level HTML, CSS, or image files.
2. Commit and push the changes to `main`.
3. Allow GitHub Pages to publish the new version.
4. Open the live URL and verify the changes.

Changes made only under `src/` or `static-html/` do not automatically update the currently published root-level website.

## Project notes

- This repository documents a website concept and its implementation, not a completed client business launch.
- The project is preserved for reference, learning, and portfolio demonstration.
- Before adapting it for a real business, replace or confirm all brand copy, images, business details, contact channels, reviews, and commercial claims with approved information.
- The current GitHub Pages version is a static front end. Features requiring server-side processing, persistent data, or a backend would need a separate service.

---

Created and maintained as a web development project by [jeiso-n](https://github.com/jeiso-n).
