# Run Guide

This file explains how to run the project without changing the source code.

## Project Path

Open PowerShell in:

```powershell
D:\RAJUAN-PERSONAL\VSCODE\wasabigamimg\ai_wasabigaming
```

## First-Time Setup

Create a virtual environment:

```powershell
python -m venv .venv
```

Activate the virtual environment:

```powershell
.\.venv\Scripts\activate
```

Upgrade `pip`:

```powershell
python -m pip install --upgrade pip
```

Install dependencies:

```powershell
python -m pip install -r requirements.txt
```

## Run the App

Start the FastAPI server:

```powershell
python -m uvicorn main:app --host 127.0.0.1 --port 8000
```

Open these URLs in your browser:

- `http://127.0.0.1:8000`
- `http://127.0.0.1:8000/docs`
- `http://127.0.0.1:8000/openapi.json`

## Next Time You Run It

If the environment is already set up, use:

```powershell
.\.venv\Scripts\activate
python -m uvicorn main:app --host 127.0.0.1 --port 8000
```

## Stop the App

Press `Ctrl+C` in the terminal.

## If PowerShell Blocks Activation

Run:

```powershell
Set-ExecutionPolicy -Scope Process Bypass
```

Then activate again:

```powershell
.\.venv\Scripts\activate
```

## Note

The app may show a warning related to `langchain` on Python 3.14, but it can still start successfully.
