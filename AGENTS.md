# Repository Guidelines

This repository hosts a single-page static portfolio site. Keep changes small, readable, and easy to test locally.

## Project Structure & Module Organization
- Root files: `index.html`, `style.css`.
- Assets: images live in `assets/` (e.g., `assets/python-logo.png`). Reference as `assets/<name>`.
- No build system or runtime dependencies.

## Build, Test, and Development Commands
- Serve locally (Python): `python -m http.server 8000` then open `http://localhost:8000/index.html`.
- Serve locally (Node): `npx serve .` or `npx http-server .`.
- Open directly: double-click `index.html` (note: some fonts/icons may require a server).

## Coding Style & Naming Conventions
- Indentation: 2 spaces for HTML/CSS.
- HTML: semantic tags where possible; lowercase attributes; double quotes for attribute values.
- CSS: group related rules; use lowercase, hyphen-separated class names (e.g., `.project-card`).
- Filenames: prefer lowercase-kebab-case for new files (e.g., `my-image.png`). Keep existing names stable.

## Testing Guidelines
- Visual pass: verify navbar links, sections, images, and responsiveness (desktop and mobile widths).
- Validation: run HTML/CSS validators (e.g., W3C) and Lighthouse for accessibility and performance.
- Links: confirm external links (GitHub, LinkedIn, Twitter) open in new tabs and are correct.

## Commit & Pull Request Guidelines
- Commits: concise, imperative subject line (<= 72 chars). Example: `Update projects section layout`.
- Group related changes; avoid mixing refactors with content edits.
- Pull Requests should include: brief description, before/after screenshots for UI changes, and any manual test notes.

## Security & Configuration Tips
- No secrets should be committed. External resources (Google Fonts, Font Awesome CDN) are loaded via HTTPS.
- If adding JS or third-party libraries, pin versions and avoid inline scripts where possible.

## Agent-Specific Instructions
- Do not introduce frameworks unless requested. Favor minimal, dependency-free changes.
- Keep styles consistent; prefer extending existing classes over adding many new ones.
- If adding a build step, document commands here and keep the default no-build path working.
