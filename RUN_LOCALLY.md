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

---

## ✍️ Tips for Writing & Editing Docs Easily

If you are transitioning from GitBook, writing raw Markdown might feel less visual. Here are some tools and setups to make writing documentation easy and intuitive:

### 1. Visual Markdown Editors (WYSIWYG)
If you prefer a document-like interface over raw text files:
*   **[Obsidian](https://obsidian.md/) (Highly Recommended)**: Open the `src/content/docs/` folder directly as an Obsidian Vault. It renders headers, bold text, and lists inline as you type, and supports drag-and-drop pasting for images.
*   **[MarkText](https://www.marktext.cc/) (Free)**: A clean, open-source editor that hides Markdown syntax symbols immediately as you type.

### 2. VS Code / IDE Extensions
If you write directly in your code editor, install these helper extensions:
*   **[Front Matter CMS](https://marketplace.visualstudio.com/items?itemName=Eliostruyf.vscode-front-matter)**: Adds a visual dashboard inside VS Code to create pages, choose templates, select images, and manage page frontmatter (titles/descriptions).
*   **[Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)**: Shows a beautiful side-by-side preview of your layout.
*   **[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)**: Provides shortcuts (`Ctrl+B`, `Ctrl+I`) and formats lists automatically.

### 3. Adding Images & Live Preview
*   **Live Preview**: Keep your local server running (`npm run dev`) side-by-side with your editor. Changes saved to files update instantly in the browser.
*   **Inserting Images**: Put any images under `src/content/docs/images/` and reference them using relative paths:
    ```markdown
    ![Alt Text](../../images/image-name.png)
    ```

