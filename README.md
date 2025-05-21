Project Overview

This project shows a complete, step-by-step pipeline to process bank statement PDF files automatically. It uses Python in Google Colab to:

Generate sample PDF statements

Extract text and annotate each field

Normalize financial data

Categorize transactions

Export structured CSV/JSON files

Visualize spend patterns

This demo highlights my ability to automate complex document workflows from start to finish.

Step-by-Step Instructions

Install Dependencies

pip install -r requirements.txt

Open the Notebook

Upload or open notebook.ipynb in Google Colab.

Upload Sample PDF

When prompted, upload demo_statement.pdf file.

Generate PDFs (Optional)

Run the PDF generation cells to create new bank statement samples.

Extract & Annotate

Run the text extraction cells using pdfplumber.

The code identifies lines starting with dates and splits fields by whitespace.

Normalize Data

Convert debit entries (Db) to negative values and credit entries (Cr) to positive values.

Categorize Transactions

Apply a simple keyword-based mapping to tag each transaction into categories like Shopping, Utilities, or Income.

Export Outputs

Download parsed_transactions.csv and transactions.json via built-in Colab commands.

Visualize Spend

Run the matplotlib cell to display a bar chart of spend by category.

Review Results

Inspect the generated CSV, JSON, and chart to verify correct automation.

Skills Demonstrated

PDF Generation: ReportLab for creating demo PDF statements.

Text Extraction: pdfplumber to pull raw text from PDFs.

Document Annotation: Regex and Python logic to label fields like date, description, amount, and balance.

Data Transformation: pandas for cleaning, normalizing, and exporting structured data.

Data Enrichment: Keyword-based mapping to categorize transactions.

Data Visualization: matplotlib for simple analytics charts.

End-to-End Automation: Orchestrating all steps in Google Colab for a self-contained demo.
