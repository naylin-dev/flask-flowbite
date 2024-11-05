# Flask Flowbite Demo

This is a demo Flask application that integrates Flowbite for UI components. The application is designed to demonstrate how to set up a basic Flask app with Flowbite styling.

![Flask app with Flowbite](banner.png)

## Prerequisites

-   [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) (for [Flowbite](https://flowbite.com/) and [Tailwind CSS](https://tailwindcss.com/))
-   [uv](https://docs.astral.sh/uv/) An extremely fast Python package and project manager, written in Rust. (Recommended)
-   [Python](https://www.python.org/) 3.12 or higher (Note: If using uv, it will automatically install Python 3.12 if not present on your system)

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/naylin-dev/flask-flowbite.git
cd flask-flowbite
```

### 2. Creating a Virtual Environment

Using uv

```bash
uv venv --python 3.12
# On macOS/Linux
source .venv/bin/activate
# On Windows
.venv\Scripts\activate
```

Using venv

```bash
python3 -m venv venv
# On macOS/Linux
source venv/bin/activate
# On Windows
venv\Scripts\activate
```

### 3. Install Dependencies

Using uv

```bash
uv sync
```

Using pip

```bash
pip install -r requirements.txt
```

### 4. Install Node.js Dependencies

```bash
cd static
npm install
```

Build CSS with Tailwind

```bash
npm run build:css
```

### 5. Run the Application

```bash
# Make sure you're in the project root directory
python app.py
```

The application will be available at http://127.0.0.1:5000.

## Project Structure

```bash
flask-flowbite/
├── app.py                  # Flask application entry point
├── pyproject.toml          # Python project configuration
├── requirements.txt        # Python dependencies
├── static/                 # Static files directory
│   ├── dist/               # Compiled assets
│   ├── src/                # Source files
│   ├── package.json        # Node.js dependencies
│   └── tailwind.config.js  # Tailwind CSS configuration
└── templates/              # HTML templates
```

## Dependencies

-   [Flask](https://flask.palletsprojects.com/) - 3.0.3
-   [Flowbite](https://flowbite.com/) - 2.5.1
-   [Tailwind CSS](https://tailwindcss.com/) - 3.4.8
