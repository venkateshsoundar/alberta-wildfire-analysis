# Wildfire Severity Analysis in Alberta: Exploring Weather and Response Factors

![Data Source: Open Alberta](https://img.shields.io/badge/Data-OpenAlberta-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-green)

## 📖 Project Overview
This repository contains an R Notebook (`DATA_602_Group_5_Project.Rmd`) analyzing historical wildfire data from Alberta (2006–2023) to understand how weather conditions and response factors influence wildfire spread and size. Through data cleaning, exploratory analysis, regression modeling, and geospatial visualization, we assess the roles of wind speed, temperature, humidity, response time, and extinguishment time in wildfire behavior.

## 🔍 Research Questions
1. **Wind Speed & Spread Rate**
   - What is the relationship between wind speed and fire spread rate? citeturn2file4

2. **Temperature & Spread Rate**
   - How does ambient temperature affect fire spread rate? citeturn2file4

3. **Response & Extinguishment Times**
   - How do response time and extinguishment time relate to fire size (hectares)?

4. **Fire Size & Weather Conditions**
   - Does initial weather (temperature, humidity, wind) predict the ultimate size of a wildfire? citeturn2file5

## 🗄️ Data
- **Source**: Wildfire dataset from Open Alberta (fp-historical-wildfire-data-2006-2023) citeturn2file4
- **File**: `fp-historical-wildfire-data-2006-2023.csv` (automatically downloaded via URL in notebook)

## ⚙️ Dependencies
Analysis is performed in R (>=4.0) with the following packages:
```r
install.packages(c(
  "mosaic",    # Data utilities and modeling
  "dplyr",     # Data manipulation
  "ggplot2",   # Static visualizations
  "e1071",     # Skewness and statistical functions
  "leaflet",   # Geospatial mapping
  "broom",     # Tidying model outputs
  "knitr",     # Notebook rendering
  "rmarkdown"  # Markdown reports
))
```

## 🚀 Rendering the Notebook
To reproduce the analysis and visualizations:
1. Clone the repo and open the R Notebook in RStudio.
2. Ensure internet connectivity for data download.
3. In RStudio, click **Run All** or **Knit** to generate the HTML output.

Alternatively, from the R console:
```r
rmarkdown::render("DATA_602_Group_5_Project.Rmd")
```

## 📑 Notebook Structure
1. **Setup & Data Import**: Load libraries and fetch the wildfire CSV.
2. **Q1: Wind Speed & Spread Rate**: EDA, correlation, and linear regression.
3. **Q2: Temperature & Spread Rate**: Scatterplots, log-transformations, and modeling.
4. **Q3: Response vs. Extinguished Times**: Data cleaning, time-delta computations, regression.
5. **Q4: Fire Size & Weather**: Multivariable regression with weather covariates.
6. **Geospatial Visualization**: Leaflet map of fire locations colored by spread category.
7. **Conclusions & Recommendations**: Key insights and model limitations.

## 🤝 Contributing
Feedback and improvements are welcome:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature`)  
3. Commit changes (`git commit -m "Add feature"`)  
4. Push branch (`git push origin feature`)  
5. Open a Pull Request

## 📜 License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---
*Prepared by DATA 602 Group 5*
