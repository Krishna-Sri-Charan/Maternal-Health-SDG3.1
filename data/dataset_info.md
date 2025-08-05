# Dataset Information

## 📌 Source
The dataset used in this project is from the AI Kosh Sustainable Development Goals (SDG) portal:  
[https://www.data.gov.in/resource/sustainable-development-goals-national-indicator-framework-version-31-2021](https://www.data.gov.in/resource/sustainable-development-goals-national-indicator-framework-version-31-2021)

## 📋 Description
This dataset contains national-level indicators for tracking progress toward the United Nations Sustainable Development Goals (SDGs).  
For this project, the focus is on **SDG 3.1**: Reducing the Maternal Mortality Ratio (MMR) to less than 70 per 100,000 live births by 2030.

### Key Columns Used:
- **AreaID**: Unique ID for the country/region
- **AreaName**: Name of the country/region
- **TimePeriod**: Year of the record
- **Goal**: SDG goal number (Goal 3: Good Health and Well-being)
- **Target**: Specific SDG target (3.1: Reduce MMR)
- **Indicator**: The health metric being measured
- **DataValue**: Value of the indicator
- **Subgroup**: Demographic category (if applicable)

## 🎯 Project-Specific Use
From the dataset, the following indicators were extracted and used as features for prediction:
- Maternal Mortality Ratio (Target variable)
- Antenatal Care Coverage (%)
- Skilled Birth Attendance (%)
- Adolescent Birth Rate
- Health Expenditure (% of GDP)

The dataset was uploaded to IBM Cloud Object Storage and processed within IBM Watson Studio AutoAI.