# Mertcan Kaya | Academic Portfolio & Robotics Dossier

[![Website](https://img.shields.io/badge/Website-mertcan--kaya.github.io-2980B9?style=flat-square&logo=google-chrome)](https://mertcan-kaya.github.io/)
[![GitHub](https://img.shields.io/badge/GitHub-mertcan--kaya-212F3D?style=flat-square&logo=github)](https://github.com/mertcan-kaya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mertcan_Kaya-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/mertcankaya/)

This repository contains the source code for my personal academic and professional portfolio. It serves as a centralized hub for my research publications, hardware deployment demonstrations, algorithm simulations, and professional dossiers.

## 🔬 About Me

I am a Doctoral Candidate at the Technical University of Munich (TUM) and a Research Associate at Coburg University of Applied Sciences. My research bridges control theory, motion planning, and human biomechanics to develop **predictive, human-aware motion-planning frameworks**. 

I focus on enabling robots (including the Franka Emika Panda, UR3, Stäubli RX160, and mobile bases like TurtleBot 4 & AgileX Scout Mini) to coordinate naturally and safely with human movement in shared physical workspaces.

**Status:** Open to Postdoctoral Fellowships and Robotics R&D roles starting **December 2026**.

## 🏗️ Repository Architecture

This site is engineered as a high-performance, zero-dependency **Single-Page Application (SPA)**. It completely avoids heavy JavaScript frameworks (like React or Vue) to ensure instantaneous load times, robust mobile responsiveness, and maximum SEO accessibility for academic web crawlers.

* **`index.html`** - The singular, core portfolio entry point housing the Hero, Research Identity & Impact, Hardware Deployments, Algorithm Simulations, Publications, and Career Timeline.
* **`*.pdf`** - Hosted professional dossiers directly accessible from the hero section:
  * Academic CV
  * Industry Resume
  * Research Statement
  * Full Publication Catalog

### Interactive UI Mechanics (Vanilla JS)
The frontend utilizes lightweight Vanilla JavaScript to execute fluid DOM manipulation without external library bloat:
* **Lazy-Load Video Injection:** Hardware and simulation demonstration videos display as static placeholder images, swapping to active YouTube `iframe` embeds only upon user click (`injectActiveStream`). This saves significant initial bandwidth.
* **Expandable Publication Drawer:** The publication catalog features an animated accordion (`togglePublications`) that dynamically reveals extended conference proceedings and preprints via CSS transitions (`drawer-anim`) without navigating away from the page.
* **Native Clipboard API:** Enables one-click BibTeX citation copying directly to the user's system clipboard (`copyBibtex`).
* **Responsive Mobile Drawer:** A native `toggleMenu` function handles the mobile navigation state, ensuring clean accessibility on smaller screens.

## 🛠️ Tech Stack & Integrations

* **Markup & Styling:** Native HTML5 & CSS3 (CSS Variables, Flexbox, CSS Grid, custom scroll-padding).
* **Interactivity:** Vanilla JavaScript (ES6) and DOM APIs.
* **Typography & Icons:** Native system fonts (`-apple-system`, `Segoe UI`) and FontAwesome 6.4.0.
* **SEO:** Integrated JSON-LD Schema markup mapping to ORCID and Google Scholar identities.
* **Robotics & Simulation Tools Showcased:** ROS/ROS 2, MATLAB & Simulink, Universal Robots RTDE, Stäubli LLI, and OptiTrack.

## 🚀 Local Deployment & Testing

To preview the website locally and test formatting changes before pushing to GitHub Pages, run a simple local HTTP server from the root directory:

```bash
# Clone the repository
git clone [https://github.com/mertcan-kaya/mertcan-kaya.github.io.git](https://github.com/mertcan-kaya/mertcan-kaya.github.io.git)

# Navigate to the project directory
cd mertcan-kaya.github.io

# Start a local web server (Python 3)
python3 -m http.server 8000
