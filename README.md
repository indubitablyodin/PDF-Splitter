
# PDF Splitter

Split tall PDF pages into slices, preview them, and optionally merge them.

## Requirements
- Python 3.10+
- macOS, Windows, or Linux

## Install
```bash
python -m venv .venv
source .venv/bin/activate   # on Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
````

## Run the GUI

```bash
python src/flet_app.py
```

## Run the CLI

```bash
python src/split_pdf_cli.py path/to/input.pdf -o output -H 792 -m -c
```
