# Arsenal Player Impact Analysis

## Project Goal
Quantify which Arsenal players have the greatest impact on match outcomes using supervised machine learning.

## Motivation
Traditional metrics such as goals and assists fail to capture the full contribution of defenders and midfielders.
This project uses match-level and player-level data to model Arsenal's goal difference and identify true drivers of success.

## Target Variable
Goal difference = Arsenal goals − opponent goals

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
