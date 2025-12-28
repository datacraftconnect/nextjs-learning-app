# Next.js Learning Workspace

This workspace is designed for a structured, step-by-step approach to learning core Next.js concepts.

## Structure Overview

- **/nextjs-learning-app**: This directory contains a single, complete Next.js application. Using one app avoids redundant installations and keeps the environment clean.
- **/nextjs-learning-app/app**: This is the heart of the project. Each sub-folder within `app` is a dedicated module for a specific Next.js concept.
- **Numbered Prefixes**: The folders are numbered to provide a recommended learning order, starting with fundamentals and progressing to more advanced topics.
- **README.md Files**: Every concept folder contains a `README.md` file that explains the concept, its purpose, use cases, and how it compares to traditional React (Vite) development.

## How to Use This Workspace

1.  **Installation**:
    -   Navigate into the `nextjs-learning-app` directory.
    -   Run `npx create-next-app@latest .` to initialize a new Next.js project in the *current* directory. Choose the recommended defaults (TypeScript, ESLint, Tailwind CSS).
    -   The installer will populate the directory with the necessary files (`package.json`, `next.config.js`, etc.).

2.  **Learning Flow**:
    -   Follow the numbered folders in the `app` directory, starting with `01-project-setup`.
    -   Read the `README.md` in each folder to understand the concept.
    -   Create `page.tsx`, `layout.tsx`, and other files inside the concept folder to experiment with the feature.
    -   To see your work, run the development server (`npm run dev`) and navigate to the corresponding URL (e.g., `http://localhost:3000/01-project-setup`).

## Best Practices for a Clean Workspace

-   **Stay in the `app` Directory**: All learning experiments should happen inside the concept folders within `/app`. Avoid cluttering the root directory.
-   **Main Navigation**: You can modify the root `app/page.tsx` file to create a main menu or a table of contents that links to each learning module.
-   **Isolate Experiments**: Try to keep the code for each concept self-contained within its respective folder. This makes it easier to review and understand later.
-   **Read the Docs**: Use the official Next.js documentation alongside these exercises for a deeper understanding. These modules are a guide, not a replacement for the docs.
