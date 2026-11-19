# princepaijamagar.com.np

Personal portfolio of **Prince Paija Magar**, cybersecurity professional based in Kathmandu.

**Live:** https://princepaijamagar.pages.dev · https://princepaijamagar.com.np

## What it is

A single-page portfolio with a scroll-driven background:

- **Glacier flight:** real drone footage that plays forward and backward with the scroll position.
- **3D layer (Three.js):** prayer flags, a live packet network, and a lattice "trap" that stops red attack packets, illustrating Genjutsu, my AI phishing detection and honeypot system.
- **Sections:** About, Genjutsu, Projects, Education & Experience, Toolkit, Contact.

## Stack

- Plain HTML, CSS and JavaScript in one `index.html`
- [Three.js r128](https://threejs.org/) from cdnjs
- Video compressed with FFmpeg (H.264, short keyframe interval for smooth scrubbing)
- Hosted on Cloudflare Pages, with security headers set in `_headers`

## Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Upload the folder to Cloudflare Pages (Direct Upload), or connect this repository to a Pages project with no build command and `/` as the output directory.
