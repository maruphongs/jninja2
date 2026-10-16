# Jinja2 & FastAPI Demo (jinjateach)

A lightweight web application demonstrating server-side rendering using **FastAPI** and **Jinja2** templates, styled with custom CSS and modular component templates.

## Features

- **FastAPI Backend**: Clean routing and form processing.
- **Jinja2 Templates**: Modular layout structure (`base.html`, `index.html`, and component partials).
- **CRUD Operations**: View server items, add new items via form submission, and delete items asynchronously via API.
- **Static Assets**: Organized static directory for custom CSS styles and JavaScript scripts.

## Tech Stack

- **Python 3.13+**
- **FastAPI**
- **Jinja2**
- **Uvicorn**

## Getting Started

### 1. Installation

Using `uv` (recommended):
```bash
uv sync
```

Or using standard `pip`:
```bash
python -m venv .venv
# On Windows:
.venv\Scripts\activate
# On Linux/macOS:
source .venv/bin/activate

pip install fastapi[standard] jinja2
```

### 2. Running the Application

Run the server with FastAPI CLI or Uvicorn:

```bash
fastapi dev main.py
```
Or:
```bash
uvicorn main:app --reload
```

Open your browser and navigate to `http://127.0.0.1:8000`.

## Project Structure

```text
├── main.py              # Application entry point & route handlers
├── pyproject.toml       # Project metadata and dependencies
├── templates/           # Jinja2 HTML templates
│   ├── base.html        # Base layout template
│   ├── index.html       # Dashboard page
│   └── components/      # Reusable template components
└── static/              # Static files
    ├── styles/          # CSS stylesheets
    └── scripts/         # Client-side JavaScript
```
