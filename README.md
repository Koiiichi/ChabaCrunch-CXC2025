# Team ChabaCrunch - TouchBistro x UW Problem Set

This repository contains an end-to-end data science project focused on analyzing restaurant transactional data from TouchBistro. By merging and processing two key datasets—`venues.csv` and `bills.csv`—we uncover insights into customer spending behaviors and tipping trends across different geographic locations.

## Project Overview

- **Data Cleaning & Preprocessing:**  
  We start by cleaning and preprocessing the data, handling missing values, outliers, and anomalous entries. This includes downcasting numeric columns for memory efficiency and addressing peculiarities such as negative values and placeholder strings.

- **Machine Learning Modeling:**  
  To enrich the dataset, we use a Random Forest model to predict missing venue "concept" entries. This step helps us better understand the impact of venue types on tipping behavior.

- **Exploratory Data Analysis (EDA):**  
  With a refined dataset, we perform EDA to investigate tipping trends. We analyze metrics like tip percentages and absolute tip amounts by city, country, and venue type, providing actionable insights for restaurant operations.

- **Outlier Capping:**  
  We apply group-level outlier capping (using a 99th percentile threshold) to mitigate the influence of extreme values on our analysis while preserving data integrity.

## Key Insights

- **Tipping Behavior:**  
  Our analysis reveals significant variations in tipping percentages across cities. While some cities (e.g., Eads, San Diego, Monson) show high tip percentages, others (e.g., Bellingham, Greenville, Richmond Hill) hover near lower percentages.

- **Impact of Venue Type:**  
  Bars and full-service restaurants tend to receive higher tips compared to cafés and fast-casual venues, suggesting that the service environment and venue concept strongly influence tipping behavior.

- **Order Type Differences:**  
  Dine-in and bar tab transactions consistently yield higher tips than takeout or delivery orders, reflecting industry norms and customer behavior patterns.

- **No Simple National Trend:**  
  The data does not support a straightforward "US vs. Canada" tipping pattern. Instead, local cultural factors and venue mix play a more decisive role in tipping behavior.

## Repository Structure

- **`CXC - ChabaCrunch.zip`**: A compressed file containing the main analysis notebook (`notebook.ipynb`) and any related code.
- **`README.md`**: A detailed overview of the project, objectives, methodology, and key findings.

## Technologies Used

- **Language:** Python
- **Libraries/Frameworks:** Pandas, NumPy, scikit-learn, Matplotlib, Seaborn
- **Platform:** Google Colab
- **Cloud Services:** Google Drive (via gdown)
- **Utilities:** zipfile, gc (garbage collection)

## Getting Started

1. Clone this repository.
2. Open the notebook in Google Colab.
3. Follow the steps outlined in the notebook to reproduce the analysis.

## Contributing

We welcome contributions! If you'd like to improve the analysis or add new features, feel free to fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

---
