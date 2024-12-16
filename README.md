# TDS-Project-2
Automated Analysis

This repository contains a Python-based tool designed for automated data analysis and visualization. It leverages OpenAI’s language model (via an API proxy) to generate narratives and suggest insights based on data analysis results. The tool supports exploratory data analysis (EDA), visualizations, and narrative generation for datasets in CSV format.

Features

Automatic Encoding Detection: Uses chardet to detect file encoding for seamless CSV loading.

LLM-Powered Analysis: Generates data insights and narratives with OpenAI's GPT-based models.

Custom Visualizations:

Distribution plots for numerical features.
Correlation heatmap for exploring relationships between variables.

Narrative Generation: Provides insights into data trends, outliers, and recommendations for further analysis.
Easy Export: Saves generated narratives and visualizations to an output folder named after the dataset.

Requirements

Python Version: Requires Python 3.11 or higher.

Dependencies

The following Python libraries are required:

seaborn, pandas, matplotlib, httpx, chardet, ipykernel, openai, numpy, scipy

To install the dependencies, run:

pip install -r requirements.txt

Setup

Clone the Repository:

git clone <repository_url>
cd <repository_name>

Set the API Token:
Export your OpenAI API proxy token as an environment variable:

export AIPROXY_TOKEN=<your_token_here>

Usage

Running the Script

To execute the script, provide the path to a CSV file as a command-line argument:

python script.py <file_path>

Example

python script.py data/happiness.csv

Outputs

Narrative: A README-style summary with insights and recommendations.

Visualizations: PNG files for key distributions and correlation heatmap.

Outputs are saved in a folder named after the input dataset (e.g., happiness).

Key Functionalities

1. Data Loading

Detects file encoding with chardet and loads CSV files seamlessly.

2. Data Analysis

Computes summary statistics, missing values, and correlation matrices.

Performs hypothesis testing (if applicable).

3. Visualizations

Generates:

Distribution plots for key numerical columns.

Correlation heatmap for all numerical features.

4. Narrative Generation

Utilizes OpenAI’s GPT-based model to generate:

Analysis summaries.

Insights on trends, outliers, and correlations.

Recommendations for further analyses, such as clustering or anomaly detection.

License

This project is licensed under the MIT License.

Acknowledgments

OpenAI for the GPT-based API.

Developers of seaborn, pandas, matplotlib, and scipy for excellent tools that made this project possible.
