# html5practical2
# HTML5 Practical Project - And the Mountains Echoed

This repository contains a personal website dedicated to my favorite book, *And the Mountains Echoed* by Khaled Hosseini. The site leverages semantic HTML5 for accessibility and structure, exploring the novel's themes of family, love, sacrifice, and generational connections.

## Pages

- **Home (index.html)**: Welcomes visitors with an introduction to *And the Mountains Echoed*, explaining why semantic HTML matters (clear structure, better discovery, accessible design, reader-friendly flow, and meaningful extras). Includes reasons for choosing the book and fun facts about its publication and author.
- **About (about.html)**: Details the history of *And the Mountains Echoed* (published in 2013, following Hosseini’s earlier works), its interconnected storytelling across generations and locations, and main themes (family bonds, love and sacrifice, separation, impact of decisions). Features a glossary of key terms and characters (e.g., Abdullah, Pari) using `<dl>`, plus reasons to recommend the book in an ordered list.
- **Media (media.html)**: Showcases a responsive book cover image using `<picture>` with `mountains-echoed-small.jpg`, `mountains-echoed-medium.jpg`, and `mountains-echoed-large.jpg`, an audio interview (`khaled-interview.mp3`) with `<audio>`, and a video trailer (`and-the-mountains-echoed-video.mp4`) with captions (`sample.vtt`) using `<video>`.
- **Extras (extras.html)**: Provides interactive elements including a `<table>` for a weekly reading schedule, `<details open>` for book insights on themes, `<dialog open>` with a quote, and `<progress>` and `<meter>` to track reading progress and emotional intensity.

## Design Decisions
- **Palette**: A mountain and literary-inspired color scheme with `--bg: #faf8f5` (warm cream background), `--fg: #2a2a2a` (dark gray text), `--brand: #1e7a8c` (vibrant teal for mountains), and `--accent: #d97706` (warm amber for warmth/sacrifice). Dark mode overrides use `--bg: #1a1a1a` and `--brand: #3b9db0` for contrast.
- **Type Scale**: A modular scale with `--h1: 2.75rem`, `--h2: 2rem`, `--h3: 1.5rem`, and `--body: 1.125rem`, using `Montserrat` (sans-serif for headings), `Merriweather` (serif for body), and `Courier New` (monospace for code).
- **Spacing Scale**: Multiples of 0.5rem for vertical rhythm: `--space-1: 0.5rem`, `--space-2: 1rem`, `--space-3: 1.5rem`, `--space-4: 2rem`, `--space-5: 3rem`.
- **Components**: Includes cards with staggered slide-in animations, responsive tables with striped rows, media elements with shadows, and accordions using `details/summary`.

## Accessibility Notes
- **Contrast Choices**: Ensures WCAG AA compliance with high contrast ratios (e.g., `--fg: #2a2a2a` on `--bg: #faf8f5`, adjusted in dark mode to `--fg: #e5e5e5` on `--bg: #1a1a1a`).
- **Focus Styles**: Visible focus indicators with `outline: 3px solid var(--accent)` on interactive elements (e.g., `nav a:focus`, `summary:focus`).
- **Reduced Motion Handling**: `@media (prefers-reduced-motion: reduce)` disables animations (e.g., sets `animation-duration: 0.01ms`) and resets card animations for users with vestibular disorders.

## Docker
- **Build Command**: `docker build -t marshanjami/html5-css3-site:lab2 .`
- **Run Command**: `docker run --rm -p 8080:80 marshanjami/html5-css3-site:lab2`
- **Push Command**: `docker push marshanjanmi/html5-css3-site:lab2`
- **Tag Command**: `docker tag marshanjami/html5-css3-site:lab2 marshanjami/html5-css3-site:latest`
- **Push Command**: `docker push marshanjami/html5-css3-site:latest`

