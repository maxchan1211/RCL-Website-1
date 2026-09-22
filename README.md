# RCL Engineering & Facilities — Website

Multi-page marketing website for RCL Engineering & Facilities Sdn. Bhd.

## Folder contents

```
rcl-website/
├── index.html      # Home
├── about.html      # About Us
├── services.html   # Services
├── projects.html   # Project gallery
├── contact.html    # Contact
├── styles.css      # Shared styles
├── main.js         # Shared JS (nav, form)
├── images/
│   ├── logo.png            # brand logo (nav, footer, favicon)
│   └── p06..p11_crop_*.jpg # project gallery photos
└── README.md
```

## Running it locally

Open `index.html` directly in any browser (double-click on Windows / Mac).

### With VS Code + Live Server (recommended)

1. Open the `rcl-website` folder in VS Code.
2. Install the **Live Server** extension by Ritwick Dey.
3. Right-click `index.html` → **Open with Live Server**.
4. Pages auto-reload on save. Click through the nav (Home / About / Services / Projects / Contact) to navigate.

## Editing tips

- Text content lives in the `.html` files directly. Search for a phrase and edit it.
- Colours and fonts are CSS variables at the top of `styles.css` (`:root { --red: ...; }`).
- Adding a new gallery item: copy a `.gallery-card` block in `projects.html`, drop a new image in `images/` and update the `<img src="...">` and `<h4>` title.
- Adding a new service: copy a `.svc-card` block in `services.html`.
- The nav and footer are duplicated across each page (no build step). If you rename a page, update it in all 5 HTML files.
