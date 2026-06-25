# Flow Note

Flow Note is a lightweight, fully offline-capable flowchart and diagramming tool built entirely in a single HTML file using React and Tailwind CSS.

It was designed to help users quickly map out plans, decision trees, and process flows without needing to install heavy software, set up a database, or even connect to the internet.

## Features

- **Zero Build Step & Offline Ready**: Runs directly in your browser. Just open the HTML file and start diagramming.
- **Drag-and-Drop Library**: Easily pull "Process" blocks (rectangles) and "Decision" blocks (diamonds) from the sidebar right onto your canvas.
- **Smart Arrow Connections**: Nodes are connected using SVG paths that automatically calculate intersections, ensuring arrows point cleanly to the edges of your shapes.
- **Lightning-Fast Hotkeys**: Select a block and press Shift + Right Arrow to instantly spawn a new, connected block.
- **Multi-Element Resizing**: Select multiple blocks and scale them proportionally together.
- **Local Save & Load**: Export your flowchart as a local .json file. Your data never leaves your computer.

## V2 Features

### 1. EPUB Extraction and Parsing
- **Drag-and-Drop Support**: Implemented native `.epub` file support, allowing users to import digital books via drag-and-drop.
- **In-Browser Processing**: Leverages the `JSZip` library to decompress and read EPUB structures directly within the browser environment.
- **Smart Order Resolution**: Includes parsing logic for `container.xml` and manifest files to ensure chapters are extracted in their correct reading sequence.
- **Japanese Text Optimization**: Features a dedicated cleaning engine to strip HTML and `<rt>`/`<rp>` (ruby) tags, preventing character duplication in Japanese light novels.

### 2. Streamlined Minimalist UI
- **Texture Reduction**: Removed "heavy" glassmorphism effects, such as backdrop blurs and translucent layers, in favor of a cleaner aesthetic.
- **Native Experience**: Redesigned panels using a flat white palette with subtle shadows against a light gray background, providing a more responsive and lightweight "native app" feel.

### 3. Integrated ZIP Export & "Drag-to-Folder"
- **Multi-File Bundling**: Automatically aggregates all processed `.txt` files into a single `.zip` archive using `JSZip` to avoid repetitive download prompts.
- **OS-Level Drag-and-Drop**: Implemented the HTML5 `DownloadURL` Drag-out API, enabling users to drag the exported ZIP directly from the browser into their local operating system folders.
- **One-Click Batch Save**: Replaced individual file downloads with a unified "Save All" button that triggers the ZIP archive download.

## Installation

1. Clone or download this repository to your local machine.
2. Ensure all the required script files (React, ReactDOM, Babel, Tailwind) are in the exact same folder as the HTML file.
3. Double-click `flow_note_app.html` to open it in any modern web browser.

Note: No local web server is required. It works flawlessly over the `file:///` protocol.

## Files Required in this Repository

To ensure this app works offline, you must include the following 5 files:
- `flow_note_app.html`
- `react.production.min.js`
- `react-dom.production.min.js`
- `babel.min.js` (v7.23.6)
- `tailwindcss.js`

## Built With
- React
- Tailwind CSS
- JSZip
- Babel
