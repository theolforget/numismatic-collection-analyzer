# Numismatic Collection Analyzer

Theo Forget
May 29th, 2025

## Overview
This project is a data engineering pipeline that processes and analyzes my personal collection of banknotes from Numista. It takes a messy dataset and turns it into something clear and insightful, while also pulling in live exchange rates to estimate the collection’s real-world value.

## Key Features
- **Data Ingestion & Parsing**: Breaks down the unstructured 'Private comment' field into clean, usable columns.
- **Live Currency Data**: Connects to a public API to fetch real-time exchange rates, converting local denominations into USD.
- **Error Detection & Logging**: Flags entries with formatting issues or unrecognized currencies and exports them to a CSV for review.
- **Data Summaries & Visualization**: Calculates total and estimated collection value, identifies the most valuable notes, and creates clean visualizations.
- **Tech Stack**: Python, Pandas, Requests, Matplotlib.

## How to Use
1. Install the dependencies: pip install -r requirements.txt
2. Open `numismatic_analyzer.ipynb` in Jupyter Notebook.
3. Run the notebook step by step to:
- Parse and clean the data
- Fetch live exchange rates
- Calculate valuations
- Export any errors to a CSV
- View key insights and charts
5. Check the `error_entries.csv` file for any rows that need attention.

## Why I Built This
I wanted to combine my interest in numismatics with my technical skills, turning a simple CSV export into a complete data pipeline. I had just completed the IBM Python for Data Science, AI & Development course and wanted to apply what I learned in a practical project. This gave me the chance to practice real-world data engineering tasks—parsing messy fields, integrating external APIs, handling errors, and summarizing data visually.

## Future Ideas
- Pull in historical exchange rates for a better valuation over time
- Deploy the pipeline to the cloud for automatic updates
- Build a lightweight web dashboard to explore the data interactively
