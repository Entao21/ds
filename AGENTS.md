# AGENTS.md

## Cursor Cloud specific instructions

This is a Python data science educational repository containing Jupyter notebooks for a supervised learning course (DSSS). There is no backend, no database, and no build system — only Jupyter notebooks.

### Services

| Service | Command | Notes |
|---------|---------|-------|
| JupyterLab | `jupyter lab --ip=0.0.0.0 --port=8888 --no-browser --ServerApp.token='' --allow-root` | Only service; serves notebooks from `/workspace` |

### Key dependencies

All Python packages are installed globally via pip: `jupyter`, `jupyterlab`, `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `xgboost`, `scipy`.

No `requirements.txt` exists in the repo; the update script installs packages directly.

### Running notebooks

- Execute all cells via JupyterLab UI (Run > Run All Cells), or headlessly: `jupyter nbconvert --to notebook --execute <notebook>.ipynb`
- Notebooks fetch data from remote GitHub URLs at runtime, so internet access is required.
- `tree_based_methods_practical.ipynb` contains exercise cells with `??` placeholders (intentional — do not "fix" them).

### Notes

- `$HOME/.local/bin` must be on `PATH` for the `jupyter` command to be found.
- No linting, testing frameworks, or build systems are configured in this repo.
