# Ethical AI Data Analysis

## Project Overview
This project aims to analyze data related to ethical concerns in Artificial Intelligence (AI). The goal is to identify trends, main themes, and concerns regarding AI ethics by processing a dataset of relevant articles. The analysis may involve identifying patterns in AI articles, keyword analysis, and understanding predominant ethical concerns.

## Features
- **Data Loading**: Loads CSV data files from URLs, including Google Drive links.
- **Exploratory Data Analysis (EDA)**:
  - Displays the first rows of data, general information, and descriptive statistics of numeric variables.
  - Generates visualizations such as histograms, bar charts, line plots, scatter plots, boxplots, and a correlation matrix.

## Functions
### `carregar_dados(url, tipo_arquivo='CSV')`
- Loads data from CSV files from a given URL, with support for Google Drive links.
- Returns the data as a pandas DataFrame.

### `analise_exploratoria(df)`
- Conducts exploratory analysis by displaying the first few rows, general information, and descriptive statistics.
- Calls visualization functions to generate various graphs to help understand the data.

### Visualizations
- `plot_histograma(df)`: Generates a histogram of a randomly selected numeric variable.
- `plot_grafico_de_barras(df)`: Generates a bar chart for a randomly selected categorical variable.
- `plot_grafico_de_linha(df)`: Creates a line plot comparing two numeric variables.
- `plot_grafico_de_dispersao(df)`: Displays a scatter plot for two numeric variables.
- `plot_boxplot(df)`: Displays the distribution of numeric variables in a boxplot.
- `identificacao_correlacoes(df)`: Generates a correlation matrix to identify relationships among numeric variables.

### `analise_especialista()`
- Allows the analyst to add specialized insights based on observations made during exploratory analysis.

### `main(urls)`
- Loads data from a list of URLs and performs exploratory analysis on each dataset.
- Calls the specialized analysis function after the exploratory analysis.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/ethical-ai-analysis.git
   cd ethical-ai-analysis
