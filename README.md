  # Personal Website Project — Elnatan Teaghes

  This repository contains a simple personal profile website created for the WECIB CTI.110 Personal Website Project (PWP) Part 2. The site demonstrates basic HTML structure, responsive CSS styling, and accessible navigation across three pages: the home page (`index.html`), an interests page (`interests.html`), and a contact page (`contact.html`).

  **Status:** Completed — basic layout, navigation, footer, and responsive behavior implemented.

  ## Features
  - Header with site title and navigation (Home / Interests / Contact)
  - Top profile row with a profile picture and name
  - Three-column content layout under the top row (Skills | About Me | Projects); middle column is larger
  - Responsive behavior: columns stack on small screens
  - Footer with contact email and copyright
  - Centralized CSS in `styles.css` with a defined color palette and typography

  ## Files
  - `index.html` — Home page (profile, skills, projects, bio)
  - `interests.html` — Interests page (hobbies and interests)
  - `contact.html` — Contact page (email, LinkedIn, GitHub links)
  - `styles.css` — Main stylesheet (layout, palette, responsive rules)
  - `README.md` — This file

  ## Color Palette & Typography
  The project uses a small, coherent color palette defined as CSS variables inside `styles.css`.

  - Light background: `--light` (light, neutral background)
  - Light accent: `--light-accent` (soft card/background accent)
  - Brand color: `--brand` (primary action / links color)
  - Dark accent: `--dark-accent` (header / darker accents)
  - Primary text: `--dark` (main readable text color)

  Typography uses system/web-safe fonts for consistent rendering:
  - `"Segoe UI", Tahoma, Geneva, Verdana, sans-serif` as the main font-family.

  Font sizes follow a readable scale (CSS uses pixel units for headings and `.name` as required by the assignment).

  ## Layout Details
  - The header sits at the top with a gradient background.
  - The profile row (`.top-row`) contains the circular profile image and the name/title on a single horizontal row.
  - The main content area uses a Flexbox three-column layout inside `section#Profile`:
    - Left column: `#skills` (flex: 1)
    - Center column: `#bio` (flex: 2 — larger)
    - Right column: `#projects` (flex: 1)
  - Responsiveness: at widths <= 900px the three columns stack vertically.

  ## How to view locally
  1. Clone the repo (if not already):

  ```powershell
  git clone <repo-url>
  ```

  2. Open `index.html` in your browser. You can double-click the file or run a local static server. For a quick server (PowerShell):

  ```powershell
  # From the repository folder
  python -m http.server 8000 ; Start-Process "http://localhost:8000/index.html"
  ```

  3. Alternatively, just open `index.html` directly in your browser.

  ## Git workflow (recommended commits used during development)
  - `git add .`
  - `git commit -m "Add navbar, footer, and responsive styles"`
  - `git push`

  ## Notes and Next Steps
  - If you'd like, I can:
    - Make the navigation sticky to the top of the page.
    - Adjust typography to match specific font-size recommendations from your instructor.
    - Add alt text improvements or more accessibility features (ARIA labels, skip links).
    - Replace the placeholder profile image with an optimized/accessible image.

  ## Credits
  Author: Elnatan Teaghes

  Instructor: Mr. Gardner (WECIB)

  ---