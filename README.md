## Analysis 1 — Minutes-based Player Impact (Ridge & Lasso)

**Question:** Which Arsenal players are most associated with improved match outcomes?

**Approach:**
- Target: `goal_diff = GF - GA` (match-level)
- Features: player minutes (one feature per player) + `is_home`
- Models:
  - Ridge regression for stable impact estimates under multicollinearity
  - Lasso regression for a sparse shortlist of impactful players
- Interpretation focused on players with **≥900 total minutes** to reduce small-sample noise.

### Key visuals
![Top & Bottom Impact Players](reports/figures/impact_top_bottom_ridge.png)
![Minutes vs Impact](reports/figures/minutes_vs_impact.png)

### Notes on interpretation
- Coefficients represent **associations**, not causal effects.
- Predictive performance (R²) is not the main goal; the emphasis is interpretability and robustness.
- Player impact is context-dependent (teammates, tactics, opposition, season effects).


## Project Structure
- `data/`: raw and processed datasets
- `notebooks/`: exploratory analysis, feature engineering, and modeling
- `src/`: reusable Python modules
- `reports/`: figures and written summaries

## Status
🚧 Project setup complete. Data ingestion next.

## Installation

1. Clone the repository
```bash
git clone https://github.com/Rohayne/arsenal-player-impact.git
cd arsenal-player-impact

2. Create and activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt

4. Launch Jupyter Notebook
jupyter notebook
