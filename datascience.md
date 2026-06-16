# Actor-Character Age Difference Data Science Project

## Overview

This project performs exploratory data analysis (EDA) on an actor-character age difference dataset. The analysis focuses on understanding relationships between actors' ages, character ages, release dates, and age differences using Python data science tools.

## Dataset

The project uses:

- `actor_character_age_difference.csv`

The dataset contains information such as:

- Actor name
- Actor age
- Character age
- Age difference
- Movie title
- Release date
- Additional actor and character attributes

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas for analysis and manipulation.

### 2. Data Cleaning

Data preprocessing steps include:

- Checking for missing values
- Removing null records
- Removing duplicate rows
- Dropping unnecessary columns
- Renaming columns for consistency

Examples:

- `love_interest` column removed
- `birthday` renamed to `dob`

### 3. Statistical Analysis

Descriptive statistics are calculated for numerical features including:

- Sum
- Mean
- Median
- Minimum
- Maximum

The analysis particularly focuses on actor age distributions.

### 4. Data Aggregation

Grouping and aggregation techniques are applied using Pandas:

- Grouping actors by name
- Summarizing release dates
- Generating dataset-level insights

### 5. Data Visualization

Several visualizations are created using Matplotlib:

#### Line Plot
- Character age vs movie title

#### Histogram
- Distribution of actor ages

#### Scatter Plot
- Age difference vs actor age

These visualizations help identify trends and patterns within the dataset.

## Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib

## Installation

```bash
pip install pandas numpy matplotlib
```

## Running the Project

1. Open the Jupyter Notebook.
2. Place the dataset file in the working directory.
3. Run all notebook cells sequentially.
4. Review the generated statistics and visualizations.

## Project Structure

```text
.
├── ahmed_moniem_jana_tera_data_science_project.ipynb
├── actor_character_age_difference.csv
└── actor_character_age_difference.md
```

## Key Analysis Objectives

- Explore actor and character age relationships
- Measure age differences between actors and portrayed characters
- Identify patterns in casting trends
- Visualize age-related distributions and correlations

## Future Improvements

- Add advanced statistical testing
- Create interactive visualizations
- Include correlation analysis
- Build predictive models using machine learning
- Develop dashboards for data exploration

## Authors

Ahmed Moniem
Jana Tera
