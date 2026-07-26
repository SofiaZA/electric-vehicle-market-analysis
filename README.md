# Electric Vehicle Market Analysis in Washington State

## Project Overview

This project analyzes the electric vehicle (EV) market in Washington State using a dataset containing information about registered electric vehicles. The analysis explores market composition, vehicle characteristics, manufacturer distribution, model popularity, and trends in electric vehicle adoption.

The project combines exploratory data analysis (EDA), data visualization, and a preliminary regression analysis to identify relevant patterns in the EV market and provide insights into its evolution.

## Objective

The main objective of this project is to explore the characteristics and distribution of electric vehicles registered in Washington State and identify patterns that can provide insights into the development of the EV market.

The analysis focuses on:

* Understanding the composition of the electric vehicle market.
* Identifying the most represented manufacturers and vehicle models.
* Exploring trends in EV registrations over time.
* Analyzing the distribution of electric range and other vehicle characteristics.
* Identifying potential data quality issues.
* Exploring whether vehicle registration trends can be approximated using a simple regression model.
* Deriving strategic insights from the observed market patterns.

## Dataset

The dataset contains information about electric vehicles registered in Washington State. It includes **177,866 records** and **17 variables** describing vehicle characteristics, registration information, and geographic attributes.

The dataset includes variables related to:

* Vehicle make and model.
* Model year.
* Electric vehicle type.
* Electric range.
* Base MSRP.
* Legislative district.
* Electric utility.
* Geographic information, including city, county, and postal code.

The data is primarily centered on electric vehicle registrations in Washington State.

## Methodology

The project follows a structured exploratory data analysis workflow:

1. **Data Loading and Inspection**

   * Imported the dataset and reviewed its dimensions and structure.
   * Examined data types and column information.
   * Identified missing values and potential inconsistencies.

2. **Data Cleaning**

   * Evaluated missing and zero values.
   * Reviewed categorical variables and numerical distributions.
   * Considered potential data quality issues affecting the interpretation of vehicle range and pricing variables.

3. **Exploratory Data Analysis**

   * Analyzed the distribution of electric vehicles by manufacturer.
   * Identified the most common vehicle models.
   * Examined trends in registrations by model year.
   * Explored electric range and Base MSRP distributions.
   * Investigated geographic and market patterns.

4. **Data Visualization**

   * Created visualizations using Python libraries to communicate the main findings.
   * Used charts to compare manufacturers, models, and registration trends.

5. **Regression Analysis**

   * Developed a simple linear regression model to explore the relationship between model year and the number of registered electric vehicles.
   * The model achieved:

     * **MAE:** 6,960.70
     * **RMSE:** 8,945.29
   * The results were interpreted as an exploratory analysis rather than a production forecasting model.

## Key Findings

The exploratory analysis revealed several important patterns in the Washington State EV market:

* **Tesla is the dominant manufacturer** in the dataset, with approximately **79,659 registered vehicles**, representing a substantial share of the observed EV market.
* **Model Y and Model 3** are among the most represented electric vehicle models, highlighting the strong market presence of Tesla's mass-market vehicle lineup.
* The dataset contains a significant number of **zero values in the Electric Range and Base MSRP variables**. These values may represent missing, unavailable, or non-applicable information rather than actual zero values and should therefore be interpreted carefully.
* The distribution of registrations across model years suggests a strong increase in electric vehicle adoption in more recent years.
* The simple regression analysis indicates a positive relationship between model year and the number of registered electric vehicles in the analyzed data. However, the relatively high MAE and RMSE indicate that model year alone is insufficient to accurately explain registration volumes.
* The EV market is highly concentrated among a limited number of manufacturers and models, with Tesla accounting for a particularly large share of registrations.

## Strategic Recommendations

Based on the findings, the following strategic recommendations can be considered:

* **For automakers:** Increasing the availability of competitively priced EV models could help capture demand in a market currently dominated by a small number of manufacturers.
* **For charging infrastructure providers:** Investment decisions should consider the geographic distribution and concentration of EV registrations to prioritize areas with higher potential demand.
* **For policymakers:** Continued monitoring of EV adoption trends can help inform infrastructure planning, incentives, and transportation policies.
* **For automotive businesses:** Understanding the popularity of specific manufacturers and models can support inventory planning, market positioning, and customer targeting.
* **For future analytics projects:** Additional variables should be incorporated into predictive models, including vehicle make, model, electric range, vehicle type, geographic location, and pricing information.

## Technologies

The project was developed using the following technologies and libraries:

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computing
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical data visualization
* **Scikit-learn** – Machine learning and regression modeling
* **Jupyter Notebook** – Interactive data analysis and documentation

## Project Structure

```text
electric-vehicle-market-analysis/
│
├── data/
│   └── Electric_Vehicle_Population_Data.csv
│
├── notebooks/
│   └── electric_vehicle_market_analysis.ipynb
│
├── images/
│   └── [analysis visualizations]
│
├── README.md
│
└── requirements.txt
```

The exact file structure may vary depending on the final organization of the repository.

## How to Explore the Project

To explore the project:

1. Clone or download the repository.
2. Install the required Python dependencies.
3. Open the Jupyter Notebook containing the analysis.
4. Run the notebook cells sequentially to reproduce the data cleaning, exploratory analysis, visualizations, and regression model.

Example:

```bash
git clone <repository-url>
cd electric-vehicle-market-analysis
pip install -r requirements.txt
jupyter notebook
```

The notebook provides a step-by-step walkthrough of the analysis and allows the visualizations and results to be reproduced.

## Limitations

Several limitations should be considered when interpreting the results:

* The dataset represents **registered electric vehicles**, not the complete population of EV sales or ownership activity.
* The analysis is limited to **Washington State** and may not be generalizable to other regions.
* The presence of zero values in variables such as **Electric Range** and **Base MSRP** may affect statistical analysis and requires additional data validation.
* The dataset may contain missing or incomplete information.
* Registration data does not necessarily represent current vehicle usage or active ownership.
* The regression model uses a limited set of features and is intended for exploratory purposes rather than accurate forecasting.
* The observed relationship between model year and registrations does not imply causation.

## Author

**Sofia**

Physicist | Teacher | Data Scientist

This project is part of a Data Science portfolio focused on applying data analysis and machine learning techniques to real-world datasets.
