# Bank Statement Automation Demo

This project demonstrates a simple, end-to-end document automation pipeline for bank statements using Python in Google Colab. It shows how to automatically extract data from a PDF, transform it into structured formats, and visualize the results.

## Project Description

1. **PDF Input**: A sample bank statement (`bank_statement.pdf`) is generated or uploaded.  
2. **Text Extraction**: Use `pdfplumber` to pull raw text from the PDF.  
3. **Field Annotation**: Identify and label each piece of text (date, description, debit/credit type, amount, balance).  
4. **Data Normalization**: Convert debit entries to negative values and credit entries to positive values.  
5. **Transaction Categorization**: Map descriptions to spending categories (e.g., Shopping, Utilities, Income).  
6. **Export**: Save the cleaned data as `parsed_transactions.csv` and `transactions.json`.  
7. **Visualization**: Display a bar chart of spend by category using `matplotlib`.  

## Repository Structure
Bank-statement-automation
  bank_statement.pdf        # Sample PDF statement
  notebook.ipynb            # Google Colab notebook with full pipeline
  parsed_transactions.csv   # Example CSV output after extraction
  transactions.json         # Example JSON output
  requirements.txt          # List of Python libraries needed
  README.md                 # This file


## How to Use

1. **Open the notebook** in Google Colab:  
   - Go to File -> Open notebook -> Upload `.ipynb file`.  
2. **Install dependencies**:  
   ```bash
   !pip install -r requirements.txt
   
3. Upload or generate the sample PDF:

  If you have bank_statement.pdf, upload it when prompted.

  Or run the PDF generation cells to create a new sample.

4. Run all cells from top to bottom.

5. Download outputs:

  parsed_transactions.csv and transactions.json will download automatically.

  Review the bar chart to see the spending breakdown by category.

Skills Highlighted

  PDF processing with ReportLab and pdfplumber.

  Document annotation via text parsing and regex.

  Data cleaning & transformation using pandas.

  Transaction categorization with keyword mapping.

  Data visualization using matplotlib.

  End-to-end automation in a notebook environment.



