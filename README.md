# House Price Prediction (Pakistan)

This project predicts house prices in Pakistan using the Zameen dataset. The full workflow is implemented in a single notebook: data cleaning, exploratory analysis, model training/evaluation, and an interactive Gradio interface.

## Features

- Data loading from a pipe-delimited CSV (`data/zameen.csv`)
- Data cleaning and numeric conversion for `price`, `bedrooms`, `baths`, and `size`
- One-hot encoding for `city` and `location`
- EDA visualizations:
   - Price distribution (clipped at the 99th percentile for visualization)
   - Size vs. price scatter plot
   - Top 10 city-location combinations
- Two prediction models:
   - Linear Regression
   - MLPRegressor pipeline (with feature scaling and target scaling)
- Evaluation metrics:
   - Mean Absolute Error (MAE)
   - R-squared
- Interactive Gradio app launched from the last notebook cell

## Dataset

- File: `data/zameen.csv`
- Delimiter: `|`
- Columns used by the model:
   - `price`
   - `city`
   - `location`
   - `bedrooms`
   - `baths`
   - `size`

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- scikit-learn
- Gradio
- Jupyter

## Project Structure

```
homevalue/
├── data/
│   └── zameen.csv
├── instructions/
│   ├── AI2002 Course Outline- Spring 2026 (2).docx
│   ├── Project Part 1 Submission (1).docx
│   └── docx_extracted_text.txt
├── main.ipynb
├── README.md
└── requirements.txt
```

## Run Locally

1. Create and activate a virtual environment (optional but recommended).
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Start Jupyter:

```bash
jupyter notebook
```

4. Open `main.ipynb` and run cells from top to bottom.

## Launch the Gradio App

There is no separate `app.py` file in this project. The Gradio interface is defined and launched inside the final cell of `main.ipynb`.

Run the notebook through the final cell to start the app.

## Notes

- The app supports both model choices (Linear Regression and ANN/MLP).
- The UI includes environmental adjustment toggles (for example near park/commercial, corner facing), and also shows an inflation/interest-adjusted estimate.
