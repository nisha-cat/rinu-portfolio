# Cinematic Photography & Videography Portfolio

Luxury dark portfolio built with React, Vite, Tailwind CSS, GSAP ScrollTrigger, GSAP SplitText, Lenis smooth scrolling, and Framer Motion.

## Add Your Media

Place your own files in:

```text
public/media
```

Supported image formats: `jpg`, `jpeg`, `png`, `webp`, `avif`  
Supported video formats: `mp4`, `webm`, `mov`, `m4v`

The site does not use stock media or remote visual assets. Every hero, gallery, project card, showreel, preview, and portrait pulls from `public/media`.

## Run

On Windows, double-click:

```text
start-portfolio.bat
```

Or run manually:

```bash
npm install
npm run prepare-media
npm run dev
```

Open the local URL Vite prints in the terminal.

## Build

```bash
npm run build
```

`prepare-media` scans uploads and writes `src/data/media-manifest.json`. When the optional `sharp` package is available, it also creates responsive WebP variants in `public/optimized`; otherwise it falls back to the original uploaded files while keeping lazy loading and responsive sizing enabled.
