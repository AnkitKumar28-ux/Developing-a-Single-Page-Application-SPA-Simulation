# Week 5 Task: Single Page Application (SPA) Simulation — NexusFlow

A complete, zero-dependency **Single Page Application (SPA) Simulation** built with semantic HTML5, modern CSS3, and vanilla ES6+ JavaScript.

## Quick Start

1. **Option A — Direct Browser Launch (`file://` safe):**
   Double-click [`index.html`](./index.html) to open the application directly in any modern browser (Chrome, Edge, Firefox, Safari).
2. **Option B — Local HTTP Server:**
   Run any static server inside this directory:
   ```bash
   npx serve .
   # or
   python -m http.server 8080
   ```

## Deliverables Checklist

| Deliverable | File Path | Description |
| :--- | :--- | :--- |
| **Main HTML Container** | [`index.html`](./index.html) | Persistent SPA shell with sidebar navigation, History API controls, route address bar, and `#app-view` dynamic container. |
| **Uniform CSS Stylesheet** | [`css/styles.css`](./css/styles.css) | Dark/Light theme variables, responsive grid layout, top progress bar, skeleton shimmer animations, and `.view-enter`/`.view-exit` transitions. |
| **Client-Side Router** | [`js/router.js`](./js/router.js) | Custom router using `history.pushState()`, `history.replaceState()`, `popstate` events, parameterized routes (`/projects/:id`), and race-condition protection. |
| **Reactive State Store** | [`js/store.js`](./js/store.js) | Centralized Pub/Sub state container with `fetch("data/mock-data.json")`, `file://` fallback, and `localStorage` persistence. |
| **Dynamic View Controllers** | [`js/views.js`](./js/views.js) | View templates & interactive controllers for Dashboard, Projects, Project Detail, Task Board, Analytics, SPA Telemetry, 404 Not Found, and 503 Error Boundary. |
| **Application Entry Point** | [`js/app.js`](./js/app.js) | Application bootstrapper, global event delegation, theme toggle, latency simulator, and quick search jump. |
| **External JSON Data** | [`data/mock-data.json`](./data/mock-data.json) | Mock dataset loaded asynchronously on startup. |
| **Technical Report** | [`TECHNICAL_REPORT.md`](./TECHNICAL_REPORT.md) | Comprehensive architectural report detailing the project plan, routing design, state management, and implementation challenges. |
| **Project ZIP Archive** | `week5-spa-simulation.zip` | Complete packaged archive ready for submission. |
