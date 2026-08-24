# File Browser
    A file browser to view files on server for debug
---
- Vivid visual effects
- Real-time interaction and operation like download
- Automatic directory scaning(based on Github Action)

due to my limited capacity, I used AI to help me. 

---
*The following content is AI-generated

## Features

- 📂 **Directory tree** – navigate folders with click/enter
- 🔍 **Live search** – filter current folder contents
- 👁️ **Preview panel** – file/folder details on selection
- ⬇️ **Download & open** – files can be downloaded or opened in a new tab
- ⌨️ **Keyboard shortcuts** – Alt+←/→/↑ (back/forward/up), F2 (rename), Delete, Ctrl+F (search)
- 🎨 **Dark-themed UI** – smooth animations, responsive
- 🤖 **Auto-deploy** – GitHub Actions builds and publishes to Pages

## Tech Stack

- Frontend: vanilla HTML/CSS/JS + TailwindCSS + Phosphor Icons
- Build: Node.js script (`build.js`) – scans directory, generates JSON tree, copies assets
- Deployment: GitHub Actions + `peaceiris/actions-gh-pages`

## Quick Start

```bash
git clone https://github.com/Chtrrrrrrr/FileBrowser.git
cd FileBrowser
npm install
npm run build          # scans parent directory (..) and outputs to dist/
npx serve dist         # preview locally at http://localhost:3000
```

## Customization

Edit `CONFIG` in `build.js`:

- `sourceDir` – directory to scan (default: `..`)
- `ignore` – list of names to exclude
- `maxDepth` – max recursion depth
- `showHidden` – show dotfiles or not

## Deployment

On every push to `main`, GitHub Actions builds and deploys the `dist` folder to the `gh-pages` branch. Set your Pages source to that branch.

## Notes

- The tree is **static** – built at deploy time, not live.
- Built with AI assistance – contributions welcome via issues/PRs.

---

*For personal use and learning – no explicit license.*
