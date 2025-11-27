# Glenair Extractor - Agent Development Guide

## Environment Setup
```bash
# Activate virtual environment
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Development Commands
```bash
# Run the application
streamlit run app.py

# Install dependencies
pip install -r requirements.txt

# No test framework currently configured
# Add pytest when implementing tests: pip install pytest
```

## Code Style Guidelines

### Imports
- Group imports: standard library, third-party, local modules
- Use `import streamlit as st` convention
- Third-party: `import pdfplumber`, `import fitz`, `import pandas as pd`

### Formatting
- Follow PEP 8
- 100 character line limit
- Use f-strings for string formatting

### Types
- Add type hints for function parameters and returns
- Use `Optional[T]` for nullable values
- Import from `typing` module

### Naming Conventions
- Functions: snake_case
- Variables: snake_case  
- Constants: UPPER_CASE
- Classes: PascalCase

### Error Handling
- Use try/except blocks for file operations
- Log errors using `utils.logger`
- Provide user-friendly error messages in Streamlit

## Project Structure
- `app.py` - Main Streamlit application
- `pages/` - Streamlit multi-page components
- `utils/` - Shared utilities (logger, helpers)
- `config/settings.yaml` - Configuration file
- `data/` - Input/output data directory
