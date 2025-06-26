# HPAI Wild Birds Data Analysis (USDA)

This project performs exploratory data analysis (EDA) on Highly Pathogenic Avian Influenza (HPAI) detections in wild birds using publicly available data from the USDA. It includes automated data ingestion, data cleaning, and visualizations to uncover trends in species, geography, and seasonality of outbreaks.

---

## Project Structure

HPAI_WILD_BIRDS_DATA_ANALYSIS/
├── data/
│ ├── cleaned_usda_hpai_wildbirds.csv
│ └── manual_usda_hpai_detections_wild_birds.csv
├── eda_on_usda_HPAI_wild_birds.ipynb
├── README.md
└── requirements.txt

---

## Features

- **Automated data download** from USDA's backend CSV link
- **One-time validation** to compare manual vs automated datasets
- **Data cleaning**: standardizing column names, parsing dates, handling missing values
- **Visualizations**:
  - Daily HPAI detection trends
  - Top bird species and states affected
  - Seasonal detection patterns by month
  - Year-over-year detection totals
  - Heatmap of detections by month and year

---

## Sample Visualizations

- Line plot of detections over time  
- Bar charts of top species and top states  
- Monthly trends  
- Yearly bar chart  
- Heatmap

---

## Requirements

Install dependencies using:

```bash
pip install -r requirements.txt

---

## How to Reproduce
```
1. **Clone the repository:**
   ```
   git clone https://github.com/your-username/hpai-wild-birds-eda.git
   cd hpai-wild-birds-eda
   `

2. **(Optional)** 
   
   Manually download the USDA csv file to validate the automated version:
   - Visit: [USDA HPAI Wild Birds Dataset] (https://www.aphis.usda.gov/livestock-poultry-disease/avian/avian-influenza/hpai-detections/wild-birds)
   - Scroll down and click the blue CSV button
   - Save the file to:
   data/manual_usda_hpai_detections_wild_birds.csv














# HPAI Wild Birds Data Analysis

## Project Overview
This project analyzes Highly Pathogenic Avian Influenza (HPAI) detections in wild birds using a dataset provided by the USDA. The analysis involves data cleaning, exploratory data analysis (EDA), and visualizations to uncover patterns in HPAI outbreaks across different bird species, locations, and time periods.

---

## Data Source
- Dataset: [USDA HPAI Detections in Wild Birds](https://www.aphis.usda.gov/livestock-poultry-disease/avian/avian-influenza/hpai-detections/wild-birds)
- Format: CSV file
- Columns Include:
  - state - The state where detection occurred
  - county - County of detection
  - collection_date - Date when the sample was collected
  - date_detected - Date when HPAI was confirmed
  - hpai_strain - Virus strain detected
  - bird_species - Species of the affected bird
  - woah_classification - Classification based on the World Organisation for Animal Health
  - sampling_method - How the sample was collected
  - submitting_agency - Agency that reported the sample

---

## Data Quality & Cleaning
- Column Names Standardized: Converted to lowercase with no spaces
- Date Columns Converted: collection_date and date_detected formatted as datetime
- Missing Values Handled: 
  - hpai_strain replaced with "Unknown" if missing
  - Other missing values filled with "Unknown"
- No Duplicates Were Removed: Each row represents a unique detection

Final Cleaned Dataset: `cleaned_usda_hpai_wildbirds.csv`

---

## Questions Addressed:
1. How have HPAI detections changed over time?
2. Which bird species are most affected?
3. Which states report the highest detections?

---

## Visualizations
The Jupyter Notebook includes the following data visualizations:
1. HPAI Detections Over Time - (Line chart)
2. Top Species Affected - (Bar chart)
3. Geographic Spread by State - (bar chart)

### Visualizations in Tableau Public & Power BI
- Tableau Public: [place_holder]()
- Power BI: [place_holder]()

---

## How to Run the Notebook
1. Download the dataset from the USDA website: [USDA HPAI Detections in Wild Birds](https://www.aphis.usda.gov/livestock-poultry-disease/avian/avian-influenza/hpai-detections/wild-birds)
3. Run each cell to process the data and generate visualizations.
Note: The [eda_on_usda_HPAI_wild_birds.ipynb](eda_on_usda_HPAI_wild_birds.ipynb) notebook gives instructions to reproduce the cleaned dataset: `cleaned_usda_hpai_wildbirds.csv`

---

## Future Work
- Use more advanced machine learning models to predict outbreaks.
- Incorporate external climate or migration data for deeper insights.
- Automate data updates for real-time visualization dashboards.

---






