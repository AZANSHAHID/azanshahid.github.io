# Azan Shahid Latif — Personal Portfolio

Personal portfolio website for Azan Shahid Latif, Mechatronics and Control Engineer.

Live at: **[azanshahid.github.io](https://azanshahid.github.io)**

---

## About

This is the source code for my personal portfolio website. It showcases my engineering projects, skills, and background in Mechatronics and Control Engineering.

Featured projects include:

- **AR Glasses** — Augmented reality wearable with end-to-end system integration
- **Hair Extension Machine (HEM)** — Computer vision powered (YOLOv11) automated bonding system
- **Arbormated** — Smart irrigation and resource management system with solar-assisted valve nodes

---

## Repository Structure

```
azanshahid.github.io/
├── .github/
│   └── workflows/
│       └── deploy.yml    ← Auto-deploys on every push to main
├── Images/               ← All media assets (images & videos)
├── .gitignore
├── LICENSE
├── README.md
└── index.html            ← Main portfolio page (all HTML, CSS & JS)
```

---

## Deployment

This site is automatically deployed to **GitHub Pages** via **GitHub Actions**.

Every push to the `main` branch triggers the workflow which:

1. Checks out the latest code
2. Configures GitHub Pages
3. Uploads the site as a deployment artifact
4. Deploys it live to [azanshahid.github.io](https://azanshahid.github.io)

No manual deployment steps required.

---

## Running Locally

Since this is a plain HTML site, no build step is needed. Simply open `index.html` in any browser:

```bash
# Option 1 — Open directly
open index.html

# Option 2 — Serve locally with Python
python -m http.server 8000
# Then visit http://localhost:8000
```

---

## License

[MIT](LICENSE) © Azan Shahid Latif
