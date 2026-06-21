# AGENTIC_AI_LEARNING

A concise, hands-on collection of experiments, notebooks, and example apps for learning about applied agentic AI, health-data analysis, and lightweight LLM integrations.

## Project Overview

AGENTIC_AI_LEARNING is a personal learning workspace that combines data analysis, interactive demos, and small experiments in working with language models. The repository is structured to make it easy to run example workflows (including a Streamlit demo), explore Jupyter notebooks, and experiment with minimal LLM calls.

This repo focuses on clarity and reproducibility — each folder contains a focused example or experiment with minimal dependencies so you can run and extend the examples quickly.

## Contents

- `main.py` — repository-level entry script for quick tests or demos.
- `pyproject.toml` — project metadata and dependency specification.
- `Health_Analysis/` — health-focused examples and a Streamlit demo.
  - `blood_work.txt` — sample data used by the analysis notebooks.
  - `health_analysis.ipynb` — exploratory analysis notebook (pandas, plotting).
  - `streamlit_app/` — Streamlit demo app folder.
    - `app.py` — interactive Streamlit application for the health analysis.
- `simple_llm_calling/` — minimal example(s) showing how to call an LLM from a notebook.
  - `call_llm.ipynb` — notebook demonstrating a small LLM integration.

## Quickstart

Prerequisites:

- Python 3.8+ installed.
- Recommended: create a virtual environment.

Create and activate a virtual environment (Windows example):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install --upgrade pip
```

Install dependencies:

If this repo provides a `requirements.txt` file, install from it. Otherwise, use `pyproject.toml` or install dependencies manually.

```bash
pip install -r requirements.txt   # if present
# or
pip install -e .                  # when a package is defined in pyproject.toml
```

Running the Streamlit demo:

```bash
streamlit run Health_Analysis/streamlit_app/app.py
```

Open `http://localhost:8501` in your browser to view the app.

Running the main script:

```bash
python main.py
```

# Working:
<img width="500" height="300" alt="Use AI Image Jun 21, 2026, 11_31_46" src="https://github.com/user-attachments/assets/e543aa2a-83ef-4ea4-90ae-95bea4792ce3" />

---

Opening the notebooks:

Launch Jupyter or open the notebooks in VS Code:

```bash
jupyter lab
# then open Health_Analysis/health_analysis.ipynb or simple_llm_calling/call_llm.ipynb
```

## Notebooks and Examples

- `Health_Analysis/health_analysis.ipynb` — exploratory data analysis on the included sample blood-work data and visualization examples.
- `simple_llm_calling/call_llm.ipynb` — demonstrates a minimal pattern for calling an LLM from Python. Replace any placeholder API keys with your own and follow secure practices.

## Development notes

- Keep secrets (API keys) out of the repository. Use environment variables or a secure secrets manager.
- If you add packages, update `pyproject.toml` or add a `requirements.txt` to make onboarding easier.

## Contributing

Contributions are welcome. Recommended workflow:

1. Fork the repo and create a branch for your change.
2. Make incremental, focused commits with clear messages.
3. Open a pull request describing the change and the motivation.

If you add new examples, include a short README or notebook cell that explains how to run them.

## License & Contact

This workspace is intended for learning and experimentation. If you want a formal license, add a `LICENSE` file. For questions or collaboration, open an issue or contact the repository owner.
