[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/YDjuDFNG)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23181263&assignment_repo_type=AssignmentRepo)
# Portfolio Website - Zetu Kuluvuyo Zide

This is a multipage portfolio built with HTML and CSS. This projects involved taking broken incomplete starter codebase and debugging, completing and styling it to meet proffessional and accessibility standards and the specified requirements. 

> **NB:**  Please note that the project section might not be truthful with regards to the projects and their tags i.e. both the Housekeepers Platform and Quote of the day didn't use HTML, CSS and JavaScript only but for the purposes of this assignment and learning scope, I've labeled them as such. And that the information provide here is in the scope of the current learning journey. Here is a [link](https://portfolio-guavz.vercel.app/) to my full portfolio.

---

## Technologies Used
 
- **HTML5** — semantic markup, accessibility attributes, form validation
- **CSS3** — custom properties, flexbox, responsive media queries, animations
- **Figma** — low-fidelity wireframe design (see `design/Wireframe.pdf`)
- **Git & GitHub** — version control and submission via GitHub Classroom

---

## Pages
 
| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Landing page with hero section and service highlights |
| About | `about.html` | Bio, skills table, and certifications |
| Projects | `projects.html` | Showcase of three projects with descriptions and tags |
| Contact | `contact.html` | Contact form with validation and accessibility features |
 
---

## Additional Documentation

Inside the design folder you will find the following files that were a major contribution to the completion of this portfolio website: 
- Issues-identifed.pdf - this file contains all the issues that I identified from the starter code. 
- Wirefram.pdf - this files contains screenshots of a low fidelity wireframe that I designed as a template for my website. This wireframe was designed on Figma. 

---

## Validation Results
 
All four HTML pages and the CSS stylesheet were validated using the W3C validators:
 
- **HTML** — validated using the [W3C Markup Validation Service](https://validator.w3.org/). All pages passed with no errors.
- **CSS** — validated using the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/). The stylesheet passed with no errors.

---

## How to View Locally
 
1. Clone or download this repository to your computer
2. Open the project folder — you should see `index.html`, `about.html`, `projects.html`, `contact.html`, a `css/` folder, a `design/` folder, a `screenshots/` folder, and an `images/` folder
3. Double-click `index.html` to open it in your browser
4. Use the navigation menu to move between pages

---

## Screenshots

Home Page
![Home Page](<screenshots/home page.png>)

About Page
![About Page](<screenshots/about page.png>)

Projects Page
![Projects Page](<screenshots/projects page.png>)

Contact Page
![Contact Page](<screenshots/contact page.png>)

---

## Known Issues
 
A full breakdown of all issues identified and resolved during this project is documented in `design/Issues-identified.pdf`. The following is a summary of the key issues found in the starter code and how they were addressed:
 
**HTML Issues**
- All four pages were missing a navigation menu, meaning users had no way to move between pages — fixed by building a consistent `<nav>` bar across all pages
- All pages used non-semantic elements instead of `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>`, replaced throughout
- Images were missing `alt` attributes, making them inaccessible to screen readers, I added descriptive alt text to all images
- The About page table was absent (only a comment placeholder existed), built from scratch with `<thead>`, `<tbody>`, `<th scope>`, and a `<caption>`
- The Projects page was missing a third project, I added it
- The contact form had no labels, incomplete input types, and no validation attributes; the email field was incorrectly typed as `text`, corrected and expanded
- All pages were missing `<meta charset>`, `<meta viewport>`, `<meta description>`, and the `lang` attribute on `<html>`, I added them to all pages
**CSS Issues**
- Only two selector types were used (element and class); requirements called for five or more, expanded to include ID, descendant, grouped, and pseudo-class selectors
- No pseudo-classes were present, added `:hover`, `:focus`, and `:nth-child`
- Navigation, table, and form styling were all missing, I added full styles
- Colour contrast failed the 4.5:1 accessibility ratio, I corrected throughout
- The footer was left-aligned, I centred it
- No box model usage (no meaningful padding, margin, or borders), I applied consistently across all sections
- No layout system, I implemented flexbox across all major sections
- No responsive design, I added media queries for tablet (`max-width: 768px`) and mobile (`max-width: 480px`)
**Remaining known limitations**
- The contact form is static and does not submit data, no back-end or form service is connected
- Autocomplete on form fields works only when the site is served over a proper connection; it does not trigger when opening the file locally via `file:///`

---

## Reflection
 
This project gave me a much clearer picture of what it takes to build a complete, standards-compliant website from a broken starting point rather than from scratch. Debugging someone else's code required me to slow down and read carefully before changing anything, which is a skill I found myself developing as the project progressed.
 
The accessibility requirements were the most challenging part. Adding things like `aria-current`, and `aria-live` regions felt unfamiliar at first, but understanding the reasoning behind them, that real users rely on these to navigate, made them feel purposeful rather than just checklist items.
 
If I were to continue improving this project, I would connect the contact form to a real submission service, add a dark mode toggle, and explore using CSS custom properties more consistently throughout the stylesheet to make future style changes easier to manage.