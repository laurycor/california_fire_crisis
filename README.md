# California Fire Crisis Analysis

## Overview
This project analyzes wildfire activity in California using historical fire data. The purpose of the project is to explore trends in wildfire size, frequency, and damage, while demonstrating a clean and reproducible data science workflow. The primary outputs of this project are summary tables and visualizations that highlight patterns in wildfire behavior over time.

This repository was professionalized as part of **CMSE 492 (Data Science Capstone), Day 06**, and is intended to be easily understood and reproduced by other students.

---

## Project Structure

The repository is organized as follows:
california_fire_crisis/
├── src/ # Core analysis scripts
├── notebooks/ # Exploratory Jupyter notebooks
├── data/
│ ├── raw/ # Original input data
│ └── processed/ # Cleaned / transformed data
├── results/
│ ├── figures/ # Generated plots
│ └── tables/ # Generated summary tables
├── README.md # Project documentation
├── .gitignore # Files ignored by Git
├── pyproject.toml # Project metadata and dependencies
└── uv.lock # Locked dependency versions
---

## Data

This project uses publicly available wildfire data related to fires in California.


### Important notes about the data
- Large raw data files may **not** be included directly in this repository.
- If the analysis scripts fail due to missing data, download the appropriate wildfire datasets and place them in `data/raw/` before running the scripts.
- File paths in the code assume the project is run from the **root directory**.

---

## Environment Setup (uv)

This project uses **uv** for Python environment management.

### Step 1: Install uv (if not already installed)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
Step 2: Create and synchronize the environment
From the project root directory, run:
uv sync
This command will:
Create a virtual environment in .venv/
Install all required Python dependencies
Step 3: Activate the environment
source .venv/bin/activate
After activation, all Python commands will use the project’s environment.


Reproducing Results
Follow these steps exactly in order to reproduce one of the project’s results.
Step 1: Make sure the environment is active
source .venv/bin/activate
Step 2: Run the main analysis script
python src/run_everything.py
Step 3: View the outputs
Generated plots will appear in:
results/figures/


Generated summary tables will appear in:
results/tables/
If the script fails due to missing data files, download the required data and place it in data/raw/, then re-run the script.

Troubleshooting / Known Issues
Python 3.10 or newer is recommended.
All commands should be run from the project root directory.
Missing data files will cause scripts to fail until data is added to data/raw/.
On Windows systems, environment activation commands may differ slightly.
Some scripts may take a few seconds to complete depending on system performance.
