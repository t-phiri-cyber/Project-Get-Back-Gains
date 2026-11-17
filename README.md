# Project Get Back Gains 🥊

A responsive countdown and weekly training tracker built for the Handshake challenge. The experience counts down to **20 January 2027** and presents a seven-day training plan with wrist-safe and full-return phases.

## Live demo

After deployment, the site will be available at:

`https://YOUR-GITHUB-USERNAME.github.io/project-get-back-gains/`

Replace `YOUR-GITHUB-USERNAME` with the GitHub account that owns the repository. The URL will not work until GitHub Pages has been enabled and its first deployment has completed.

## Features

- Live days, hours, minutes and seconds countdown to 20 January 2027 (midnight UK time).
- Seven-day Monday–Sunday training schedule.
- Toggle between the wrist-safe phase and the full-return phase.
- Mark sessions complete and view weekly completion progress.
- Weekly progress is stored locally in the browser using `localStorage`.
- Add the target date to a calendar using a downloadable `.ics` file.
- Responsive layout for mobile and desktop.
- Accessibility features including semantic sections, labelled controls and timer labelling.

## Project structure

```text
project-get-back-gains/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── .nojekyll
├── index.html
├── styles.css
├── script.js
└── README.md
```

## Run locally

No build tools, package installation or backend are required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. For a local web server, run `python -m http.server 8000` from the project directory and visit `http://localhost:8000`.

## Deploy with GitHub Pages

This repository includes a GitHub Actions workflow that publishes the static site whenever changes are pushed to the `main` branch.

1. Create a **public** GitHub repository named `project-get-back-gains`.
2. Upload the contents of this project folder to the repository root (not the enclosing folder). Ensure `index.html`, `styles.css`, `script.js`, `.nojekyll`, `README.md` and `.github/workflows/deploy.yml` are present.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, select **GitHub Actions** as the source.
4. Open the **Actions** tab and wait for the `Deploy to GitHub Pages` workflow to complete successfully.
5. Your public website URL will be `https://YOUR-GITHUB-USERNAME.github.io/project-get-back-gains/`. Copy that URL into the Handshake challenge.

If the workflow does not start automatically, check that GitHub Actions are enabled for the repository and that the workflow file is on the `main` branch.

## Technology

- HTML5 for semantic page structure.
- CSS3 for responsive styling and layout.
- Vanilla JavaScript for the countdown, phase selector, weekly tracker and calendar export.
- Browser `localStorage` for local progress persistence.
- GitHub Actions and GitHub Pages for static hosting and deployment.

## Important behaviour and limitations

- The countdown uses the fixed target instant `2027-01-20T00:00:00Z` (midnight GMT / UK time on the target date).
- The tracker stores progress in the current browser on the current device. It does not sync across devices or browsers. Clearing browser storage may erase saved progress.
- The full-return phase is a selectable programme view, not a medical clearance. The target date is not proof that an injury has healed. Resume impact, heavy loading or sparring only when symptoms and appropriate clinical guidance permit.
- This is a static front-end project. It does not collect personal data or require a server/database.

## Handshake submission description

**Project Get Back Gains** is a responsive training countdown and habit-tracking web app. It combines a live countdown to 20 January 2027 with a seven-day training schedule, selectable wrist-safe and full-return training phases, weekly completion tracking and calendar export. Built with HTML, CSS and vanilla JavaScript, the project runs entirely in the browser and is deployed as a static site using GitHub Pages.
