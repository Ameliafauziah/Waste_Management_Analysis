♻️ Singapore Waste Management Analysis (2003–2020)
📁 Dataset Overview
This project utilizes data from three key CSV files:
- waste_energy_stat.csv
- 2003_2017_waste.csv
- 2018_2020_waste.csv

These datasets contain detailed information on waste types, total waste generated and recycled, and energy savings in Singapore between 2003 and 2020.

🧹 1. Data Cleaning and Preparation
To ensure consistent structure across datasets, the following steps were performed:

- a. Renaming inconsistent columns (Total Generated ('000 tonnes) → total_waste_generated_tonne, etc.)
- b. Filling in missing values and correcting known data entry errors using .iloc[]
- c. Removing unnecessary columns such as Waste Type rows with no numeric values
- d. Dropping columns not required for analysis (e.g., waste_disposed_of_tonne)
- e. Merging datasets into a unified dataframe spanning 2003 to 2020

📈 2. Time Series Trends (2003–2020)
The trends of the following metrics were visualized over the years:

- a. Total Waste Generated
- b. Total Waste Recycled
- c. Recycling Rate

Using plotly, dual-axis bar and line charts were created for visual clarity.
We also analyzed the proportion of waste types contributing to total waste using a pie chart.

3. Waste Type Focus: Metals, construction, food, paper, plastic, nonmetal,glass
A focused analysis on ferrous and non-ferrous metals included:

- a. Tracking their annual waste generation and recycling rates
- b. Plotting waste-specific recycling performance from 2003 to 2020

Understanding how different waste contributed to the overall recycling rate

⚡ 4. Energy Saving Potential (Per Waste Type)
Certain waste types have significant energy-saving potential when recycled. Based on external energy factors (kWh saved per tonne), the project:

- a. Assigned energy saving values to plastics, paper/cardboard, glass, ferrous, and non-ferrous metals
- b. Calculated energy saved (in kWh and converted to GWh)
- c. Rounded values to two decimal points
- d. Aggregated energy saving totals per year from 2003 to 2020
