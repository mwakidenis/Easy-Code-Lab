# EasyCodeLab 

An interactive, browser-based learning tool that helps complete beginners build mental models around HTML and CSS through visual, hands-on exercises.

Built for students fresh out of high school who have never written a line of code. No prior knowledge required.

## Modules

### Tag Builder

Learn HTML and CSS syntax by building tags piece by piece. Fill in the blanks, see your tags visualized as colorful nested boxes, and watch a live preview update as you type.

- 9 progressive lessons covering HTML tags, nesting, attributes, links, images, lists, and CSS basics
- Gap-fill exercises for guided learning
- Free-edit coding with live preview
- Real-time tag tree visualization

### Box Model Explorer

Understand the CSS box model through interactive 3D visualization. Adjust padding, margin, and border with sliders and see changes in real time.

- 6 lessons from content box to combined layouts
- Interactive 3D view powered by Three.js
- 2D Chrome DevTools-style overlay
- "Match the target" challenges

## Tech Stack

- **Next.js 16** — App Router, static generation
- **React 19** — `useDeferredValue`, `startTransition` for responsive typing
- **Three.js** — 3D box model visualization via `@react-three/fiber` + `@react-three/drei`
- **CodeMirror 6** — Code editor with syntax highlighting
- **Motion** — UI animations and transitions
- **IndexedDB** — Persistent progress storage (no backend required)
- **Tailwind CSS v4** — Custom color theme with playful design tokens

## Getting Started

```bash
# Install dependencies
npm install

# Start the dev server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to start learning.

## Project Structure

```text
src/
├── app/                    # Next.js App Router pages
│   └── (modules)/          # Tag Builder & Box Model routes
├── components/
│   ├── editor/             # CodeEditor, GapFillEditor, HtmlPreview
│   ├── tag-builder/        # TagVisualizer, TagBuilderLesson
│   ├── box-model/          # 3D canvas, 2D overlay, controls
│   ├── layout/             # Header, LessonStepper, InstructionPanel
│   └── ui/                 # Button, Slider, Card, etc.
├── content/                # Lesson definitions (typed TypeScript)
├── hooks/                  # useLessonProgress, useCodeValidation, useIndexedDB
├── lib/                    # HTML parser, tag validator, lesson engine
├── stores/                 # Zustand stores
└── types/                  # TypeScript type definitions
```

## Build 

see 👉[build](https://github.com/mwakidenis/Easy-Code-Lab/blob/main/README.md)
