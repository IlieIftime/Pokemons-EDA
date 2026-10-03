# Pokémon Unsupervised Learning and Exploratory Data Analysis

This repository contains a university project focused on **unsupervised machine learning** and exploratory data analysis using a dataset of Pokémon. The main deliverable is a Jupyter Notebook that documents the complete analysis workflow, from data characterization and cleaning to dimensionality reduction and clustering.

## Project objectives

The notebook investigates the relationships between Pokémon attributes and aims to:

- Explore the distribution of Pokémon types and statistics;
- Prepare the dataset for unsupervised learning;
- Reduce the dimensionality of the numerical features;
- Identify groups of Pokémon with similar characteristics;
- Compare and interpret clustering results;
- Detect potential atypical observations or outliers;
- Draw conclusions about the structure of the dataset.

## Dataset

The analysis uses the Pokémon dataset originally published on Kaggle:

- **Rows:** 800 Pokémon
- **Original columns:** 13
- **Main attributes:** name, primary type, secondary type, total base statistics, HP, Attack, Defense, Special Attack, Special Defense, Speed, Generation, and Legendary status.

The dataset is included in the repository as [`Pokemon.csv`](Pokemon.csv).

## Analysis workflow

The notebook is organized into the following stages:

1. **Problem definition** — formulation of the unsupervised learning task.
2. **Dataset characterization** — description of the variables and their types.
3. **Data wrangling** — loading the CSV file, removing the redundant `#` column, renaming variables for readability, checking missing values, and treating missing secondary Pokémon types as `Inexistente`.
4. **Exploratory data analysis** — inspection of descriptive statistics, categorical distributions, Pokémon types, and relationships between numerical attributes.
5. **Dimensionality reduction** — application and interpretation of techniques including PCA, t-SNE, and UMAP to represent the data in lower-dimensional spaces.
6. **Clustering** — application of unsupervised clustering methods to group Pokémon according to their characteristics.
7. **Cluster analysis** — visualization and interpretation of the groups, including the identification of possible outliers.
8. **Conclusion and bibliography** — summary of the main findings and references used in the study.

## Repository contents

- [`TUT1_TDIA_112779.123557.123554_VF.ipynb`](TUT1_TDIA_112779.123557.123554_VF.ipynb) — main notebook containing the analysis, visualizations, dimensionality-reduction techniques, clustering work, and conclusions.
- [`Pokemon.csv`](Pokemon.csv) — dataset used by the notebook.
- [`LICENSE`](LICENSE) — MIT license.

## Requirements

Python 3.8 or later is recommended. The notebook uses common data-analysis and visualization libraries, including:

- pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook or JupyterLab

Depending on the notebook sections being executed, additional dimensionality-reduction or visualization packages may be required, such as `umap-learn`.

## Getting started

1. Clone the repository and move into its directory:

   ```bash
   git clone https://github.com/IlieIftime/Pokemons-EDA.git
   cd Pokemons-EDA
   ```

2. Install the core dependencies:

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter umap-learn
   ```

3. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

4. Open `TUT1_TDIA_112779.123557.123554_VF.ipynb` and run the cells sequentially.

> The notebook reads the dataset using the relative path `Pokemon.csv`, so the notebook and CSV file should remain in the repository root unless the path is updated.

## Authors

- Ilie Iftime — 112779
- Inês Cruz — 123557
- Sofia Quintino — 123554

## License

This project is distributed under the MIT License. See [`LICENSE`](LICENSE) for details.
