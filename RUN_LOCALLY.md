# 💻 Running The Red Book Locally

Follow these quick steps to run the Starlight documentation site locally on your machine.

## Prerequisites

Make sure you have **Node.js** (v18.x or higher) installed. You can check your version by running:
```bash
node -v
```

## Setup & Execution

### 1. Install Dependencies
Navigate to the project root directory and run the following command to install the required packages:
```bash
npm install
```

### 2. Start the Local Development Server
Launch the development server:
```bash
npm run dev
```

The terminal will display the local development address, usually:
👉 **[http://localhost:4321/redbook/](http://localhost:4321/redbook/)**

Open this URL in your web browser. The dev server features hot reloading, meaning any changes you make to the markdown docs will reflect instantly.

---

## Useful Scripts

| Command | Description |
| :--- | :--- |
| `npm run dev` | Starts the local dev server at `http://localhost:4321/redbook/` |
| `npm run build` | Compiles the production build (outputs to the `./dist` folder) |
| `npm run preview` | Runs a local web server previewing the built production files |
| `npm run astro ...` | Runs raw Astro CLI commands (e.g. `npm run astro info`) |
