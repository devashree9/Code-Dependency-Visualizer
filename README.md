# Code Dependency Visualizer 🚀

An interactive full-stack developer tool designed to perform AST-based static analysis on GitHub repositories and map module relationships into dynamic, interactive dependency graphs.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-009688?style=flat&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?style=flat&logo=react&logoColor=black)
![React Flow](https://img.shields.io/badge/React_Flow-Visualization-FF007A?style=flat)

---

## 📌 Features

- **Automated AST Parsing:** Uses Python's native Abstract Syntax Tree parsing to extract module imports, class structures, and function calls.
- **Graph Topology Engine:** Builds directed acyclic dependency graphs using `NetworkX` to compute layout nodes and hierarchy levels.
- **Interactive UI:** Renders custom nodes, draggable structures, and zoomable maps using `React Flow`.
- **Git Integration:** Integrates `GitPython` for dynamic repository cloning, temporary workspace handling, and module isolation.
- **RESTful Architecture:** Lightweight, asynchronous endpoint execution via `FastAPI`.

---

## 🛠️ Tech Stack

- **Frontend:** React.js, React Flow, Axios
- **Backend:** Python 3.10+, FastAPI, Uvicorn
- **Static Analysis & Graph Theory:** `ast`, `NetworkX`, `GitPython`

---

## 📂 Project Structure

```text
code-dependency-visualizer/
├── backend/
│   ├── main.py              # FastAPI server entry point & CORS configuration
│   ├── clone_repo.py        # Git repository extraction and workspace management
│   ├── ast_parser.py        # AST parsing engine & dependency mapping
│   ├── graph_builder.py     # NetworkX directed graph computation
│   └── requirements.txt     # Python backend dependencies
└── frontend/
    ├── src/
    │   ├── components/      # React Flow graph components & controls
    │   ├── services/        # API calls to FastAPI backend
    │   └── App.js           # Main UI container
    └── package.json         # Node.js dependencies & scripts
