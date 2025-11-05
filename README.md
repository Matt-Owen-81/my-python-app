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

## 🛡️ `.gitignore`
Create this file in the same directory:
```gitignore
# Ignore virtual environment
.venv/

# Ignore Python cache
__pycache__/
*.py[cod]

# Ignore artifacts if needed
artifacts/*.log
artifacts/*.tmp

# Ignore OS files
.DS_Store
Thumbs.db
```

## 🛠️ Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
```

## 📤 Artifact Upload
Artifacts are stored in `artifacts/` and committed manually:
```bash
git add artifacts/
git commit -m "Add new artifacts"
git push
```

## 🌿 Branching Strategy

### 🔀 Branch Types
- **`main`** – Stable branch with production-ready code and verified artifacts
- **`dev`** – Active development branch for new features and testing
- **`feature/*`** – Optional branches for isolated feature work (e.g., `feature/logging`, `feature/qr-generator`)

### 🧪 Workflow
1. Create or switch to a dev branch:
   ```bash
   git checkout -b dev
   ```
2. Make changes, commit, and push:
   ```bash
   git add .
   git commit -m "Add new feature"
   git push -u origin dev
   ```
3. Open a pull request on GitHub to merge into `main`

### 📦 Artifact Handling
- Artifacts generated in `dev` should be reviewed before merging to `main`
- Use commit messages like `Add artifact: output_2025-11-05.txt` for clarity



