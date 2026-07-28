# MotionFeed Keyword Animation Engine

A dependency-free, single-page HTML visual engine that generates full-screen animated story backgrounds from headlines, summaries and keywords.

It is designed as an image replacement for vertical news and social feeds. The engine maps semantic themes—such as weather, AI, finance, sport, travel and nature—to large canvas/CSS animations. Unmatched subjects receive deterministic abstract fallback visuals, so every feed story has a usable animation.

## Features

- Single standalone `index.html`
- No build step or external dependencies
- Responsive full-screen and 9:16 mobile layout
- Keyword, phrase and combination matching
- Detailed weather animation states
- AI, LLM, agent, automation and robotics themes
- Broad news category coverage
- Deterministic fallback animations for unmatched keywords
- Built-in story editor, demo navigation and playback controls
- URL query parameter integration

## Run locally

Open `index.html` directly in a modern browser, or serve the directory:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Feed integration

Pass content through query parameters:

```text
index.html?headline=AI%20agents%20are%20changing%20work&keywords=AI,agent,automation,LLM&summary=New%20tools%20can%20plan%20and%20complete%20multi-step%20tasks
```

Supported parameters:

- `headline`
- `keywords` — comma-separated
- `summary`

## Fallback visuals

When no named category matches, the engine selects one of several content-sensitive deterministic animations:

- Orbit
- Wave
- Signal
- Bloom
- Pulse grid

The same text produces the same fallback family and particle layout.

## Project structure

```text
.
├── index.html
├── README.md
├── LICENSE
└── .gitignore
```

## Licence

MIT
