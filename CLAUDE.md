# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Nudgy is a static landing page for a mobile app that sends humorous screen time reminders. The entire site is a single `index.html` file with inline CSS and JavaScript — no build system, no dependencies, no package manager.

## Development

To develop locally, serve `index.html` with any static file server:

```bash
# Using Python
python3 -m http.server 8000

# Or open directly in browser
open index.html
```

There are no build, lint, or test commands — changes are made directly to `index.html`.

## Architecture

- **Single file:** All markup, styles, and scripts live in `index.html`
- **No frameworks:** Pure HTML5, vanilla CSS, vanilla JavaScript
- **Dark theme:** Black background (#0a0a0a) with amber-to-red gradient accents (#f59e0b → #ef4444)
- **Responsive:** Mobile-first layout using Flexbox/Grid with a breakpoint at 500px
- **Animations:** CSS keyframe animations with staggered delays for notification demos

## Key Sections in index.html

1. **Hero** — "Coming Soon" badge, headline with gradient text, subtitle
2. **Notification demos** — Animated example notifications showing the app's roasting messages
3. **Email signup form** — Captures email; currently only logs to console (no backend)
4. **Features grid** — Three feature cards (Custom Timers, Mean Notifications, No Blocking)
5. **Footer**

## Current Limitations

- Form submission logs email to console only — needs backend integration for actual email capture
- No version control initialized yet
