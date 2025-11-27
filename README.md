# Glenair Extractor

A Streamlit app for extracting tables, diagrams, and part numbers from Glenair PDF catalogs.

## Features
- PDF browsing and preview
- Table extraction and validation
- Diagram extraction
- Part numbering and mapping
- Export to JSON

## Setup
1. Create a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   pip install -r requirements.txt
   ```
2. Run the app:
   ```bash
   streamlit run app.py
   ```

## Project Structure
- `app.py`: Main Streamlit app
- `pages/`: Multi-page Streamlit components
- `utils/`: Shared utilities
- `config/settings.yaml`: Configuration
- `input/`, `output/`, `cache/`: Data directories

## Requirements
See `requirements.txt` for dependencies.
