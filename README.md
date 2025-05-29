# Numismatic ETL Pipeline

**Theo Forget**  
**May 29th, 2025**

## Overview
This project is a data engineering ETL pipeline that processes and analyzes my personal collection of banknotes from Numista. It takes a messy dataset and transforms it into structured, enriched data with real-time exchange rates to estimate the collection’s USD value.

## Key Features
- **Extract**: Loads semi-structured data from a Numista CSV export.
- **Transform**: Parses and cleans the 'Private comment' field, enriches data with live exchange rates, calculates USD valuations, and flags formatting issues.
- **Load**: Consolidates the cleaned dataset and exports error logs to CSV for review.
- **Visualization**: Generates summary charts and tables highlighting key insights.
- **Tech Stack**: Python, Pandas, Requests, Matplotlib.

## How to Use
1. Install the dependencies:  
 pip install -r requirements.txt
2. Open `numismatic-etl-pipeline.ipynb` in Jupyter Notebook.
3. Run the notebook step by step to:
- Extract and parse the data
- Enrich with live exchange rates
- Calculate valuations
- Export errors to a CSV
- View key insights and charts
4. Check the `error_entries.csv` file for any rows needing attention.

## Why I Built This
I wanted to combine my interest in numismatics with my technical skills, turning a simple CSV export into a complete ETL pipeline. I had just completed the IBM Python for Data Science, AI & Development course and wanted to apply what I learned in a practical project. This gave me the chance to practice real-world data engineering tasks—parsing messy fields, integrating external APIs, handling errors, and summarizing data visually.

## Future Ideas
- Pull in historical exchange rates for a better valuation over time.
- Deploy the ETL pipeline to the cloud for automatic updates.
- Build a lightweight web dashboard to explore the data interactively.
