# Carthage Data Visualization Lecture and Hackathon
#### April 29, 2025

## Overview
This project provides materials for an undergraduate lecture on data visualization and a hackathon using the College Scorecard dataset. Students will learn to analyze and visualize educational institution data using Python and popular data science libraries.

## Prerequisites
- Python 3.8 or higher
- Git
- Visual Studio Code (recommended)

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/PhysicsBen/carthage-lecture-2025.git
cd carthage-lecture-2025
```

### 2. Create and Activate Virtual Environment
```bash
python -m venv env
env\Scripts\activate
```

### 3. Update Python Install Tools
```bash
python -m pip install -U pip wheel setuptools
```

### 4. Install Required Packages
```bash
pip install -r requirements.txt
```

Required packages:
- ipykernel
- pandas
- seaborn
- plotly
- bokeh
- altair
- kagglehub
- pyyaml

## Project Structure
```
carthage-lecture-2025/
├── data_vis/
│   ├── Data Vis.pptx
│   └── data_vis.ipynb
├── hackathon/
|   ├── data/
│   |   ├── field_map.csv
│   |   ├── field_study_all_years_carthage.csv
│   |   └── institution_all_years_carthage.csv
|   ├── documentation/
│   |   ├── CollegeScorecardDataDictionary.xlsx
│   |   ├── EarningsDataErrata.pdf
│   |   ├── FieldOfStudyDataDocumentation.pdf
│   |   └── InstitutionDataDocumentation.pdf
|   ├── hackathon_data_prep.ipynb
|   └── hackathon_readme.ipynb
├── README.md
└── requirements.txt 
```

## Hackathon Data Description

## Getting Started

1. Launch Visual Studio Code:
```bash
code .
```

2. Start with `hackathon_readme.ipynb` for:
   - Dataset introduction
   - Basic visualization examples
   - Sample analyses

3. Review Data Visualization resources:
   - `Data Vis.pptx` for data visulization best practices.
   - `data_vis.ipynb` for example for making graphics 

4.  If curious, review `hackathon_data_prep.ipynb` to understand:   
    - Data processing workflow
    - Field mappings
    - Data preparation steps

## Working with the Data

The project includes three main data files created by `hackathon_data_prep.ipynb`:
1. `field_map.csv` - Data dictionary and field descriptions to understand the columns in the data files.
2. `field_study_all_years_carthage.csv` - Program-level statistics for Carthage College.
3. `institution_all_years_carthage.csv` - Institution-wide metrics for Carthage College.

## Data Sources

### Hackathon
The project utilizes College Scorecard data from the U.S. Department of Education (https://collegescorecard.ed.gov/data). In order to shrink the memory footprint needed to use this data. It has been filtered to only data associated with Carthage College. Only this filtered data is available in the `data\` folder. 

The raw College Scorecard data avaialbe on the goverment site contains the following:

#### Institution-level Data (1996-97 through 2022-23)
- Comprehensive institutional characteristics
- Student enrollment statistics
- Financial aid information
- Cost metrics
- Student outcome measurements

#### Field of Study Data (2014-15 through 2019-20)
- Program-level data by credential type
- 4-digit CIP code combinations
- Debt statistics at graduation
- Post-graduation earnings data
- Completion rates

#### Crosswalk Files (2000-01 through 2022-23)
- Links Department's OPEID with IPEDS UNITID
- Institutional identification mapping

If you choose to download the raw College Scorecard, beware it is very large. To use the the `hackathon_data_prep.ipynb` code without modification, you will need to run it on a machine with at least 32GB of ram. To run on a smaller machine, you may consider rewriting some steps to not keep the entirety of the college scorecard data in memory at once.

### Data Visualization

Data for the data visualization lecture is sourced from Kaggle data sets:
https://www.kaggle.com/datasets

In order to download Kaggle datasets, you will need to create a Kaggle account. See here for instructions:
https://www.kaggle.com/docs/datasets#using-datasets-in-notebooks

## License
This project is provided for educational purposes. All data is sourced from public domain government data or Kaggle.

## Contact
Benjamin Burch, PhD
benjaminburch@gmail.com
https://www.linkedin.com/in/benjaminburch/