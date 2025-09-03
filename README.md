# visionflow2.0
AI Software Design Diagram Generator

An interactive web-based tool that converts a problem statement into structured software design diagrams using Mermaid.js and Google’s Gemini API.

It provides a step-by-step workflow to generate DFDs (Data Flow Diagrams), Class Diagrams, and Sequence Diagrams, all in the browser. Users can copy the generated Mermaid code or save diagrams as PNGs.

🚀 Features

Problem Statement Input → Describe your system (e.g., Library Management System).

DFD Workflow:

Generate Level 0 (Context Diagram)

Expand into Level 1 (Processes & Data Stores)

Expand individual processes into Level 2

UML Derivation:

Generate Class Diagram (from Level 1)

Generate Sequence Diagram(s) (from Level 2)

Live Rendering using Mermaid.js with dark theme support.

Export Options: Copy Mermaid code or save diagrams as PNG.

Smooth UI with TailwindCSS, dark mode, and animated buttons.

🛠️ Tech Stack

Frontend:

TailwindCSS
 – Styling

Mermaid.js
 – Diagram rendering

Google Fonts: Inter

Backend (API):

Gemini API
 (Gemini 2.5 Flash Preview)

Utilities:

Vanilla JavaScript for state management & UI logic

Exporting diagrams as PNG via <canvas>

📂 Project Structure
📦 ai-software-design-diagram-generator
 ┣ 📜 index.html        # Main application (all logic in one file)
 ┣ 📜 README.md         # Documentation (this file)
 ┗ 📂 assets/           # (optional) place for screenshots, icons, etc.

⚙️ Setup & Usage

Clone this repo:

git clone https://github.com/your-username/ai-software-design-diagram-generator.git
cd ai-software-design-diagram-generator


Open the project:
Just open index.html in any modern browser (no build step required).

Provide Problem Statement:
Example:

A library management system where users can borrow and return books.


Generate Diagrams Sequentially:

Click Generate DFD Level 0

Expand to DFD Level 1

Optionally expand processes into Level 2

Derive Class Diagram and Sequence Diagram(s)

Export & Save:

Copy Mermaid code (for reuse in docs/wiki).

Save diagrams as PNG with one click.

🔑 API Key Setup

This project uses Gemini API.

Replace the placeholder key inside index.html:

const apiKey = "YOUR_API_KEY_HERE";


Get your API key from Google AI Studio
.

⚠️ Important: Do not commit your private API key to a public repository. Use environment variables or prompt users to paste their own.

📸 Demo Screenshot

(Optional: Add a screenshot of your app UI here, e.g., in /assets/screenshot.png)

📌 Roadmap

 Add Use Case Diagram support

 Add ER Diagram support

 Integrate export to PDF option

 Deploy live demo with GitHub Pages

🤝 Contributing

Contributions are welcome! To contribute:

Fork this repo

Create a feature branch (git checkout -b feature/awesome-feature)

Commit changes (git commit -m 'Add awesome feature')

Push (git push origin feature/awesome-feature)

Create a Pull Request

📄 License

MIT License – free to use, modify, and distribute.
