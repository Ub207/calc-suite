# calc‑suite

A **multi‑interface calculator** built with Python, FastAPI, Tkinter, a static web page, and an Electron desktop wrapper.

## Features
- **CLI** – `python calculator.py "2 + 3 * (4 - 1)"`
- **Tkinter GUI** – `python calculator_tkinter.py`
- **Web UI** – Open `calculator_web.html` (requires the FastAPI backend).
- **Electron app** – Desktop app that loads the same web UI.
- **FastAPI backend** – Evaluates arithmetic expressions safely using `ast`.
- **Unit tests** – `python -m unittest test_calculator.py`

## Quick start (Windows)
```bat
rem 1. Install Python dependencies
pip install -r requirements.txt

rem 2. Start the API (keep this window open)
uvicorn calculator_api:app --host 127.0.0.1 --port 8000

rem 3. Choose a UI:
rem   • Tkinter GUI
python calculator_tkinter.py

rem   • Web UI (open in browser)
start "" "c:\\calculator\\calaculator\\calculator_web.html"

rem   • Electron app (install once, then start)
cd c:\\calculator\\calaculator\\electron_app
npm install
npm start
```

## Project structure
```
calc-suite/
├─ calculator.py               # core evaluator & CLI
├─ calculator_tkinter.py       # Tkinter wrapper
├─ calculator_api.py           # FastAPI server
├─ calculator_web.html         # static web UI
├─ test_calculator.py          # unit tests
├─ electron_app/               # Electron wrapper
│   ├─ package.json
│   ├─ main.js
│   └─ index.html
└─ requirements.txt            # Python deps
```

## Contributing
Feel free to open issues or pull requests. Adding new UI frameworks, more advanced math functions, or styling improvements are welcome.

## License
MIT – see `LICENSE` file.

---
*Showcase your coding skills, attract collaborators, and even monetize through sponsorships or a paid Pro version.*
