# matplotlib-challenge
**Objective**: Using Pandas and Matplotlib to analyze study data and generate tables and figures for the technical report of the clinical study. 

The datasets in the "data" folder are:
- `Mouse_metadata.csv`: Mouse ID, Drug Regimen, Sex, Age_months, and Weight(g).
- `Study_results.csv`: Mouse ID, Timepoint, Tumor Volume(mm3), Metastatic Sites.

## Prerequisites
- Visual Studio Code
- Python
- Pandas
- Matplotlib
- SciPy stats

## Setup and Usage
1. Clone the `matplotlib-challenge` repository to your local computer.
2. Navigate to the cloned directory in Visual Studio Code.
3. Open the Jupyter Notebook `pymaceuticals_starter.ipynb` in the "Pymaceuticals" folder to run and view the analysis.

## Output
The Jupyter Notebook analyzes the data and generates the required DataFrames and figures for the report:
- `study_data_complete`: Datasets merged into a single DataFrame.
- `clean_study_data`: A clean DataFrame after dropping the duplicate mouse.
- `drug_regimen_summary`: DataFrame containing the summary statistics, including mean, median, variance, standard deviation, and SEM of the tumor volume for each regimen.
- `drug_regimen_agg_summary` The same summary statistics as the DataFrame above, but generated using the aggregation method.
- Bar Plots: Shows the total number of rows (Mouse ID/Timepoints) for each drug regimen using Pandas.
- Pie Charts: Shows the distribution of unique female versus male mice used in the study.
- Quartiles, Outliers and Boxplots: Shows the distribution of the tumor volume for each treatment group.
- Line Plot: Shows the tumor volume vs. timepoint for a single mouse (mouse l509) treated with Capomulin.
- Scatter Plot: Shows mouse weight vs. the average observed tumor volume for the entire Capomulin regimen.
- Correlation and Regression: Calculates the correlation coefficient and generates a linear regression model for mouse weight and average observed tumor volume for the entire Capomulin regimen.
