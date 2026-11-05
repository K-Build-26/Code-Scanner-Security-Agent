# Code Scanner Security Agent

The goal is to gradually build a security pipeline using automated Github Actions that helps identify security issues in code before changes are merged into the main branch.

As security tools and GitHub Actions workflows are added, this README will be updated with additional setup instructions and documentation.

## Prerequisites

- Git installed
- Python 3 installed
- Google Gemini API key
- GitHub account

## Getting Started

### 1. Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/K-Build-26/Code-Scanner-Security-Agent.git

cd Code-Scanner-Security-Agent
```

### 2. Create a Virtual Environment

A virtual environment keeps this project's Python dependencies separate from other Python projects on your computer.

Run:

```bash
python3 -m venv .venv
```

### 3. Activate the Virtual Environment

```bash
source .venv/bin/activate
```

Once activated, you should see `(.venv)` at the beginning of your terminal prompt.

### 4. Install Dependencies

Install the project dependencies:

```bash
pip install -r requirements.txt
```

### 5. Configure Your Gemini API Key

You can obtain one through Google AI Studio:

https://aistudio.google.com/apikey

Create a `.env` file in the root directory of the project:

```text
GEMINI_API_KEY=your_api_key_here
```

Replace `your_api_key_here` with your actual Gemini API key.

**Important:** Never commit your API key to GitHub. Make sure `.env` is included in your `.gitignore` file.

If `.gitignore` does not exist, create it and add:

```text
.env
venv/
.venv
__pycache__/
```

### 6. Run the Python Application

```bash
python3 main.py
```


