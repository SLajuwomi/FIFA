# FIFA 19 Player Undervaluation Analysis Notebook

## Project Description

This Jupyter Notebook analyzes the FIFA 19 Complete Player Dataset using unsupervised learning (DBSCAN) to identify potentially undervalued player archetypes within specific positions (e.g., Strikers). The analysis focuses on clustering players based on position-specific composite skill metrics versus their market value ('Value').

This project fulfills the requirements for the AI class assignment and serves as a practical example for CS students and football analysts interested in player valuation.

## Data Source

The analysis uses the [FIFA 19 Complete Player Dataset](https://www.kaggle.com/datasets/javagarm/fifa-19-complete-player-dataset) available on Kaggle.

_(Original source link mentioned in technical specification was: https://www.kaggle.com/datasets/stefanoleone992/fifa-19-complete-player-dataset - this link appears dead, using the one provided in the implementation plan)_

## Setup and Usage

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Place the dataset:** Download the `FIFA_19_COMPLETE_PLAYER_DATASET.csv` file from the Kaggle link above. Place the file in the root directory of this project, alongside the `fifa19_undervaluation_analysis.ipynb` notebook. (Alternatively, you can place it in a `./data/` subdirectory and update the `data_path` variable in Step 3 of the notebook).
3.  **Install dependencies:** It is recommended to use a virtual environment.
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    # Optionally, create a requirements.txt file and run: pip install -r requirements.txt
    ```
4.  **Run Jupyter Notebook:**
    ```bash
    jupyter notebook fifa19_undervaluation_analysis.ipynb
    ```
    Alternatively, open the notebook in Jupyter Lab, VS Code, or Google Colab (uploading the data file might be necessary for Colab).

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
