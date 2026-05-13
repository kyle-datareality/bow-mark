# Bow Mark — Website

A modern, static one-page site for **Bow Mark Paving & Concrete** (Okotoks, AB · est. 1979), plus an *In the Community* page.

Pure HTML + CSS + JS. No build step. Deploys to any static host (Vercel, Netlify, GitHub Pages, Cloudflare Pages).

## Structure

```
.
├── index.html          # main site (hero, services, projects, about, safety, careers, quote)
├── community.html      # "In the Community" page (linked from the hamburger menu)
├── README.md
├── .gitignore
└── images/
    ├── logo.png        # silver Bow Mark badge used in nav + footer
    ├── commercial/     # Commercial & Industrial project photos
    ├── residential/    # Residential development photos
    ├── transportation/ # Transportation Infrastructure photos (incl. bow01.jpg hero bg)
    └── community/      # Community page photos
```

## Local preview

Any static server works. Examples:

```bash
# Python (built-in)
python3 -m http.server 8000

# Ruby (built-in on macOS)
ruby -run -e httpd . -p 8000

# Node
npx serve .
```

Then open http://localhost:8000

## Deploy to Vercel

1. Push this folder to a new GitHub repo
2. In Vercel: **Add New → Project → Import** the repo
3. Leave all defaults (Framework Preset = *Other*, no build command, output dir = root)
4. **Deploy**

That's it. Vercel auto-redeploys on every push to `main`.
