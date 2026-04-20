# Cecelia Alfonso-Stokes — Academic Website

A polished personal academic website for Cecelia Alfonso-Stokes, PhD Candidate in Literary Studies at the University of Wisconsin-Madison.

---

## Deploying to GitHub + Vercel

### First-time setup

1. Create a new GitHub repository (e.g., `cecelia-website`)
2. Push the contents of this `site/` folder to the repo root:
   ```
   git init
   git add .
   git commit -m "Initial site"
   git remote add origin https://github.com/YOUR_USERNAME/cecelia-website.git
   git push -u origin main
   ```
3. Go to [vercel.com](https://vercel.com) and sign in with GitHub
4. Click "Add New Project" and import your new repository
5. Vercel will detect it as a static site — no build settings needed
6. Click "Deploy" — done

Your site will be live at `https://cecelia-website.vercel.app` (or a custom domain).

### Custom domain

In Vercel project settings, go to Domains and add your custom domain (e.g., `ceceliaalfonsostokes.com`). Follow the DNS instructions Vercel provides.

---

## File Structure

```
site/
├── index.html              # Homepage
├── about.html              # Full biography and background
├── research.html           # Dissertation and research agenda
├── publications.html       # Publications and writing
├── teaching.html           # Teaching experience and philosophy
├── talks.html              # Conference presentations and talks
├── public-scholarship.html # Podcast, Holding History, public work
├── cv.html                 # Web CV with PDF download link
├── contact.html            # Contact information
├── css/
│   └── style.css           # All styles (one file)
├── js/
│   └── main.js             # Navigation and subtle interactions
├── images/
│   └── headshot.jpg        # [REPLACE] Cecelia's headshot photo
├── files/
│   └── cv.pdf              # [REPLACE] Cecelia's CV as a PDF
├── favicon.svg             # Site favicon (monogram "CA")
└── README.md               # This file
```

---

## How to Update Content

### Add a publication
Open `publications.html`. Find the **Published Work** section. Copy the commented-out template block and fill in:
- Year
- Article type (journal article, book chapter, etc.)
- Title
- Venue and citation details
- Brief description
- Link (if available)

### Add a conference talk
Open `talks.html`. Copy the entry template and fill in:
- Date
- Paper title
- Conference name and organization
- Location

### Add a new course
Open `teaching.html`. Copy a `<div class="course">` block and update the course number, title, institution, and description.

### Update the CV
1. Replace `files/cv.pdf` with the updated PDF
2. Update the web CV on `cv.html` to match (optional but recommended)
3. Update the date note at the bottom of `cv.html`

### Replace the headshot
Save the photo as `images/headshot.jpg`. The site references this path. Recommended: square or portrait crop, at least 600px wide.

### Add teaching philosophy
Open `teaching.html`. Find the `<div class="placeholder">` block in the **Teaching Philosophy** section and replace it with the actual statement.

### Add past conference presentations
Open `talks.html`. Find the **Past Presentations** section. Follow the entry template (commented out in the code). Add entries in reverse chronological order (most recent first).

---

## Design System

**Font pairing:**
- Headings: Cormorant Garamond (300, 400, 500, 600) — elegant humanist serif
- Body: EB Garamond (400, 400 italic, 500) — readable classical serif
- UI / labels / navigation: Jost (300, 400, 500) — clean geometric sans

**Color palette:**
- Background: `#f9f6f0` (warm cream)
- Text: `#28231e` (warm near-black)
- Accent: `#4d6b58` (muted forest sage)
- Text secondary: `#6b5d52` (warm brown)
- Rule / border: `#ddd5c8` (warm light)

---

## Placeholder Checklist

Before going live, replace the following:

- [ ] `images/headshot.jpg` — Cecelia's photo
- [ ] `files/cv.pdf` — Latest CV as PDF
- [ ] Teaching philosophy statement in `teaching.html`
- [ ] MELUS 2025 paper title in `talks.html` and `cv.html`
- [ ] Past conference presentations in `talks.html`
- [ ] Publications in `publications.html` (as they are completed/accepted)
- [ ] Institutional email in `contact.html` (if preferred over personal email)
- [ ] CV PDF date in `cv.html` (bottom of page)
- [ ] Any chapter titles or working paper titles in `publications.html`

---

## Maintenance Notes

- The site is plain HTML/CSS/JS — no build tools, no dependencies, no CMS. To update any page, simply edit the HTML file and push to GitHub. Vercel redeploys automatically.
- All styles live in one file: `css/style.css`. Colors and fonts are set as CSS custom properties at the top of the file, making global changes easy.
- The navigation bar uses `class="active"` on the current page link. When adding new pages, remember to update the `active` class in each page's nav.
- All placeholder sections are marked with `class="placeholder"` and a visible label so they are easy to find.

---

*Built for Cecelia Alfonso-Stokes. Font licenses: Google Fonts (SIL OFL). No build dependencies.*
