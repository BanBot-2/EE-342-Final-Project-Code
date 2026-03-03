# 1. Directory & File Organization

- Place all scripts in `src/`.
- Place exploratory notebooks in `notebooks/`, calling functions from `src/`.
- Final report should be a Jupyter notebook in the root folder, helper functions used should be placed inside the notebook instead of calling from `src/`
- Do not make any changes to `data/raw`, processed data should be stored in `data/processed`.

---

# 2. Reproducibility Requirements

- Use relative paths.
- Use Conda for environment management, store environment configuration in `environment.yml`.


# Conda Setup Guide (Quick Start)

## 1) Assume Miniconda/Anaconda installed
---

## 2) Set up from an `environment.yml` 

### A) Create the environment from the file
From the repo root (where `environment.yml` is located):
```bash
conda env create -f environment.yml
```

Activate it (use the `name:` inside the YAML):
```bash
conda activate <env-name>
```

## 3) Notes

### Mixing `conda` and `pip`
- Prefer `conda install` when possible.
- Use `pip` only when a package isn’t available on conda channels.
- If you use pip, include it under `pip:` in `environment.yml`.