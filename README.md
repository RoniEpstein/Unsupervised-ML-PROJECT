# Israeli Municipal Authorities Analysis
This project analyzes comprehensive data from 255 local authorities in Israel, including municipalities, local councils, and regional councils.
The analysis focuses on understanding patterns in budget allocation and identifying key factors that differentiate various types of authorities using unsupervised learning techniques.

## Project Structure
- `2018.xlsx` - Original dataset containing municipal authority data from data.gov.il and CBS
- `data preparation.ipynb` - Notebook for translating column names from Hebrew to English
- `df_2018_final.xlsx` - Dataset after column name translation
- `EDA.ipynb` - Exploratory Data Analysis notebook
- `data_after_EDA.xlsx` - Clean dataset after EDA processing
- `Unsupervised Learning.ipynb` - Main analysis notebook implementing clustering techniques
- `requirements.txt` - Project dependencies

## Data Description
The dataset contains information on all 255 local authorities in Israel for the year 2018, covering 397 variables across multiple domains:
- Basic authority information
- Regular and development budgets
- Municipal taxes
- Demographics
- Education and health metrics
- Employment and welfare statistics
- Infrastructure and transportation data
- And more

## Methodology
The analysis follows these main steps:

1. **Data Preprocessing** (`EDA.ipynb`)
   - Handles missing values using different strategies based on percentage
   - Implements outlier detection using Isolation Forest
   - Performs data validation and standardization

2. **Column Translation** (`data preparation.ipynb`)
   - Translates column names from Hebrew to English
   - Exports processed data to `df_2018_final.xlsx`

3. **Unsupervised Learning Analysis** (`Unsupervised Learning.ipynb`)
   - Implements topic-based data segmentation
   - Applies multi-stage dimensionality reduction using Kernel PCA
   - Performs clustering analysis
   - Visualizes and validates results

## Key Findings
The analysis identified three distinct clusters of municipalities:
1. Peripheral and Rural Arab Municipalities
2. Urban Mixed Population Centers
3. Established Central Jewish Municipalities

Each cluster shows unique characteristics in terms of:
- Geographic location
- Demographics
- Budget allocation
- Infrastructure development
- Resource distribution

## Setup and Installation
1. Clone the repository
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run notebooks in the following order:
   - `EDA.ipynb`
   - `data preparation.ipynb`
   - `Unsupervised Learning.ipynb`

## Dependencies
See `requirements.txt` for complete list of dependencies and versions.

## Data Flow
```
2018.xlsx (Original Data)
       ↓
EDA.ipynb
       ↓
data_after_EDA.xlsx
       ↓
data preparation.ipynb
       ↓
df_2018_final.xlsx
       ↓
Unsupervised Learning.ipynb
```

## Authors
- Odeya Hazani 
- Roni Epstein 

## References
- data.gov.il - Israeli government data portal
- Central Bureau of Statistics (CBS)
- Additional references available in the technical report
- Kaggle code credits and references can be found within the code files as comments
