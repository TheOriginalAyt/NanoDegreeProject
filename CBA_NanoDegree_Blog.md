```markdown
# 📘 Commercial Business Applications Analysis

## 📌 Overview

This notebook analyzes weekly business application data across U.S. regions, focusing on **Commercial Business Applications (CBA)**. It uses Python libraries to load, explore, and visualize trends in business formation statistics, particularly highlighting regional and temporal patterns.

---

## 📊 Data Source

- **Dataset**: https://www.census.gov/econ/bfs/data/weekly.html
- **Data Dictionary**: https://www.census.gov/econ/bfs/pdf/bfs_weekly_data_dictionary.pdf
- **File Used**: `region_bfa.csv` (loaded via `pandas.read_csv()`)

---

## 🧰 Requirements

Ensure the following Python packages are installed:

```bash
pip install pandas numpy matplotlib seaborn
```

Optional (commented out in the notebook):
```bash
pip install scikit-learn
```

---

## ▶️ How to Run

1. Clone or download the repository containing this notebook.
2. Place the `region_bfa.csv` file in the same directory.
3. Run the notebook using Jupyter or any compatible Python environment.

---

## 📈 Visualizations

The notebook includes:

- **Histogram**: Distribution of Commercial Business Applications (`CBA_NSA`) by region.
- **Line Plot**: Weekly trend of `CBA_NSA` across regions.
- **Subplots**: Multiple time series plots for variables like `BA_NSA`, `HBA_NSA`, `WBA_NSA`, and their year-over-year changes.

---

## 🧠 Key Functions

```python
def df_details(df):
    print("Description of DataFrame:")
    print(df.describe())
    print("DataFrame Head:")
    print(df.head())
    print("DataFrame Columns:")
    print(df.columns)
```

This function provides a quick summary of the dataset's structure and statistics.

---

## 📌 Notes

- The notebook uses `matplotlib` and `seaborn` for plotting.
- Data spans from 2006 to 2025 and includes regional breakdowns (`Fregion`) and various business application metrics.
```