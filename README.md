
# PDF Splitter

> Split tall PDF pages into slices, preview them, and optionally merge them.

I built this small tool because I kept running into PDFs that were way too tall for a single page to render properly in Adobe. I imagine it being useful for posters, schematics, long charts — stuff that just doesn’t “fit.” PDF Splitter cuts those into clean, printable slices, lets you preview them, and even merge them back if that’s what you want. All without turning them into blurry images.

## Non-rasterizing!

I didn’t want to rasterize anything (that’s for images). Instead, this tool works straight on the PDF’s vector data using pdfrw and reportlab, so everything stays sharp. For previews, I lean on pymupdf (fitz) — it’s fast and does what it needs to do without fuss.

## Flet

I like writing things all in Python. With Flet, I can build a GUI without touching JavaScript or SDKs. The same code can run locally, as a web app, or be packaged for distribution on Linux (my preference!) as well as Mac, Windows, and mobile. Do note that I haven't tested this app on mobile devices yet, so you're likely to encounter bugs.

## Updates/ideas/support
If you want to contribute, please do so! /;

# Requirements
- Python 3.10+
- macOS, Windows, or Linux

# Install
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
