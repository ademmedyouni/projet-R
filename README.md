
# Restaurant Tipping Analysis with R

## Project Overview
This project analyzes restaurant tipping data to uncover patterns and relationships between variables like total bill amount, tip size, and customer demographics. The analysis includes descriptive statistics, visualizations, and regression modeling to understand factors influencing tipping behavior.

## Key Features
- **Data Exploration**: Comprehensive analysis of restaurant bills and tips
- **Statistical Analysis**: Measures of central tendency, dispersion, and distribution shape
- **Data Visualization**: Histograms, boxplots, bar charts, and scatter plots
- **Regression Modeling**: Relationship between total bill and tip amount

## Dataset
The dataset contains 244 observations with the following variables:
- `total_bill`: Total bill amount (USD)
- `tip`: Tip amount (USD)
- `gender`: Customer gender (Female/Male)
- `smoker`: Smoking section (Yes/No)
- `day`: Day of week (Thur, Fri, Sat, Sun)
- `time`: Meal time (Lunch/Dinner)
- `size`: Size of the party

## Code Examples

### Data Loading
```R
mydata <- read.csv("data.csv", header = TRUE)
```

### Descriptive Statistics
```R
calculate_stats <- function(variable) {
  mean_var <- mean(variable, na.rm = TRUE)
  median_var <- median(variable, na.rm = TRUE)
  sd_var <- sd(variable, na.rm = TRUE)
  # ... and other statistics
}
```

### Visualization
```R
# Histogram of total bills
hist(mydata$total_bill,
     main = "Histogram of Total Bill",
     xlab = "Amount",
     col = "skyblue")
```

## Key Findings
1. **Gender Distribution**: 64% male customers vs 36% female
2. **Tip Amount**: Average tip was $3.00 (median $2.90)
3. **Bill Amount**: Average bill was $19.79 (median $17.80)
4. **Strong Correlation**: 0.68 between total bill and tip amount

## How to Use
1. Clone the repository
2. Open the R Markdown file in RStudio
3. Install required packages (`e1071` for skewness/kurtosis)
4. Knit the document to generate the full report

## Dependencies
- R (version 4.0+)
- R packages:
  - `e1071`
  - `ggplot2` (for enhanced visualizations)

## Contributors
- Adem Medyouni

---

For detailed analysis and visualizations, see the full R Markdown report.
