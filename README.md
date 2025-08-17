
# Quiver → Fletchy Converter (Standalone)

Convert your **Quiver** library (`.qvlibrary` or zipped) into a **Fletchy** bundle (`.fletchy`) — directly in the browser. No servers, no accounts, no uploads.

> This project helps people looking for a **Quiver app alternative** migrate their notebooks to **Fletchy**, a modern, open‑source notebook for developers and researchers.

- **Live demo:** Open `index.html` (works from file system)
- **Privacy:** 100% client‑side using JSZip
- **Output:** Single `.fletchy` file importable by the Fletchy web or desktop app

## Why a Quiver App Alternative?

Quiver hasn't been actively maintained for years. Fletchy offers a clean, actively developed experience with Markdown, code cells, LaTeX, and Mermaid diagrams — keeping the multi‑format spirit of Quiver while adding a modern UI and export/import features.

**Keywords:** Quiver app alternative, Quiver replacement, migrate from Quiver, Quiver to Fletchy, Quiver importer, developer notebook, Markdown and code notes.

## Features

- Drag‑and‑drop **`.qvlibrary`** or **`.zip`** export
- Parses notebooks and notes in‑browser (JSZip)
- Preserves Markdown, code (with language where available), LaTeX, and basic structure
- Exports a **`.fletchy`** bundle for quick import
- Progress UI with stages: Upload → Converting → Download
- Offline / private by default

## Usage

1. Export your Quiver library (`YourLibrary.qvlibrary`) or zip the folder.
2. Open **`index.html`** in a modern browser (no server required).
3. Drop the `.qvlibrary` or `.zip` into the page.
4. Download the generated **`.fletchy`** file.
5. Import it in the **Fletchy** app: Web or Desktop.

## How It Works

The converter scans `*.qvnotebook/` directories in your archive, reads `meta.json` and `content.json`, then maps Quiver cell types to Fletchy's generic schema. Everything happens **locally** in your browser via **JSZip**; your data never leaves your machine.

## FAQ

**Is this an official Quiver tool?**  
No. It's a community migration path to Fletchy.

**What about images/attachments?**  
This minimal converter focuses on Markdown, code, LaTeX, and structure. You can extend it to traverse binary attachments and embed or link them into the exported schema.

**Which browsers are supported?**  
Any modern Chromium/Firefox/Safari.

## Roadmap

- Attachment extraction (images/resources)
- Richer metadata mapping (tags, favorites)
- CLI variant for batch jobs

## Contributing

PRs welcome! Open an issue to discuss features or edge cases found in real‑world Quiver libraries.

## License

MIT © Yxanu

---

