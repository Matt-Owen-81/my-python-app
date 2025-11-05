# My Python App

A simple Python project for testing GitHub-based development and artifact tracking.

## 🧪 Features
- Python 3.x
- Virtual environment (`.venv`)
- Artifact generation and upload
- GitHub-based code editing and syncing

## 🚀 Workflow
1. Edit code in GitHub browser
2. Pull to Ubuntu dev laptop
3. Run scripts locally
4. Push generated artifacts back to GitHub

## 📂 Structure
```
my-python-app/
├── .venv/              # Local virtual environment (ignored)
├── hello.py            # Sample script
├── artifacts/          # Generated outputs
└── README.md           # Project overview
```

## 🛠️ Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## 📤 Artifact Upload
Artifacts are stored in `artifacts/` and committed manually:
```bash
git add artifacts/
git commit -m "Add new artifacts"
git push
```
