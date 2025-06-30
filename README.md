# Python Jupyter Notebook Project for Thesis

This repository accompanies the thesis and provides code, experiments, and documentation. It uses a virtual environment (venv) for dependency management.

## Setup on a Local Environment

1. Create a Python virtual environment using the command line interface

   for `python`:
   ```bash
   python -m venv .venv
   ```
   or `python3`:
   ```bash
   python3 -m venv .venv
   ```
   , then activate it on Linux/macOS with
   ```bash
   source .venv/bin/activate
   ```
   or on Windows (PowerShell) with
   ```bash
   .\.venv\Scripts\Activate.ps1
   ```
   . In case of access issues in PowerShell, run
   ```bash
   Set-ExecutionPolicy Unrestricted -Scope Process
   ```

   then retry activating the environment.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start Jupyter:

   from the command line 
   ```bash
   jupyter notebook
   ```
   which opens a browser at the address of your local Jupyter server. From there, open the file under `notebook/papiamento-keyword-spotting.ipynb`. Alternatively, you can open this file from your preferred code editor with Jupyter support (e.g., VS Code).

## Project Structure
- Notebooks and scripts for experiments
- requirements.txt for dependencies
- .gitignore to exclude unnecessary files

## Usage
- All code and results are provided for reproducibility.
- See individual notebooks for details.
