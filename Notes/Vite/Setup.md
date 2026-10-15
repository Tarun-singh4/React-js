# What is Vite?

**Vite** is a frontend build tool that helps us create, run, and build React projects quickly.

### How to Create a React Project

**Step 1: Open the terminal in VS Code**

Press `` Ctrl + ` `` to open the terminal.

**Step 2: Create a React project**

```bash
npm create vite@latest my-react-app -- --template react
```

**Step 3: Enter the project folder**

```bash
cd my-react-app
```

**Step 4: Install dependencies**

```bash
npm install
```

**Step 5: Run the project**

```bash
npm run dev
```

Open the local URL shown in your terminal (usually `http://localhost:5173/`) in your browser.

### Basic Folder Structure

```text
my-react-app/
├── node_modules/
├── public/
├── src/
│   ├── assets/
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── index.html
├── package.json
└── vite.config.js
```

### Important Files

* **`src/App.jsx`** — Your main React component.
* **`src/main.jsx`** — The entry point that renders React into the webpage.
* **`src/App.css`** — Styles for your app.
* **`index.html`** — The HTML page where your app is mounted.
* **`package.json`** — Contains project information, dependencies, and scripts.
* **`node_modules/`** — Stores installed dependencies.

### How Does It Work?

1. Vite starts a development server.
2. The browser loads `index.html`.
3. `main.jsx` starts the React application.
4. React renders the `App` component.
5. Vite supports fast updates while you develop.

**Remember:** `npm run dev` starts the development server. Keep the terminal running while you work.



# Vite + React Folder Structure

* **`node_modules/`** → Contains installed packages and dependencies.
* **`public/`** → Stores static files like images and icons.
* **`src/`** → Contains the main React source code.

  * **`assets/`** → Images, SVGs, and other imported assets.
  * **`App.jsx`** → Main React component that builds the UI.
  * **`App.css`** → CSS styles for the app.
  * **`index.css`** → Global CSS styles.
  * **`main.jsx`** → Entry point that renders `App` into the HTML page.
* **`index.html`** → Main HTML file containing the `root` element.
* **`package.json`** → Project dependencies and npm scripts.
* **`package-lock.json`** → Records the exact dependency versions installed.
* **`vite.config.js`** → Vite configuration.
* **`.gitignore`** → Specifies files Git should ignore.

### Working Flow

`index.html` → `main.jsx` → `App.jsx` → UI in the browser.
