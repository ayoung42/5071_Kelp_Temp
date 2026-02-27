# Temperature Effects on Kelp: Dealing with Missing Temperature Imputation

>  We will assess various methods for imputing missing temperature data in the NWSC-MRC kelp monitoring datasets.

---

## Project Overview


- **Objective:** There is often missing data and we want to determine the best method for imputing. This in turn will enable analysis of kelp monitoring efforts as they relate to temperature.
- **Domain:** Ecology
- **Key Techniques:** knn, linear regression, time series

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:**
- NWS-MRC Data - Community Science Monitoring Efforts Performed by the Marine Resource Committees (MRCs) and Northwest Straits Commission (NWSC) 2016 - 2024
- Washington State Department of Ecology (2026). Environmental Information Management database [Environmental monitoring data portal]. Washington State Department of Ecology. A searchable database of environmental monitoring data including air, water, soil, sediment, and biological sampling. Available at: https://ecology.wa.gov/research-data/data-resources/environmental-information-management-database (accessed Feb 14, 2026).
- **Description:** This project will tackle the question of the effectiveness of imputing missing temperature values within the NWSC - MRC data set with temperature values that vary in time and space provided from a Washington State Department of Ecology (WDOE) data set. 
- **License:** 

---

## Analysis

Describe the notebooks and/or scripts used to perform the analysis. Specify the order in which the code should be run to reproduce the results.

The notebooks should be run in this order:
1. Mid_clean
2. EDA_linegraphs # for interesting intermediate EDA
3. kelp_modeling1 # imputation

Mid cleaning cleans and does some initial preprocessing of the data. EDA_line graphs produces line graphs depicting the temperature recordings over time. kelp_modeling compares different imputation methods and their effectiveness.

---

## Results

As of right now we have some preliminary results for the manual imputation method. 18 values needed to be imputed, 11 of which were orphaned because no data was found in nearby EIM sites. Of the 7 that were imputed the imputation closely matches the real observed data, so this seems to be a reasonable method for imputation. We will follow up by assessing how well this method does at predicting, as well as assessing linear regression methods.

---

## Authors
- Carter Ellis- [@EllisWebb](github.com/EllisWebb)

- Ahrial Young - [@ayoung42](https://github.com/ayoung42)
---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements
