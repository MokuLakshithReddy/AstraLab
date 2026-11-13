# AstraLab — Interactive Science Learning Modules

[![Forks](https://img.shields.io/github/forks/MokuLakshithReddy/AstraLab?style=flat-square)](https://github.com/MokuLakshithReddy/AstraLab/forks) [![Open Issues](https://img.shields.io/github/issues/MokuLakshithReddy/AstraLab?style=flat-square)](https://github.com/MokuLakshithReddy/AstraLab/issues)


A browser-based collection of interactive science and classroom learning pages. The repository is built from standalone HTML modules, with a shared cyber-terminal visual style and a dashboard that links learners to individual simulations.

[![HTML](https://img.shields.io/badge/HTML-5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind%20CDN-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Stars](https://img.shields.io/github/stars/MokuLakshithReddy/AstraLab?style=flat-square)](https://github.com/MokuLakshithReddy/AstraLab/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/MokuLakshithReddy/AstraLab?style=flat-square)](https://github.com/MokuLakshithReddy/AstraLab/commits/main)

## Explore the repository

| Page | Learning interaction |
|---|---|
| [dashboard.html](dashboard.html) | Module selection dashboard |
| [titration.html](titration.html) | Add titrant and observe a changing pH display and titration curve |
| [optics.html](optics.html) | Adjust incidence angle and refractive index to explore Snell's law |
| [ohms.html](ohms.html) and [ohms_law.html](ohms_law.html) | Ohm's law learning pages |
| [atomic.html](atomic.html) | Atomic-science module |
| [friction.html](friction.html) | Friction module |
| [logic.html](logic.html) | Logic module |

## Learner flow

~~~mermaid
flowchart TD
    A["Open AstraLab"] --> B["Enter the learning interface"]
    B --> C["Choose a module from the dashboard"]
    C --> D["Read the safety / module guidance"]
    D --> E["Change simulation controls"]
    E --> F["Observe visual or chart feedback"]
    F --> G["Try another value or module"]
~~~

## Implementation notes

- Standalone HTML pages with JavaScript interactions.
- Tailwind CSS is loaded from its CDN in the pages.
- The titration page uses Chart.js to plot pH against added volume.
- The optics page uses a canvas for the ray / refraction visualization.
- Several modules include a safety acknowledgement screen before the activity.

The repository currently contains no automated test suite, published accuracy benchmark, or verified performance evaluation. The interactive simulations should be treated as educational visualizations, not laboratory instruments or substitutes for supervised practical work. The interface includes an assistant-style widget in some modules; this README does not claim a validated AI model backend.

## Run locally

Because this is a static HTML project, open [index.html](index.html) in a modern browser. For consistent local routing, you can also serve the folder with a static development server, for example:

~~~bash
python -m http.server 8000
~~~

Then visit http://localhost:8000.

## Why it matters

Interactive visual models give students a way to change inputs and immediately see how a scientific relationship responds, making abstract concepts easier to explore before or after a supervised lesson.
