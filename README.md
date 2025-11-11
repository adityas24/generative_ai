# Generative AI

This repository contains experiments and code related to generative AI and other ML projects. It is structured to keep Python scripts and individual project work separated.

## Structure
- `python/` — standalone Python scripts (entry point: `python/main.py`).
- `ai-projects/ann-project/` — ANN project with a dataset (`Churn_Modelling.csv`), a notebook (`experiments.ipynb`), and its own `requirements.txt`.
- `ai-projects/other-project/` — placeholder for additional projects.

## Getting Started

### Prerequisites
- Python 3.9+ installed and available in your PATH
- Git installed and configured with your GitHub account

### Setup (Windows)
1. Create a virtual environment at the repo root (recommended):
   ```powershell
   python -m venv .venv
   .venv\Scripts\activate
   ```
2. Install dependencies for specific projects as needed, e.g. ANN project:
   ```powershell
   pip install -r ai-projects\ann-project\requirements.txt
   ```

### Running
- Run the main script:
  ```powershell
  python python\main.py
  ```
- Open and run the notebook:
  - Use your preferred editor to open `ai-projects/ann-project/experiments.ipynb` and run the cells.

## Development Notes
- Virtual environments (`.venv`, `venv`, etc.), notebook checkpoints, IDE settings, and OS files are ignored via `.gitignore`.
- If you plan to add large datasets or model artifacts (>100MB), consider using Git LFS:
  ```powershell
  git lfs install
  git lfs track "*.pt" "*.h5" "*.ckpt"
  git add .gitattributes
  git commit -m "Track large model files with Git LFS"
  ```

## GitHub Setup
1. Initialize the repository (if not already):
   ```powershell
   git init
   git checkout -b main
   git add .
   git commit -m "Initialize repository with .gitignore and README"
   ```
2. Create a new GitHub repo (via GitHub UI) and add it as a remote:
   ```powershell
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

## License
This project currently has no explicit license. If you plan to open-source, add a license file (e.g., MIT) at the repo root.