# Data Science Pipeline Project

## Overview

This project implements a comprehensive data science pipeline for classifying customer reviews. It encompasses all stages of a typical data science workflow—from data ingestion and exploratory analysis to preprocessing, modeling, evaluation, and hyperparameter tuning. Built with industry-standard tools, this pipeline demonstrates best practices in both software engineering and data science.

## Features

- **Data Ingestion & Exploration:**  
  - Reads the dataset from a CSV file.
  - Performs detailed exploratory data analysis (EDA) to assess data distribution, missing values, and class imbalance.
  
- **Preprocessing & Feature Engineering:**  
  - Utilizes a custom spaCy-based transformer for text preprocessing (lemmatization and stopword removal).
  - Implements separate pipelines for numerical, categorical, and text features using scikit-learn’s `Pipeline` and `ColumnTransformer`.
  
- **Modeling:**  
  - Integrates a `RandomForestClassifier` within a unified pipeline.
  - Conducts hyperparameter tuning with GridSearchCV to optimize model performance.
  
- **Visualization & Evaluation:**  
  - Generates comprehensive visualizations, including plots of feature distributions, class imbalances, and confusion matrices.
  - Creates Word Clouds to visualize key terms in review texts.
  - Provides detailed classification reports and accuracy metrics.

## Technologies Used

- **Python 3.x**
- **Pandas & NumPy:** For data manipulation and numerical analysis.
- **Matplotlib & Seaborn:** For creating visualizations.
- **spaCy:** For advanced natural language processing.
- **WordCloud:** For text data visualization.
- **scikit-learn:** For building machine learning models and pipelines.
- **Jupyter Notebook / Google Colab:** For interactive development and experimentation.

## Installation and Setup

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/rruisan/dsnd-pipelines-project
    cd ds-pipeline-project
    ```
2. **Create a Virtual Environment (Recommended):**
    Ensure that you have a requirements.txt file listing all necessary packages. Then, run:
    ```bash
    python -m venv env
    source env/bin/activate  # For Windows: env\Scripts\activate
    ```

3. **Install Dependencies:**
    Ensure that you have a requirements.txt file listing all necessary packages. Then, run:
    
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the spaCy English Model:**
    ```bash
    python -m spacy download en_core_web_sm
    ```


## Usage

- **Interactive Exploration:**
  
  Open the notebook.ipynb file in Jupyter Notebook or Google Colab to explore the pipeline interactively.

- **Running as a Script:**
  
    If preferred, convert the notebook to a Python script:
    ```bash
    jupyter nbconvert --to script notebook.ipynb
    python notebook.py
    ```

## License

See the LICENSE.txt file for details.


