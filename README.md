# Saurabh Lohia - Portfolio Website

Official GitHub profile repository showcasing my tech stack, featured projects, work experience, education, certifications, and resume. Built as a dependency-free static site with plain HTML, CSS, and JavaScript, so it runs in any browser and deploys to Vercel with zero configuration.

## Live Demo

> Add the Vercel URL here after deployment, for example: `https://saurabh-lohia.vercel.app`

## Project Structure

```
portfolio/
├── index.html      # Page structure and content (HTML)
├── css/
│   └── style.css   # All styling: theme, layout, animations, responsive rules (CSS)
├── js/
│   └── main.js     # Interactivity: mobile menu, scroll effects, reveal animations (JavaScript)
├── resume.pdf      # Resume served by the "Download resume" button
└── README.md       # This file
```

Each layer lives in its own file:

| File | Language | Responsibility |
| --- | --- | --- |
| `index.html` | HTML5 | Semantic sections: hero, about, skills, experience, projects, education, certifications, contact, footer |
| `css/style.css` | CSS3 | Design tokens as CSS variables, dark theme, grid and flexbox layouts, hover effects, responsive breakpoints, reduced-motion support |
| `js/main.js` | Vanilla JavaScript (ES5-style IIFE) | Header shadow on scroll, mobile navigation toggle, `IntersectionObserver` scroll reveals, auto-updating footer year |

## Sections

1. **Hero:** name, role, short intro, call-to-action buttons, and key stats.
2. **About:** bio and a quick-facts card (education, focus area, current role).
3. **Skills:** grouped into Languages, Frontend, Backend, Data, Cloud & DevOps, and AI.
4. **Experience:** timeline of internships at Small Fare (Full Stack Developer Intern) and Cognifyz IT (Java Development Intern).
5. **Projects:**
   - **Earnity:** AI-enhanced student earning and career platform (Java, Firebase, AI tools).
   - **DevCollab:** real-time collaborative coding platform with an AI pair-programming assistant (React, Node.js, Socket.IO, Redis, Docker).
6. **Education & Certifications:** B.Tech in Computer Science (IIMT University) and CBSE Class X and XII results, plus three NPTEL certifications.
7. **Contact:** email, GitHub, LinkedIn, and phone.

## Features

- Fully responsive layout for phones, tablets, and desktops
- Sticky header with a blur effect that appears on scroll
- Mobile hamburger menu that closes after you pick a link
- Smooth scrolling between sections
- Fade-and-slide animations as sections enter the viewport
- Respects the `prefers-reduced-motion` setting and turns off animations when it's set
- Keyboard focus styles and a skip-to-content link for accessibility
- Semantic HTML with a meta description, for better search indexing
- No frameworks, build step, or npm packages

## Tech Stack

- **Markup:** HTML5
- **Styling:** CSS3 (custom properties, Grid, Flexbox)
- **Scripting:** Vanilla JavaScript
- **Fonts:** Google Fonts (Syne, Inter, JetBrains Mono), loaded via `<link>` in `index.html`
- **Hosting:** Vercel (static deployment)
- **Version control:** Git and GitHub

## Running Locally

No installation is needed.

**Option 1: open the file directly**

Double-click `index.html`, or open it from your browser's File menu.

**Option 2: run a local server (recommended)**

```bash
cd portfolio
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying to Vercel

1. Push this repository to GitHub.
2. Sign in at [vercel.com](https://vercel.com) with your GitHub account.
3. Click **Add New → Project** and import the repository.
4. Leave the framework preset as **Other** and leave the build and output settings empty. Vercel serves the root folder as a static site.
5. Click **Deploy**.

After the first deploy, every push to the `main` branch triggers an automatic redeploy.

## Customizing

| What to change | Where |
| --- | --- |
| Name, role, intro, stats | `index.html`, hero section |
| Bio and quick facts | `index.html`, about section |
| Skills and tags | `index.html`, skills section (`<ul class="chips">` items) |
| Experience entries | `index.html`, experience section (`<article class="timeline-item">`) |
| Projects | `index.html`, projects section (`<article class="project-card">`) |
| Live links and GitHub links | `href` values on the project and contact links |
| Colors and fonts | `css/style.css`, `:root` block at the top (CSS variables) |
| Resume | Replace `resume.pdf` with an updated file of the same name |

## Known Items to Update

- **DevCollab live link:** the "Live" button is a placeholder (`href="#"`) and needs the deployed URL.
- **Earnity link:** currently points to the GitHub profile. Replace it with the direct repository URL.

## Author

**Saurabh Lohia**
- GitHub: [@SAURABHLOHIA24](https://github.com/SAURABHLOHIA24)
- LinkedIn: [linkedin.com/in/saurabhlohia0014](https://linkedin.com/in/saurabhlohia0014)
- Email: Saurabhlohia0014@gmail.com

## License

This project is for personal use. All content, including the resume and project descriptions, belongs to Saurabh Lohia.
