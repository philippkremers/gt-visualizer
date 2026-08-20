# Game Theory Visualizer

A tool for demonstrating game-theoretical concepts through interactive payoff matrices. I used this tool in my own classes on social and political philosophy at Georgetown University. I hope it can also be useful to other instructors and students.

You can see a [live demonstration](https://www.philippkremers.com/game-theory-visualizer) here.

## Technical Details

This tool is a single-page application (SPA) designed for client-side interaction only. This approach allows for easy deployment and minimal server requirements: the app can run entirely as static files on any web server.

It is built with Vue 3 and Vite and uses Vue Router with hash-based routing to ensure compatibility across different hosting environments.

## Installation

Clone repository and install dependencies:

```sh
git clone https://github.com/philippkremers/gt-visualizer.git
cd game-theory-visualizer
npm install
```

## Compile and Hot-Reload for Development

```sh
npm run dev
```

Afterwards, you can open your browser at the URL displayed in the terminal (usually http://localhost:5173) to see the app live during development.

## Compile for Deployment

If you do not plan to host this project from the domain root, but from a subdirectory (e.g., `/game-theory-visualizer/`), you must set the correct base path in `vite.config.js`.

To generate static files for deployment:

```sh
npm run build
```

The compiled files will be placed in the `dist/` folder. Because this is a pure client-side SPA, you can deploy them on any static web server.

