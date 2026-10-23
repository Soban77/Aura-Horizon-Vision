# Aura Horizon Vision

A responsive, single-page smartwatch launch site with a WebGL Hero watch and interactive Design Studio.

## Features

- Hero smartwatch rendered with Three.js and interactive drag rotation.
- Studio model with PBR-inspired case materials, studio environment reflections, and four interchangeable bands.
- GSAP camera focus presets, selectable watch-face textures, and live rear-plate engraving preview.
- Live pre-order pricing for 42mm ($799), 46mm ($899), and 49mm ($1,099), with a $100 5G Satellite option. Band choices are included at no extra charge.
- Responsive product details, hardware hotspots, specifications, and comparison sections.

## Run locally

Open `index.html` in a modern browser, or serve the project root with any static web server. The page loads Tailwind CSS, Three.js, GSAP, Lucide icons, and fonts from CDNs, so an internet connection is required for those assets.

## Deploy with GitHub Pages

1. Push this project to a GitHub repository.
2. In the repository, open **Settings > Pages**.
3. Select deployment from the `main` branch and the root (`/`) folder.
4. Save; GitHub Pages will publish `index.html`.

No build step is required.

## Checkout limitations

The pre-order form sends reservation details as `FormData` to the configured FormSubmit mailbox. Confirm the mailbox activation email from FormSubmit before accepting submissions. The UI shows the invoice only after FormSubmit accepts the request; acceptance does not guarantee delivery to the mailbox.

The selected card, mobile wallet, or bank-wire option is a **payment preference only**. The static site does not process or verify payments, generate checkout links, store orders, or guarantee fulfillment. The sales team must provide final checkout or wire instructions. Use a trusted payment provider and a secure backend before accepting real payments.

## Environment values and secrets

There are no required environment variables for the current static site. `.env` is ignored by Git; keep local secrets and personal information out of tracked files. Never commit a populated `.env` file.
