# SF Crime Analysis & Prediction

> A data mining and machine learning project for analyzing historical crime patterns in San Francisco and discovering relationships between **location, time, and crime categories**.

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit--learn](https://img.shields.io/badge/scikit--learn-Machine%20Learning-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

---

## Overview

Crime datasets contain valuable spatial, temporal, and categorical information that can be used to understand recurring patterns in criminal activity.

This project analyzes historical San Francisco crime data to:

- Explore the distribution of reported crimes.
- Investigate crime patterns across locations and time.
- Prepare and clean raw data for analysis.
- Identify meaningful relationships between crime-related features.
- Apply clustering techniques to discover groups and patterns in the data.
- Explore how historical patterns can support crime-related analysis and prediction.

The project was developed as a **Data Mining / Machine Learning** project using Python and Jupyter Notebook.

---

## Problem Statement

The main question addressed by this project is:

> **Can historical crime data be used to discover meaningful spatial, temporal, and categorical patterns that help us better understand crime activity in San Francisco?**

The analysis focuses on transforming raw crime records into useful insights through data preprocessing, exploratory analysis, feature preparation, clustering, and predictive analysis.

---

## Dataset

The project uses the **SF Crime Rate Prediction** dataset from Kaggle.

The original/raw dataset is intentionally **not stored in this GitHub repository** because the dataset files are large and should not be committed directly to a standard Git repository.

### Expected data files

Depending on the version of the project, the analysis uses files such as:

```text
train.csv
test.csv
cleaned_train.csv
cleaned_test.csv
```

Place the required dataset files in a local `data/` directory before running the notebook.

> **Note:** Dataset ownership and licensing remain with the original dataset provider. Please follow the original Kaggle dataset's terms when downloading or redistributing the data.

---

## Project Workflow

```text
Raw Crime Data
      │
      ▼
Data Loading
      │
      ▼
Data Cleaning & Preprocessing
      │
      ▼
Exploratory Data Analysis
      │
      ├───────────────┐
      ▼               ▼
Temporal Analysis   Location Analysis
      │               │
      └───────┬───────┘
              ▼
       Feature Engineering
              │
              ▼
          Clustering
              │
              ▼
       Pattern Analysis
              │
              ▼
     Insights & Prediction
```

---

## Methodology

### 1. Data Preprocessing

The preprocessing stage prepares the raw data for analysis by addressing data-quality issues and transforming relevant features.

Typical steps include:

- Inspecting the dataset structure.
- Checking missing values.
- Handling invalid or incomplete records.
- Removing unnecessary columns.
- Correcting data types.
- Preparing categorical and numerical variables.
- Creating analysis-ready datasets.

### 2. Exploratory Data Analysis

The exploratory analysis investigates the main characteristics of crime activity, including:

- Crime category distribution.
- Temporal patterns.
- Geographic patterns.
- Frequency of different crime groups.
- Relationships between selected variables.

Visualizations are used to make these patterns easier to interpret.

### 3. Feature Engineering

Relevant features are prepared and transformed to make them suitable for statistical analysis and machine learning techniques.

### 4. Clustering

Clustering is used to group observations with similar characteristics and investigate whether distinct crime patterns can be identified.

The clustering analysis considers relevant combinations of features such as:

- Location-related information.
- Time-related information.
- Crime categories/groups.

### 5. Prediction / Pattern Forecasting

The project explores the use of historical crime information to support prediction-oriented analysis.

> **Important:** The exact predictive models, target variables, and evaluation metrics should be interpreted from the notebook implementation rather than assumed from the project title.

---

## Key Questions

The analysis investigates questions such as:

1. Which crime categories occur most frequently?
2. How does crime activity vary over time?
3. Are there noticeable geographic differences in crime activity?
4. Can similar crime patterns be grouped together?
5. Which features are most useful for understanding crime patterns?
6. What insights can historical crime data provide for future analysis?

---

## Results

The main findings and quantitative results are documented in the project notebook and final report.

### Results to highlight

After the final notebook cleanup, this section should contain the project's strongest findings, for example:

- **Most common crime categories:** _[add verified result]_
- **Strongest temporal pattern:** _[add verified result]_
- **Important geographic pattern:** _[add verified result]_
- **Best clustering configuration:** _[add verified result]_
- **Predictive model / evaluation result:** _[add verified result]_

> The values above are intentionally left as placeholders until the final notebook is reviewed and the results are verified.

---

## Project Structure

```text
SF-Crime-Analysis-and-Prediction/
│
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
├── notebooks/
│   └── crime_rate_analysis.ipynb
│
├── data/
│   └── README.md
│
├── src/
│   ├── preprocessing.py
│   ├── clustering.py
│   └── visualization.py
│
├── reports/
│   └── final_report.pdf
│
├── assets/
│   ├── workflow.png
│   ├── analysis.png
│   └── results.png
│
└── results/
    └── README.md
```

> Some folders may be added during the final repository refactoring. The structure above represents the intended portfolio-ready organization.

---

## Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and preprocessing |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning and clustering |
| Jupyter Notebook | Interactive analysis and experimentation |
| Git & GitHub | Version control and project documentation |

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Rowan-ali/Crime-Rate.git
cd Crime-Rate
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS / Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add the dataset

Download the required dataset from its original source and place the necessary CSV files inside:

```text
data/
```

Do **not** commit large raw datasets directly to the repository.

### 5. Run the notebook

```bash
jupyter notebook
```

Then open:

```text
notebooks/crime_rate_analysis.ipynb
```

---

## Reproducibility

To reproduce the analysis:

1. Clone the repository.
2. Create a clean Python environment.
3. Install the dependencies from `requirements.txt`.
4. Download the required dataset.
5. Place the data in the expected `data/` directory.
6. Run the notebook from top to bottom.

---

## Limitations

Crime data analysis has important limitations.

- Historical crime records represent **reported incidents**, not necessarily all crimes that occurred.
- Observed patterns should not automatically be interpreted as causal relationships.
- Geographic patterns may be influenced by population density, reporting behavior, policing practices, and other factors.
- Predictive results depend strongly on data quality, feature selection, and model assumptions.
- The project should be used for analytical and educational purposes rather than as a standalone decision-making system.

---

## Future Improvements

Potential improvements include:

- Building a reproducible preprocessing pipeline.
- Comparing multiple clustering algorithms.
- Performing systematic hyperparameter tuning.
- Adding stronger model evaluation and cross-validation.
- Developing an interactive dashboard.
- Adding geographic visualizations and crime heatmaps.
- Creating a lightweight prediction API or web application.
- Automating data preprocessing and model training.

---

## Documentation

The repository includes:

- **Jupyter Notebook:** Complete exploratory and modeling workflow.
- **Final Report:** Detailed project documentation.
- **README:** Project overview, setup instructions, methodology, and limitations.

---

## Author

**Rowan Ali**

GitHub: [@Rowan-ali](https://github.com/Rowan-ali)

---

## License

This project is intended for educational and portfolio purposes.

If a specific license is added to the repository, refer to the `LICENSE` file for the applicable terms.
