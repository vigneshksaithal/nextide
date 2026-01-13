# Next IDE

A modern landing page for **Next IDE** - The AI Code Reviewer. Next IDE is a VS Code extension that provides AI-assisted code reviews, visual diffs, and collaboration tools to accelerate your development workflow.

## Features

- **Code Diagrams** - Visualize your entire code architecture at a glance to understand dependencies and impact
- **Flowchart Diffs** - Intuitively grasp logic changes with visual diffs that show flow instead of just text
- **Faster Reviews** - Leverage AI-powered suggestions and a streamlined UI to complete reviews in record time

## Tech Stack

- [SvelteKit](https://kit.svelte.dev/) - Full-stack framework
- [Svelte 5](https://svelte.dev/) - Modern reactive framework
- [TypeScript](https://www.typescriptlang.org/) - Type safety
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Vite](https://vitejs.dev/) - Build tool and dev server

## Getting Started

### Prerequisites

- Node.js 18+ (or Bun)
- npm, pnpm, yarn, or bun

### Installation

```sh
# Install dependencies
npm install

# or with bun
bun install
```

### Development

Start the development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

The app will be available at `http://localhost:5173`

### Building

Create a production build:

```sh
npm run build
```

Preview the production build:

```sh
npm run preview
```

### Running Production Build

After building, you can run the production server:

```sh
npm start
```

This uses the Node.js adapter and serves the built application.

## Project Structure

```
src/
├── app.html          # HTML template
├── app.css           # Global styles
├── routes/           # SvelteKit routes
│   ├── +layout.svelte
│   └── +page.svelte  # Landing page
└── lib/
    ├── components/   # Reusable components
    │   └── Landing/ # Landing page components
    └── styles/       # Component styles
```

## Links

- [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=Next-IDE.next-ide)
- [Discord Community](https://discord.gg/xxRAHzRQcY)

## License

Private project
