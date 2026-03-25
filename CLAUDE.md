# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a collection of browser-based games built as standalone HTML files. Each game is fully self-contained — HTML, CSS, and JavaScript all live in a single `.html` file with no build step, no dependencies, and no server required. Open any file directly in a browser to play.

## Architecture

Each game file follows the same pattern:
- **CSS** in a `<style>` block in `<head>` — dark-themed UI with smooth transitions
- **HTML** in `<body>` — minimal markup, state driven by JS
- **JavaScript** in a `<script>` block at the end of `<body>` — vanilla JS only, no frameworks or libraries

### Current games
- `spinbottle.html` — Spin the Bottle: players added via UI, bottle spins using `requestAnimationFrame` with easeOut, wheel drawn on `<canvas>`, bottle is an inline SVG rotated via CSS transform
- `tictactoe.html` — Xs & Os: two-player local game with win detection, persistent score counter across rounds

## Git Workflow

**Commit and push to GitHub after every meaningful unit of work** — after adding a feature, fixing a bug, or completing any discrete change. Never leave work uncommitted at the end of a task. This ensures we can always revert to a known good state and never lose progress.

Commit messages should be concise and descriptive, explaining what changed and why:

```bash
git add <file>
git commit -m "short description of what changed and why"
git push
```

Remote: `https://github.com/evancarroll15/claude-code-projects`
