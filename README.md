# OTT Streaming Viewing Patterns & Genre Association Mining Using R

## Project Overview

This project analyzes user viewing behavior on an OTT streaming platform and applies association rule mining to discover relationships between content genres.

Using the KION streaming dataset, the project explores viewing interactions, genre popularity, user engagement, and frequently occurring genre combinations. The discovered patterns can help explain audience preferences and support data-driven content discovery and recommendation strategies.

## Problem Statement

OTT platforms generate large volumes of user interaction data. Analyzing this data can reveal which genres attract viewers, how users engage with content, and which genres frequently occur together.

This project uses data analysis and association rule mining to extract meaningful patterns from streaming interaction data.

## Objectives

- Analyze OTT user viewing patterns.
- Identify popular content genres.
- Study user engagement using viewing-related attributes.
- Discover frequent genre combinations using association rule mining.
- Evaluate associations using support, confidence, and lift.
- Export analysis results into CSV files for further exploration.

## Dataset

The project uses the KION streaming dataset, consisting of the following files:

| File | Description |
|---|---|
| `interactions.csv` | User-content interactions and viewing-related information |
| `items_en.csv` | Content metadata, including item information and genres |
| `users_en.csv` | User-related metadata |

These datasets are combined where necessary to connect viewing interactions with content genres and user information.

**Note:** The exact columns and available records depend on the dataset version used in the analysis.

## Technologies Used

- **Programming language:** R
- **Development environment:** Google Colab
- **Data processing:** Data cleaning, transformation, and aggregation
- **Data mining:** Association rule mining
- **Algorithms:** Apriori and Eclat, where implemented in the notebook
- **Output format:** CSV
- **Version control:** Git and GitHub

## Methodology

### 1. Data Loading

Load the dataset files into the analysis environment and inspect their structure, dimensions, and column names.

### 2. Data Preprocessing

Inspect missing values, clean relevant fields, and prepare the viewing interaction and genre information for analysis.

### 3. Exploratory Data Analysis

Explore the distribution of genres, viewing interactions, and engagement-related attributes to understand the dataset.

### 4. Genre Analysis

Analyze genre popularity and identify genres that appear frequently in the available content and viewing data.

### 5. Transaction Preparation

Transform the genre data into a transaction-based representation suitable for frequent itemset mining.

### 6. Association Rule Mining

Apply the association mining methods implemented in the notebook to discover relationships among genres.

### 7. Rule Evaluation

Evaluate discovered rules using:

- **Support:** How frequently an itemset appears in the transactions.
- **Confidence:** How often the consequent occurs when the antecedent occurs.
- **Lift:** How strongly the observed association differs from what would be expected if the items were independent.

A lift greater than 1 indicates a positive association, while a lift near 1 indicates little association beyond independence.

### 8. Result Export

Save the generated association rules and selected top genre rules as CSV files for further analysis.

## Project Outputs

The analysis generates CSV outputs, including:

- `ott_genre_association_rules.csv` — discovered genre association rules.
- `ott_top20_genre_rules.csv` — selected top 20 genre-related rules.

These files can be inspected using spreadsheet software or further analyzed using R.

## Applications

- Understanding audience genre preferences.
- Exploring relationships between content genres.
- Supporting OTT content discovery.
- Providing insights for genre-based recommendation strategies.
- Supporting data-driven content catalog planning.

## Limitations

- Findings depend on the quality and coverage of the available dataset.
- Association rules describe relationships, not causal effects.
- Results depend on transaction construction and rule-mining thresholds.
- Observed viewing interactions may not represent every OTT user or platform.

## Future Enhancements

- Build an interactive dashboard for viewing patterns and genre associations.
- Explore personalized recommendations based on viewing history.
- Compare association patterns across user groups.
- Evaluate results using additional datasets and alternative mining techniques.

## Repository Contents

The repository is intended to contain:

- The main analysis notebook.
- This README documentation.
- Exported association rule CSV files.
- Additional project code and supporting files, where applicable.

## How to Run

1. Clone or download this repository.
2. Open the analysis notebook in Google Colab.
3. Obtain and upload the required KION dataset files.
4. Install or load the R packages specified in the notebook.
5. Run the notebook cells in order.
6. Review the analysis and generated CSV outputs.

## Author

**Akhil Kandibanda**

Chaitanya Bharathi Institute of Technology (CBIT), Hyderabad

Artificial Intelligence and Data Science

---

*This project was developed for academic learning in data analysis and association rule mining.*
