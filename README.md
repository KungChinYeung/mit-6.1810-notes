# MIT 6.1810 — Lecture Notes (Modern Web Edition)

A modern, self-contained HTML rendering of the **MIT 6.1810 Operating System Engineering**
(Fall 2026) lecture notes — starting with **Lecture 1: O/S Overview**.

The content is adapted from the official lecture outline
[`l-overview.txt`](https://pdos.csail.mit.edu/6.1810/2026/lec/l-overview.txt),
rewritten as an interactive, beautifully typeset web page.

## ✨ Features

- **Tailwind CSS** design system with custom typography
  (Space Grotesk / Inter / JetBrains Mono)
- **Dark / light theme** toggle, persisted in `localStorage` (no flash on load)
- Animated **aurora** background and gradient accents
- **Reading progress bar** and scroll-reveal animations
- Sticky **table of contents** with scroll-spy highlighting
- **Syntax-highlighted code** (highlight.js) with a theme-aware token palette
- **One-click copy** buttons on every code block
- Fully **responsive** — collapsible layout on mobile
- Single file, no build step, opens directly in a browser

## 📁 Structure

```
lec/
├── index.html        # the whole page (self-contained)
├── examples/         # the 9 example programs from Lecture 1
│   ├── ex1.c         # copy input to output
│   ├── ex2.c         # create a file
│   ├── ex3.c         # fork()
│   ├── ex4.c         # exec()
│   ├── ex5.c         # fork + exec + wait
│   ├── ex6.c         # output redirection
│   ├── ex7.c         # pipe()
│   ├── ex8.c         # IPC over a pipe
│   ├── ex9.c         # list a directory
│   └── echo.c        # reading argv
└── README.md
```

## 🚀 Viewing

Just open `index.html` in a browser:

```bash
# Option 1: local server (recommended)
python3 -m http.server -d . 8000
# then visit http://localhost:8000

# Option 2: open the file directly
xdg-open index.html
```

> An internet connection is used only to load Tailwind CSS, highlight.js and
> Google Fonts from their CDNs. The page content itself is fully local.

## 📚 Topics covered (Lecture 1)

- What an operating system is — the software layer between applications and hardware
- Goals: multiplex, isolate, share, abstract
- Conflicting design constraints: performance, generality, power, security
- Course structure, labs, and grading (65% / 30% / 5%)
- The user-space / kernel / hardware model and the system-call mechanism
- Nine hands-on system-call examples on **xv6**

## 🙏 Attribution

Lecture content © MIT PDOS, from the public 6.1810 course materials.
This is an unofficial, personal re-formatting for study purposes.
