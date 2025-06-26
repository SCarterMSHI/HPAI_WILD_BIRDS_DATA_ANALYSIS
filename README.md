# HPAI Wild Birds Data Analysis (USDA)

This project performs exploratory data analysis (EDA) on Highly Pathogenic Avian Influenza (HPAI) detections in wild birds using publicly available data from the USDA. It automates the ingestion of the latest dataset, validates it against a manually downloaded version, cleans the data, and visualizes trends in species, geography, and seasonality of outbreaks. The notebook provides reproducible, policy-relevant insights to support public health and environmental monitoring.

---

## Project Structure
```
HPAI_WILD_BIRDS_DATA_ANALYSIS/
├── data/
│ ├── cleaned_usda_hpai_wildbirds.csv
│ └── manual_usda_hpai_detections_wild_birds.csv
├── eda_on_usda_HPAI_wild_birds.ipynb
├── README.md
└── requirements.txt
```
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
```
---

## How to Reproduce
1. Clone the repository:
```bash
   git clone https://github.com/your-username/hpai-wild-birds-eda.git
   cd hpai-wild-birds-eda
```
2. **(Optional)** 
```
 Manually download the USDA csv file to validate the automated version:
 - Visit: [USDA HPAI Wild Birds Dataset] (https://www.aphis.usda.gov/livestock-poultry-disease/avian/avian-influenza/hpai-detections/wild-birds)
 - Scroll down and click the blue CSV button
 - Save the file as: data/manual_usda_hpai_detections_wild_birds.csv
```
3. **Install Required Packages:**
```
pip install -r requirements.txt
```
4. **Lauch the Notebook:**
```
jupyter notebook eda_on_usda_HPAI_wild_birds.ipynb
```
## Future Work
- Forecast detections using time series models
- Integrate climate and migration data for improved insights
- Build interactive dashboards using Tableau, PowerBI, or Dash
- Automate weekly csv updates using Github Actions or cron jobs
- Visualize detections geographically with interactive maps
## Author
Stacy Carter, MS
## License 
This project is provided for educational and public health analysis purposes. Data is publicly available from the USDA APHIS website.





