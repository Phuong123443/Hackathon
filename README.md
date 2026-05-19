# MEOWIE-CRM

## Setup

1. Create and activate the virtual environment:
   - PowerShell: `python -m venv .venv ; .\.venv\Scripts\Activate.ps1`
   - CMD: `python -m venv .venv && .\.venv\Scripts\activate.bat`

2. Install dependencies:
   - `.\.venv\Scripts\python.exe -m pip install -r requirements.txt`

3. Copy `.env.example` to `.env` and update the values.

4. Run the app:
   - `.\.venv\Scripts\python.exe app.py`

## Notes

- The app serves static pages from the workspace root.
- `login.html` now uses the role returned by the backend instead of overriding it from the form selection.
- If `OPENAI_API_KEY` is not configured or remains a placeholder, the AI endpoint will return a clear informational reply instead of failing.
