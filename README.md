# SDSS Hackathon 2026 — Airline Route & Fare Analysis

A data science project analyzing US domestic airline routes, fares, and market competition. Built for the SDSS 2026 Datathon.

## Notebooks

| Notebook | Description |
|----------|-------------|
| `Analysis.ipynb` | Data loading, cleaning, exploratory data analysis, and a Random Forest fare prediction model |
| `InteractiveDashboards.ipynb` | Interactive Plotly dashboards with ipywidgets for exploring routes and fares |
| `traveler_strategy_tool TEST.ipynb` | Traveler-facing tool for comparing carriers and choosing routes |

## Prerequisites

- **Python 3.10+** (developed on 3.13)
- **pip**
- The dataset file `airline_ticket_dataset.xlsx` is already included in the repo

## Setup

1. **Clone the repository**

   ```bash
   git clone <repo-url>
   cd SDSS-hackathon
   ```

2. **Create a virtual environment**

   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment**

   macOS / Linux:
   ```bash
   source .venv/bin/activate
   ```

   Windows:
   ```powershell
   .venv\Scripts\activate
   ```

4. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

5. **Register the Jupyter kernel**

   ```bash
   python -m ipykernel install --user --name sdss --display-name "SDSS Hackathon"
   ```

## Running the Notebooks

1. Start the Jupyter server:

   ```bash
   jupyter notebook
   ```

2. Open a notebook in the browser and select the **SDSS Hackathon** kernel from **Kernel > Change Kernel**.

3. Recommended run order:
   - `Analysis.ipynb` — run first (loads and cleans the data, builds the model)
   - `InteractiveDashboards.ipynb` — interactive exploration of routes and fares
   - `traveler_strategy_tool TEST.ipynb` — traveler strategy tool

## Dataset

`airline_ticket_dataset.xlsx` contains 14,004 rows and 21 columns of US domestic airline route data, including city pairs, distances, passenger counts, fares, carrier market shares, and market structure metrics.
