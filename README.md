# princepaijamagar.com.np

Personal portfolio of **Prince Paija Magar**: networking, web design and cybersecurity, based in Kathmandu.

**Live:** https://princepaijamagar.pages.dev · https://princepaijamagar.com.np

## What it is

A single-page portfolio with a scroll-driven background:

- **Glacier flight:** real drone footage that plays forward and backward with the scroll position.
- **3D layer (Three.js):** prayer flags, a live packet network, and a lattice "trap" that stops red attack packets, illustrating Genjutsu, my AI phishing detection and honeypot system.
- **Sections:** About, Genjutsu, Inside Genjutsu (pipeline, results, SIEM export), phish_lab case study, Projects, Education & Experience, Toolkit, Contact.
- **Lite mode:** phones and data-saver connections get the still poster only, with no video or 3D, so the page loads fast on mobile data.

## Stack

- Plain HTML, CSS and JavaScript in one `index.html`
- [Three.js r128](https://threejs.org/) from cdnjs
- Video compressed with FFmpeg (H.264), loaded into memory as a blob so scroll scrubbing can seek even where the host ignores HTTP range requests
- One-page CV in `Prince_Paija_Magar_CV.pdf`, built with ReportLab
- Hosted on Cloudflare Pages, with security headers set in `_headers`

## Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Upload the folder to Cloudflare Pages (Direct Upload), or connect this repository to a Pages project with no build command and `/` as the output directory.
