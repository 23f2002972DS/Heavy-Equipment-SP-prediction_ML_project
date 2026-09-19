# Heavy Equipment Selling Price Prediction

A Kaggle notebook for exploratory data analysis, feature engineering, preprocessing, and regression modeling to predict heavy-equipment selling prices.

## Contents

- `23f2002972-notebook-2026t2.ipynb`: analysis and modeling notebook
- `requirements.txt`: Python packages used by the notebook

## Dataset

The notebook currently expects the Kaggle competition files at:

```text
/kaggle/input/competitions/heavy-equipment-selling-price-prediction-challenge/
```

The expected files are `train.csv`, `test.csv`, `sample_submission.csv`, and `metadata.csv`. The dataset is not included in this repository. Run the notebook on Kaggle, or update the four paths in the data-loading cell when running locally.

## Run locally

1. Create and activate a virtual environment:

   ```powershell
   py -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

2. Install dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

3. Open the notebook in VS Code and select the `.venv` Python kernel.

4. Place the competition data in a local folder and update the data paths in the notebook, or run it in Kaggle where the original paths already exist.

## Notes

- The notebook uses a log-transformed target and evaluates models with RMSLE-aligned validation.
- Do not commit Kaggle API keys, private data, or generated submission files.
