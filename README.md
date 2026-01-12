# GBV Geospatial Mapping in Rwanda

## Overview
This project analyzes and visualizes the distribution of Gender-Based Violence (GBV) cases across Rwandan districts using Python and QGIS. It transforms administrative data from the Gender Monitoring Office into clear, intuitive geospatial maps and analytical graphics. The goal is to support evidence-based decision-making by identifying GBV hotspots, revealing spatial patterns, and enabling targeted prevention and response strategies by MINIJUST, the Justice Sector, and partners.

## Data Source
The project uses secondary administrative data obtained from the Gender Monitoring Office (GMO), covering GBV cases from 2022 to date. Key variables include:
- District
- Year of occurrence
- Victim gender
- Age group
- Type of violence (Economic, Psychological, Sexual, Physical)

Rwanda’s administrative boundary shapefiles are used for spatial integration and mapping.

## Methodology
1. **Data Preparation (Python)**
   - Remove duplicates and handle missing values
   - Standardize district names and categorical fields
   - Validate records and formats
   - Aggregate GBV cases by district, year, gender, age group, and violence type
   - Generate analysis-ready tables

2. **Exploratory Data Analysis (Python)**
   - Descriptive statistics by gender, age group, and violence type
   - Trend analysis over time
   - Graphical outputs (bar charts, boxplots)

3. **Geospatial Analysis (QGIS)**
   - Join aggregated GBV data with district shapefiles
   - Create thematic maps for:
     - Overall GBV distribution
     - Psychological GBV
     - Sexual GBV
     - Physical GBV
   - Identify hotspots and spatial disparities

This workflow ensures a transparent, reproducible, and scalable pipeline from raw data to policy-ready insights.

## Tools
- **Python** (pandas, numpy, matplotlib): Data cleaning, aggregation, and analysis  
- **QGIS**: Spatial integration, hotspot visualization, and cartographic outputs  
- **GitHub**: Version control and project documentation

## Outputs
- Cleaned and aggregated datasets
- Statistical summaries and charts by:
  - Gender
  - Age group
  - Type of violence
- District-level GBV maps:
  - Overall GBV distribution
  - Psychological GBV
  - Sexual GBV
  - Physical GBV
- Policy-oriented visualizations for presentations and reports

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/GBV-Geospatial-Mapping-Rwanda.git
   cd GBV-Geospatial-Mapping-Rwanda
Create a virtual environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run data processing scripts:

bash
Copy code
python scripts/data_cleaning.py
python scripts/aggregation.py
python scripts/analysis.py
Open QGIS:

Load the processed data from data/processed/

Load Rwanda district shapefiles

Join tables by district name

Apply symbology to generate maps

Contact
Project Lead: Charles Iyamuremye
Email: your.email@example.com
Affiliation: MINIJUST / Justice Sector, Rwanda
