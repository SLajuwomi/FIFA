# FIFA 19 Player Undervaluation Analysis Notebook

## Project Description

This Jupyter Notebook performs unsupervised learning (DBSCAN) on the FIFA 19 player dataset to identify potentially undervalued player archetypes within specific positions (e.g., Strikers). The analysis focuses on clustering players based on position-specific composite skill metrics versus their market value ('Value'). The notebook follows the structure required for an AI class assignment, including introduction, EDA, preprocessing, model training/tuning, and conclusion.

## Data Source

The analysis uses the "FIFA 19 Complete Player Dataset" available on Kaggle:
[https://www.kaggle.com/datasets/javagarm/fifa-19-complete-player-dataset](https://www.kaggle.com/datasets/javagarm/fifa-19-complete-player-dataset)
_(Note: The technical specification linked to a different dataset URL, but this plan uses the one specified here)_

## Setup and Execution

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Download the dataset:** Download `FIFA_19_COMPLETE_PLAYER_DATASET.csv` from the Kaggle link above.
3.  **Place the dataset:** Place the downloaded CSV file in the root directory of this project (the same directory as the `fifa19_undervaluation_analysis.ipynb` notebook). Alternatively, create a `data/` subdirectory and place the CSV file inside it, then update the `data_path` variable in the notebook accordingly.
4.  **Install dependencies:** Ensure you have Python installed. It is recommended to use a virtual environment. Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    # Or, if a requirements.txt file is provided:
    # pip install -r requirements.txt
    ```
5.  **Run Jupyter Notebook:** Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    # or
    # jupyter lab
    ```
    Open the `fifa19_undervaluation_analysis.ipynb` file and run the cells sequentially.

## Notebook Structure

The notebook is structured as follows:

1.  **Introduction:** Problem definition, goal, data source, methodology.
2.  **Data Loading and Initial Exploration:** Loading the dataset and performing basic checks.
3.  **Data Preprocessing:** Cleaning, type conversions, handling missing values.
4.  **Feature Engineering:** Calculating a composite skill score for Strikers.
5.  **Exploratory Data Analysis (Post-Preprocessing):** Visualizing cleaned data and engineered features.
6.  **Unsupervised Learning (DBSCAN):** Filtering, scaling, hyperparameter tuning, and model application.
7.  **Analysis of Undervalued Archetypes:** Visualizing clusters, identifying undervalued groups, displaying sample players.
8.  **Conclusion:** Summarizing findings, evaluating the approach, discussing limitations, suggesting future work.
9.  **References:** Data source link.
