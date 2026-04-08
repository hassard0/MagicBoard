# MagicBoard ✨

An AI-powered infinite whiteboard for generating, arranging, and annotating Mermaid diagrams — all from natural language prompts.

## Features

- **AI Diagram Generation** — Click the ✨ Magic button, describe what you want, and an AI-generated Mermaid diagram appears on the canvas.
- **Infinite Canvas** — Pan and zoom freely. Drag diagrams anywhere. The canvas scales to fit your thinking.
- **Freehand Drawing** — Sketch annotations directly on the canvas with adjustable brush size and color.
- **Background Images** — Upload a PNG/JPEG as a semi-transparent backdrop for tracing or context.
- **Light / Dark Mode** — Full theme support. Diagrams and canvas re-render automatically when you toggle.
- **Export** — Download your board as a PNG snapshot.

## How It Works

1. **Prompt → Mermaid** — Your description is sent to a backend function (`generate-mermaid`) which uses an AI model to produce valid Mermaid syntax.
2. **Mermaid → SVG** — The Mermaid library renders the syntax into an SVG in-browser, themed to match your current light/dark mode.
3. **SVG → Canvas** — The SVG is drawn onto an HTML5 `<canvas>`, composited with your drawings, background image, and other diagrams.
4. **Interact** — Drag to reposition diagrams, draw freehand annotations, pan/zoom the viewport, or generate more diagrams to build out your board.

## Tech Stack

- **React 18** + **TypeScript** + **Vite**
- **Tailwind CSS** + **shadcn/ui**
- **Mermaid.js** for diagram rendering
- **Framer Motion** for UI animations
- **Lovable Cloud** (backend functions + AI gateway)

## Getting Started

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) and click the ✨ button to create your first diagram.
