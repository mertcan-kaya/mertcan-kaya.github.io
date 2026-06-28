# Mertcan Kaya | Academic Portfolio & Robotics Dossier

[![Website](https://img.shields.io/badge/Website-mertcan--kaya.github.io-2980B9?style=flat-square&logo=google-chrome)](https://mertcan-kaya.github.io/)
[![GitHub](https://img.shields.io/badge/GitHub-mertcan--kaya-212F3D?style=flat-square&logo=github)](https://github.com/mertcan-kaya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mertcan_Kaya-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/mertcankaya/)

This repository contains the source code for my personal academic and professional portfolio. It serves as a centralized hub for my research publications, hardware deployment demonstrations, and professional dossiers.

## 🔬 About Me

I am a Doctoral Candidate at the Technical University of Munich (TUM) and a Research Associate at Coburg University of Applied Sciences. My research bridges control theory, motion planning, and human biomechanics to develop **predictive, human-aware motion-planning frameworks**. 

I focus on enabling robots (such as the Franka Emika Panda, UR3, and mobile bases like TurtleBot 4) to coordinate naturally and safely with human movement in shared physical workspaces.

**Status:** Open to Postdoctoral Fellowships and Robotics R&D roles starting **December 2026**.

## 🏗️ Repository Architecture

This site is engineered as a high-performance, zero-dependency **Single-Page Application (SPA)**. It completely avoids heavy JavaScript frameworks (like React or Vue) to ensure instantaneous load times, robust mobile responsiveness, and maximum SEO accessibility for academic web crawlers.

* **`index.html`** - The singular, core portfolio entry point housing the Hero, Research Vision, Hardware Projects, Publications, and Career Timeline.
* **`*.pdf`** - Hosted academic CVs, industry resumes, and full publication lists directly accessible from the hero section.

### Interactive UI Mechanics (Vanilla JS)
The frontend utilizes lightweight Vanilla JavaScript to execute fluid DOM manipulation without external library bloat:
* **Lazy-Load Video Injection:** Hardware demonstration videos display as static placeholder images, swapping to active YouTube `iframe` embeds only upon user click (`injectActiveStream`). This saves significant initial bandwidth.
* **Expandable Publication Drawer:** The publication catalog features an animated accordion (`togglePublications`) that dynamically reveals extended conference proceedings and preprints via CSS transitions (`drawer-anim`) without navigating away from the page.
* **Responsive Mobile Drawer:** A native `toggleMenu` function handles the mobile navigation state, ensuring clean accessibility on smaller screens.

## 🛠️ Tech Stack & Integrations

* **Markup & Styling:** Native HTML5 & CSS3 (CSS Variables, Flexbox, CSS Grid, custom scroll-padding).
* **Interactivity:** Vanilla JavaScript (ES6).
* **Mathematical Rendering:** [KaTeX](https://katex.org/) auto-render engine for sub-millisecond LaTeX equation compiling directly in the DOM.
* **Typography & Icons:** Native system fonts (`-apple-system`, `Segoe UI`) and FontAwesome 6.4.0.
* **SEO:** Integrated JSON-LD Schema markup mapping to ORCID and Google Scholar identities.

## 🚀 Local Deployment & Testing

To preview the website locally and test formatting changes before pushing to GitHub Pages, run a simple local HTTP server from the root directory:

```bash
# Clone the repository
git clone [https://github.com/mertcan-kaya/mertcan-kaya.github.io.git](https://github.com/mertcan-kaya/mertcan-kaya.github.io.git)

# Navigate to the project directory
cd mertcan-kaya.github.io

# Start a local web server (Python 3)
python3 -m http.server 8000
