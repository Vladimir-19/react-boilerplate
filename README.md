# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React App Setup with Vite

A beginner-friendly guide for creating and running a React application using Vite, the modern build tool that replaces Create React App (CRA).

This guide walks you through setting up your first React app using Vite, a fast, modern build tool designed for an optimized developer experience.

## Prerequisites

You’ll need Node.js and npm (Node Package Manager) installed.

Check if Node is Installed: `node -v`

If installed, this returns a version like v23.1.0.

## Required Versions

Vite requires:

- Node v18+ or v20+

### Update npm

Even if you just installed Node, it’s a good idea to update npm:
`# macOS / Linux`
`sudo npm install -g npm@latest`

## Setting Up Your React App with Vite

Vite helps you quickly generate a boilerplate React app with an optimized configuration.

### Benefits of Using Vite

1. Consistent, familiar project structure

2. Optimized builds out-of-the-box

3. Lightning-fast dev server with hot module replacement (HMR)

4. Modern tooling with minimal setup

# Create Your Project

Open your terminal and run one of the following:

### Using npm

`npm create vite@latest`

###Follow the interactive prompts:

1. Enter your project name (e.g. my-react-app)
2. Select React as your framework
3. Choose your variant: JavaScript or TypeScript

### Or skip the prompts by running:

`# npm`
`npm create vite@latest my-react-app -- --template react`

`# yarn`
`yarn create vite my-react-app --template react`

`# pnpm`
`pnpm create vite my-react-app --template react`

Once complete, you’ll:
`cd my-react-app`
`npm install`
`npm run dev`

## Create a proper .gitignore

1. Ensure that .gitignore includes following:
   
  ## Recommended .gitignore

```gitignore
# dependencies
node_modules/

# build output
dist/
.vite/

# environment variables
.env
.env.local
.env.*.local

# logs
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# IDE files
.vscode/
.idea/
.DS_Store


3. Remove files that should have been ignored
   `git rm -r --cached .`
   `git add .`
   `git commit -m "Clean up repo and add .gitignore"`
   `git push -f origin main`

After this, your Source Control in VS Code should show only your project files — no 10k other files.

## Project Structure

<pre> ```plaintext 📁 my-react-app ├── 📁 public │ └── vite.svg ├── 📁 src │ ├── App.css │ ├── App.jsx │ ├── 📁 assets │ │ └── react.svg │ ├── index.css │ └── main.jsx ├── .gitignore ├── eslint.config.js ├── index.html ├── package-lock.json ├── package.json ├── README.md └── vite.config.js ``` </pre>

## Key Directories

/node_modules – Contains all dependencies (auto-generated; don’t edit).
/public – Holds static assets like icons and logos.
/src – Main source folder for your React code: - App.jsx – main app component - App.css – styles for the app - main.jsx – entry point (equivalent to index.jsx) - assets/ – for images and static assets

💡 You can rename main.jsx → index.jsx if preferred, but update the import in index.html.

## 🗂️ Key Files

| File               | Description                                                   |
| ------------------ | ------------------------------------------------------------- |
| `index.html`       | Entry point HTML file. Vite injects compiled JavaScript here. |
| `package.json`     | Lists dependencies, metadata, and npm scripts.                |
| `vite.config.js`   | Configures Vite (React plugin, aliases, proxy, etc.).         |
| `eslint.config.js` | Linting rules for consistent code style.                      |
| `.gitignore`       | Specifies files/folders Git should ignore.                    |

## 🚀 Important npm Scripts

| Command           | Description                          |
| ----------------- | ------------------------------------ |
| `npm run dev`     | Starts the development server.       |
| `npm run build`   | Builds a production-ready version.   |
| `npm run preview` | Serves the production build locally. |

# Making Your First Edit

Open src/App.jsx and add something new!

### Happy Coding! 💻
