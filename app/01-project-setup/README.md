# Concept: Project Setup & App Router Basics

This module covers the initial setup of a Next.js project and the fundamental principles of the App Router.

### What is the App Router?

The App Router is the new routing system in Next.js (from version 13 onwards). It's a paradigm shift from the previous `pages` directory router. It is built on top of React Server Components and supports shared layouts, nested routing, loading states, and error handling. Every folder inside the `app` directory becomes a route segment in the URL.

### Why does it exist?

The App Router was created to address the limitations of the original `pages` router and to better align with modern React features, especially Server Components. It aims to provide:

-   **Better Performance**: By leveraging Server Components, much of the rendering work can be done on the server, sending less JavaScript to the client.
-   **Improved Developer Experience**: Features like layouts, loading UI, and error boundaries are now built-in and co-located with the routes they affect.
-   **Advanced Routing Patterns**: It easily supports complex routing scenarios, like nested layouts and parallel routes, which were difficult to implement in the `pages` router.

### When to use it?

You should use the App Router for **all new Next.js projects**. It is the standard for modern Next.js development. While the `pages` router is still supported for backward compatibility, the App Router offers more features and better performance.

### How it differs from React (Vite)

| Feature           | Next.js (App Router)                                                                                             | React (Vite)                                                                                                   |
| ----------------- | ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Routing**       | **File-system based**. A folder structure inside `/app` defines the URL paths. Built-in and server-centric.        | **Library-based**. Requires a third-party library like `react-router-dom` to handle client-side routing.        |
| **Rendering**     | **Server-first**. Components are React Server Components by default, meaning they render on the server.            | **Client-only**. All components render in the browser by default. SSR needs manual and complex configuration.    |
| **Project Setup** | **Integrated**. `create-next-app` sets up a complete, opinionated framework with routing, and server capabilities. | **Minimalist**. `create-vite` sets up a lightweight, fast build tool and dev server. Routing is not included. |
| **Backend**       | **Built-in**. You can create backend API endpoints directly within the same project.                               | **Separate**. Typically requires a separate backend server (e.g., Express, FastAPI) to be created and managed. |

---

### Exercise

1.  **Create a Page**: Inside this `01-project-setup` folder, create a file named `page.tsx`.
2.  **Add Content**: Add a simple React component to `page.tsx`, for example:
    ```tsx
    export default function ProjectSetupPage() {
      return <h1>Hello from the Project Setup Page!</h1>;
    }
    ```
3.  **Run the Server**: Run `npm run dev` in your terminal.
4.  **View the Page**: Navigate to `http://localhost:3000/01-project-setup` in your browser. You should see your heading. You have just created your first route with the App Router!
