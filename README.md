🔷 Flow Note

Flow Note is a lightweight, fully offline-capable flowchart and diagramming tool built entirely in a single HTML file using React and Tailwind CSS.

It was designed to help users quickly map out plans, decision trees, and process flows (like life plans, business workflows, or cash flow diagrams) without needing to install heavy software, set up a database, or even connect to the internet.

✨ Features

Zero Build Step & Offline Ready: Runs directly in your browser. Just open the HTML file and start diagramming.

Drag-and-Drop Library: Easily pull "Process" blocks (rectangles) and "Decision" blocks (diamonds) from the sidebar right onto your canvas.

Smart Arrow Connections: Nodes are connected using SVG paths that automatically calculate intersections, ensuring arrows point cleanly to the edges of your shapes without overlapping text.

Lightning-Fast Hotkeys: Select a block and press Shift + Right Arrow to instantly spawn a new, connected block to its right and begin typing.

Multi-Element Resizing: Select multiple blocks (by shift-clicking or dragging a selection box) and drag the bounding box handle to scale a whole "pack" of elements proportionally together.

Local Save & Load: Export your flowchart as a local .json file and load it back up at any time. Your data never leaves your machine.

🚀 How to Run

Clone or download this repository to your local machine.

Ensure all the required script files (React, ReactDOM, Babel, Tailwind) are in the exact same folder as the HTML file.

Double-click flow_note_app.html to open it in any modern web browser (Chrome, Edge, Safari, Firefox).

Note: No local web server (like localhost) is required. It works flawlessly over the file:/// protocol.

📂 Files Required in this Repository

To ensure this app works offline for anyone who downloads it, you must upload the following 5 files to your GitHub repository:

flow_note_app.html (The main application file)

react.production.min.js (React core library)

react-dom.production.min.js (React DOM rendering library)

babel.min.js (Babel compiler, specifically v7.23.6, used to translate JSX in the browser)

tailwindcss.js (Tailwind CSS engine)

(Note: Ensure the local filenames match exactly what is listed above, as the HTML file links to them directly!)

🛠️ Built With

React 18

Tailwind CSS

Babel (Standalone)