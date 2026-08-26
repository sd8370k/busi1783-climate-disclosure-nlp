# BUSI1783 Dissertation on "Readability and Sentiment of Climate-related Risk Disclosures in UK FTSE 100 Annual Reports (2021–2024)"

MSc Business Analytics, University of Greenwich
Supervisor: Dr Thamaraikani Chandrasooden

## What this project does:

Uses NLP to measure how readable and how positively/negatively worded climate disclosures are in FTSE 100 annual reports, and tests whether high-carbon firms differ from low-carbon firms.

## How to run:

1. Install packages: `pip install -r requirements.txt`
2. Open `Research_Project_Final_Part.ipynb` in Jupyter Notebook
3. Run the cells in order from top to bottom

## Note:
Extraction of text from the 208 annual report PDFs and takes more than two days. The extracted data is already saved in the `data/` folder, so you can skip the extraction stage and start from next cell onwards.

The Loughran-McDonald Master Dictionary is not included here because it is third-party. Download it from https://sraf.nd.edu/loughranmcdonald-master-dictionary/ and put it in `data/` before running score sentiment.

The annual report PDFs are not included due to file size. They were downloaded from company investor relations websites and the FCA National Storage Mechanism.

## Files in this repository:

**Notebook:**
- `Research_Project_Final_Part.ipynb` — full analysis pipeline

**Data files (in `data/` folder):**
- `company_list.xlsx`: list of 52 firms with ICB sectors
- `financial_data.xlsx` : hand-collected financial data (2021–2024)
- `panel_data_enhanced.xlsx` : financial controls panel
- `master_panel.xlsx` : merged panel before winsorisation
- `master_panel_winsorized.xlsx` : final analysis dataset (199 observations)

**Figures (in `figures/` folder):**
- `fig4_1_highcarbon_vs_lowcarbon.png`
- `fig4_2_correlation_matrix.png`
- `fig_readability_trend.png`

## Note:
Some intermediate CSV files (climate_text.csv, climate_text_clean.csv, readability.csv, sentiment.csv) could not be uploaded due to GitHub file size limits. The final analysis dataset (master_panel_winsorized.xlsx) is included and is sufficient to reproduce all results from the regression stage onwards.
